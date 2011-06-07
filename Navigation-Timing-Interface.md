Great example from Mr. Doob: [[http://mrdoob.com/lab/javascript/requestanimationframe]]

##Usage
###anonymous function
    window.requestAnimationFrame(function( time ){

    	// Time is equal to the current unix time
    	// you can use this to calculate time
    	// deltas between the calls of your
    	// requestAnimationFrame callback.
    	
    	// Write your event loop code here.
    });

###named function
    var eventLoop = function( time ){

    	// Time is equal to the current unix time
    	// you can use this to calculate time
    	// deltas between the calls of your
    	// requestAnimationFrame callback.
    	
    	// Write your event loop code here.
    };
    window.requestAnimationFrame( eventLoop );

### Signature
    window.requestAnimationFrame( callbackFunction, boundingElement )

* **callbackFunction**: The function to be called each time the page is repainted.
* **boundingElement**: Required reference to the canvas element if you are animating in a canvas context, optional if you are doing animations on with DOM elements.

## Shim:
    // requestAnim shim layer by Paul Irish ( [[http://paulirish.com/2011/requestanimationframe-for-smart-animating]] )
        window.requestAnimFrame = (function(){
          return  window.requestAnimationFrame       || 
                  window.webkitRequestAnimationFrame || 
                  window.mozRequestAnimationFrame    || 
                  window.oRequestAnimationFrame      || 
                  window.msRequestAnimationFrame     || 
                  function(/* function */ callback, /* DOMElement */ element){
                    window.setTimeout(callback, 1000 / 60);
                  };
        })();

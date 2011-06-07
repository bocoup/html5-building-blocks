The requestAnimationFrame method of the window is a new interface that allows you to pass a callback to be run every time the browser is able to repaint the window. This is much more efficient then setting up your own timer with [[setInterval]] or [[setTimeout]]. This API is still in flux, with experimental implementations in Firefox, and Chrome. For safe usage today see the cross browser shim bellow with a fallback to [[setTimeout]].

Here is a great example from Mr. Doob: [[http://mrdoob.com/lab/javascript/requestanimationframe]]

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

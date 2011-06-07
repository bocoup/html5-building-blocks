Great example from Mr. Doob: [[http://mrdoob.com/lab/javascript/requestanimationframe]]

## Usage:
    window.requestAnimationFrame(function( time ){

    	// Time is equal to the current unix time
    	// you can use this to calculate time
    	// deltas between the calls of your
    	// requestAnimationFrame callback.
    	
    	// Write your event loop code here.

    });

## Shim:
    // requestAnim shim layer by Paul Irish
    // [[http://paulirish.com/2011/requestanimationframe-for-smart-animating]]
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

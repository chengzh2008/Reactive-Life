# A Reactive Game of Life

This is a very simple applet for playing around with John Conway's [Game of Life][1]. 

[1]: http://en.wikipedia.org/wiki/Conway%27s_Game_of_Life

The actual--surprisingly simple--implementation of the game itself was largely influenced by [some slides][2] by a certain kizzx2 I found online. Of course, once somebody has pointed out the stencil API in Repa, figuring out how to use it for the game of life is pretty simple.

[2]: http://illustratedhaskell.org/index.php/2011/09/24/conways-game-of-life-with-repa/

The interesting part of the project is the interface, which is written in a functional reactive style using [reactive-banana][3]. This is really primarily a demo of how simple and concise functional reactive programming can be. 

[3]: http://www.haskell.org/haskellwiki/Reactive-banana

This is actually my very first FRP program, so it's entirely a learning experience; I've found FRP to be very easy to pick up so far. It's certainly easier than the old event-driven style I used in the past with frameworks like Swing and Tk. In fact, the FRP code has been extremely simple to write--all the actual difficulties come from having to interface with wxWidgets.
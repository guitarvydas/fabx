Fabrication explorer.

Generate JavaScript from a fab spec.

![fabx.png](fabx.png)
# Usage
![[fabxscreenshot.png]]
- load `fabx.html` into a browser
- click one of the `fill` buttons to insert canned fabrication scripts, or, enter a fabx spec manually in the `src` field (one line or many lines)
- click the `Click JavaScript from FMT specifcation` button
- observe generated JavaScript code in `equivalent JavaScript code:` textbox
	- copy/paste the generated code into your project to be used in conjunction with the Ohm-JS parser
# Status
The status line at the bottom of the screen shows
- 'OK' if the fabrication spec was successfully transpiled into JavaScript code
	- the `equivalent JavaScript code:` textbox contains the generated code
- 'FAILED' if there was an error during transpilation
	- the `equivalent JavaScript code:` textbox contains the error message(s)
	- `rightmostPosition` is the character offset from the top of the file, to the furthest point in the parse
		- this is usually where the error occurred, but, due to backtracking might indicate a different spot in the file



v1.0
	Fixed export pdf being cropped out. 
	Dimensions of pdf and images can now be seen in Console.

v1.1
	Changed circles to ellipse. 
	Changed button from 'Bubble size' to 'Text Size'. Ellipse size changes with text size and length. 

v1.2
	Now support image files.

v1.3
	Leader lines are movable.
	Floating top menu.
	Menu/button will change size with browser zoom. As a workaround, a 'Zoom Slider' is added.

v1.4
	Line width/thickness set to 1 (was 2). (Looks better in final pdf)
	'+' button added for Zoom Slider
	
v1.5
	Now renumbering ignores suffix and update the 'base'
		Eg: "9a" 	→ { base: 9, suffix: "a" }
			"9b" 	→ { base: 9, suffix: "b" }
			"9f-g" 	→ { base: 9, suffix: "f-g" }
			"10-x1" → { base: 10, suffix: "-x1" }
v1.6
	Text box can be added, resized, edited.
	If the text box is empty or has few line, need to click on the right-edge of text for it to be selectable/editable. (Empty text box don't get saved in final pdf)
	Button min size changed from 0.9 to 0.7

v1.6.1
	Removed redundant code. 
	Text box changed from dotted line to solid line. 
	Known Error: Position relative to pdf change when Zoom is changed and undo is clicked. 

v1.6.2
	Fixed position of bubble and line changing relative to pdf when zoom is changed and 'Undo' is clickedPosition

v1.7
	Added 'Text Box Size' option to change font size of text inside text box. 
	Button highlight when Leader Line Mode and Text Box Mode are enabled.
	
	
	
Note: 
	The size of bubble is linked to the zoom level. A Text Size = 30 bubble at zoom 400% will be a little smaller than Text Size = 30 bubble at zoom 200%. 
 	The quality and file size of saved pdf will depend on the zoom level at which it is saved. Pdf saved at zoom = 200% is smaller than Pdf saved at zoom = 500%.
	
	
	

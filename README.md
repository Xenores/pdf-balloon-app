<pre>



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
	Button Size updated. 

v1.7.1
	Text box position is now fixed relative to pdf while zooming. 
	Text box padding updated to reduce difference between app and saved pdf. 

v1.8
	Bubbles snap to invisible grid. 
	Added Move button. Activating move button disables edit promt when clicking balloon. 

v1.8.1
	Corrected alignment of top menu icons and texts. 

v1.8.2
	Updated text box logic. Now text box size in app is similar to that in saved pdf. 
	Added a 'How to Use' guide at the bottom of the screen

v1.8.3
	Expanded remubering logic to pure alphabet bubbles. So if you delete balloon c, all balloons d,e,f… shift back.

v1.8.4
	Fixed renumbering error when number with 3 char (Eg. 1abc,5f-g..) is deleted.
	Default balloon color set to green.
	Clicking 'Save as PDF' now opens a window asking save location in Chromium-based browsers (Chrome, Edge, Opera).

v1.8.5
	Updated balloon text size to multiply with Zoom level. Now Ballons are consistent at different zooming.

v1.9
	Save and Load project options added.
	
v1.9.1
	Fixed bubble size change after edits. 
	Error: bubble size change after Undo

v1.9.2
	Replaced buttons with icons. 
	Fixed bubble size change after Zoom -> Undo
	Fixed Undo remove multiple balloons. 

v1.9.3
	Ongoing: Show file name when project is loaded. 
	Can correctly load project with balloon and leader line.

v1.9.4
	Cosmetic update for balloon Size and Text Box Size icons.

v1.9.5
	Fixed text box not loading with project issue. 
	Fixed text box position not updated in saved pdf issue.
	Balloon Size is now saved and can now be saved and loaded with project.

v1.9.6
	loading project now show the name of pdf used. 
	Error: if pdf is already loaded window still opens. 
	
v1.9.7
	Added instructions icon. 
	Added alert if opened with firefox.
	Renamed app and added icon. 
	
v1.9.8
	Now 'image projects' can be loaded. 
	Updated undo logic to teat bubble and its line as a single state. 
	Fixed error due to bubble deleted after leader line is enabled. 

v1.9.9.1
	removed 'Move mode'. 
	Moving a balloon do not open the edit window popup. 
	Double click opens the edit popup. 
	Text Box mode now disable automatically after first click.
	
v1.9.9.2
	Reworked Text Box creation logic to make it easier to edit and resize. 	
	
v2.0
	Added auto increment for duplicate number. 

v2.1
	Grid size changed from 20 to 5 (4 times more grid points). 
	
v2.2
	Reworked the zoom logic. 
	Fixed balloon drift  during large zoom. 

v2.3
	White space added at the top for headings (=50). 
	Changed icons to be more intuitive. 
	Translated to Deutsch. 
	..NOT BACKWARD COMPATIBLE..
	
	Fixed Issue: Balloon/Text Box position changes after load project. 
	Issue: Text box size increase when loading project. 
	
	************Fixing security error when loading pdf with project. 
	
	
	
	
Note: 
	The size of bubble is linked to the zoom level. A Text Size = 30 bubble at zoom 400% will be a little smaller than Text Size = 30 bubble at zoom 200%. 
	(Undo button reloads the all bubble's size for the current zoom)
	The quality and file size of saved PDF will depend on the zoom level at which it is saved. PDF saved at zoom = 200% is smaller than PDF saved at zoom = 500%.
	Since app takes time to update edits, continuous and rapid zoom/clicks may cause errors due to incorrect update of history stack. 
	
	
Bugs: 
	Text Box dimensions resets when zoomed: Fixed
	Text Boxes are generated dynamically in the end. Therefor, the dimension might differ from what is in the app. - v1.7.1: The difference is now minor.
	Text box position isnt locked to pdf, so relative position can change if zoom is varied: - v1.7.1 Fixed.
	Text Box Dimensions dont update in saved pdf after zoom is changed. Workaround- resize after zoom to update. v1.8.2
	
	

	
Prompt: In my web app for ballooning pdf/image file, I added an option to save (save-project-btn) and load (load-project-input)the project as json. The json need to save bubbles, lines, text boxes and zoom level. So later when I load the json after opening the pdf, it will load the bubbles and other items that I can edit. Currently its not working. Code: 

In my web app for ballooning pdf/image file, I want the balloons (with number/text) of a 'Balloon Text Size' to be consistent at different zoom level. Currently, if I make balloon at one zoom, then change zoom and click the new balloon appear to be same size as the first balloon (after scaling for new zoom). BUT sometimes when I click Undo, the size of bubbles that I created changes



</pre>

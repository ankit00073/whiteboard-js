# whiteboard-js
**Project Structure:**

**1. Create a project folder with the following structure:**
   ├── index.html
   ├── style.css
   └── script.js

**2. **HTML Structure (index.html)****

**3. **CSS Styling (style.css)****
   -> Create a CSS file to style the whiteboard and buttons as needed.
   
**4.JavaScript File (script.js)**
  The script.js file in this project contains the client-side JavaScript code responsible for creating a whiteboard with drawing capabilities, along with undo and delete functionality. Below is an overview of   its key features:
  
 ** Initialization:**
  
  It initializes variables and retrieves necessary HTML elements from the DOM, including the canvas, delete button, and undo button.
  The canvas element is used for drawing.
  Drawing Functions:
  
  startDrawing(e): This function is triggered when the mouse button is pressed (mousedown) on the canvas. It begins recording the drawing path.
  draw(e): Handles the actual drawing process while the mouse is moved (mousemove) over the canvas. It records the mouse position and redraws the canvas.
  stopDrawing(): Stops the drawing process when the mouse button is released (mouseup) or when the mouse pointer leaves the canvas area (mouseout).
  Canvas Management:
  
  redrawCanvas(): Clears the canvas and redraws all recorded drawing paths from the objects array. It's used to refresh the canvas with the current drawings.
  Undo and Clear:
  
  clearWhiteboard(): Clears the entire whiteboard by resetting the objects array and calling redrawCanvas().
  handleUndo(): Removes the last drawn object from the objects array, effectively undoing the most recent drawing action.
  Object Management:
  
  addObjectToCanvas(path): Adds a drawing path to the objects array. Each object in the array represents a collection of points that make up a drawing.
  Event Listeners:
  
  Event listeners are set up for mouse interactions (mousedown, mousemove, mouseup, mouseout) on the canvas, as well as for the delete and undo buttons.
  This JavaScript file enables users to draw on the canvas, undo their drawings, and clear the entire whiteboard. It achieves this by managing drawing data in the objects array and continuously redrawing the    canvas to display the current state of the whiteboard.


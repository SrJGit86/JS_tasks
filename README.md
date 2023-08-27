
#  1. Whiteboard with Delete and Undo Buttons

A simple interactive whiteboard application built using HTML5 Canvas and JavaScript. The application allows you to draw on the canvas, delete your drawings, and undo your previous drawing actions.

## Features
Draw on the canvas using your mouse.
Delete all the drawings on the canvas with the "Delete" button.
Undo your last drawing action using the "Undo" button.

## Usage
- Drawing: Click and drag your mouse on the canvas to draw lines.
- Delete: Click the "Delete" button to clear the canvas and remove all drawings.
- Undo: Click the "Undo" button to remove the most recent drawing action.

## Customization

You can customize the appearance of the whiteboard by modifying the CSS styles in the <style> section of the HTML file (index.html). The following styles are available for customization:

- Background color of the canvas.
- Border properties of the canvas.
- Font family and text styles.


## JavaScript Logic
The whiteboard application's functionality is powered by JavaScript code that handles user interactions, drawing on the canvas, and managing actions like deletion and undo.
#### Canvas Setup

fetches the canvas element from the HTML using its id and obtains a 2D rendering context (ctx) which provides methods for drawing shapes, paths, and text on the canvas.

#### Drawing Interaction
 functions manage the drawing interactions is:
 - startDrawing: Initializes a new drawing path when the mouse is pressed down.
- draw: Continuously adds points to the temporary path and redraws the canvas.
- stopDrawing: Finalizes the drawing action and adds the path to the objects array.

#### Managing Drawings
The objects array stores drawing paths, and the addObjectToCanvas function appends a new path to the array and triggers a redraw.

#### Redrawing the Canvas
The redrawCanvas function clears the canvas and then iterates through the objects array to redraw all saved paths.

#### Deleting and Undoing
functions respond to button clicks is:
- clearWhiteboard: Clears all drawings on the canvas.
- handleUndo: Removes the most recent drawing action.

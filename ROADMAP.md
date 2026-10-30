# Pen Draw roadmap

Current version: see the number shown in the bottom-right corner of the app.

## Done

- Pen, eraser, six fixed colours and six custom colours (hold to edit), with a detachable colour window
- Layers: show/hide, reorder, opacity, rename (✎ on each row). The grid is a special bottom layer; measurements are a special top layer, shown or hidden from the Measure drawer.
- Shapes, in two columns with the simple ones first and the vanishing point last, and the actions grouped together (v0.34.1): rectangle, oval, arc, triangle, line (a straight stroke, selectable and movable), parallelogram (drag from one corner to the other: one edge at 30 degrees, one vertical, aligned with the isometric grid). Polygon: tap each corner. Tap the first corner or Close polygon to close it, or Finish as open line. Undo removes the last corner while drawing. A dashed line and ring mark the start. Corners snap to the grid, the nearest line, or nothing. Open lines are not selected as a whole or filled. Closed polygons move, but cannot yet be resized or rotated, and have no dimension lines (v0.32.1). Arcs have a bulge handle to change their depth, and a radial handle at each end to move that end round the circle (up to 350 degrees, and past the other end to a reversed arc). The centre handle turns the whole arc about its centre; tapping it locks the centre in place. With the lock on, an end handle places its end anywhere, snapping to other ends or the grid. An arc's radius is limited to 10 inches.
- Dimension lines on rectangles, ovals, arcs and triangles. The Dims button: a tap shows or hides them on all shapes, and a hold opens the Dims drawer, with two checkboxes: Show dimension lines while drawing, and Maintain dimension lines. Shape dims shows them on the selected shape. Circles and arcs show their diameter (v0.31.7).
- Brush: round, soft, square, flat and spray shapes, with size, opacity, colour and Pencil pressure (harder means bigger and darker). Brush strokes are undoable but not editable. The shapes wrap three across, and a sample box shows the current brush (v0.31.3).
- Fill, text (font, size, colour, bold), and pictures (SVG, PNG, JPEG, WebP, GIF)
- Select, move, resize, rotate, cut, copy, paste, delete
- Grid, with a default spacing of 1/4 in (v0.34.1): square or isometric style (isometric has vertical, 30 and 150 degree, and horizontal guide lines), inches or centimetres, snap to grid, spacing changeable at any time. Isometric snapping picks the nearest lattice point (v0.33.0).
- Vanishing point: one point, placed by tapping and moved by dragging. Dashed guides run from it through each rectangle and polygon corner. Removed with Remove vanishing point (v0.33.0). A tap on the Grid button shows or hides the grid; holding it opens the Grid drawer (v0.31.4). Keeps its true spacing after a saved calibration is loaded (v0.31.1)
- Measure: hold for a drawer with Snap to (Grid, Nearest line or None), Sticky readings that stay until Erase All, and Inches or Centimetres. Nearest line snaps to pen, brush, rectangle and oval outlines, not arcs, triangles, text or pictures. Changing units relabels sticky readings at once (v0.31.2, v0.31.5)
- Scale calibration with an on-screen 150 mm ruler and a credit card, in Settings (gear in the top bar). The grid and dimension lines need a calibrated scale: turning either on starts calibration first, then turns it on (v0.31.9)
- Project save and open (.pendraw), New project with Cancel / Delete / Save
- File menu: new, open, save as drawing, PNG or JPEG, copy PNG, and export to PDF, PNG or JPEG on US Letter at 300 dpi. Top bar grouped with separators; app icon with the version in the corner
- Select: a Pencil or finger resting on an object doesn't move it until it has moved clearly
- PNG export and PDF export at true size on US Letter (300 dpi, visible layers only)
- Undo and redo, limited to 15 steps

## Next

- **Pixel selection on pictures.** Two tools, rectangle and lasso. Cut makes a new picture and leaves a hole. Copy makes a new picture and leaves the original. Delete erases the selected pixels. Fill paints the selection with the current colour.
- **Scale in project files.** Save the scale with each project. When a project with a different scale is opened, ask whether to use the project's scale or this device's.
- **PDF options.** Choose the page position, and add an optional print margin.
- **iPad testing.** Check the arc frame, the colour window, and the drawer behaviour on a real device.

## Ideas, not yet planned

- **On hold: brush from a clipboard bitmap.** Either a sixth brush shape that stamps a copied image as its tip, or a texture the brush paints with. Needs the image stored in the project file.
- Free painting limited to a selection. Not needed for now.
- Printing the grid at a chosen spacing, separate from the on-screen grid.
- Using the calibrated scale to set a default grid spacing.

## Known limits

- Undo keeps 15 steps.
- Canvas: taps line up with the drawing after the canvas changes size (v0.32.2).
- Imported pictures are a single object. Their parts cannot be selected separately, until pixel selection is added.
- Scale is saved on this device only, until scale-in-project is added.
- Dimension lines can only be turned on before drawing a rectangle or oval.
- Measurements are not saved with the drawing, only the visibility of their layer.
- The vanishing point and its guides are not saved with the drawing.

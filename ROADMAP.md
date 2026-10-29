# Pen Draw roadmap

Current version: see the number shown in the bottom-right corner of the app.

## Done

- Pen, eraser, six fixed colours and six custom colours (hold to edit), with a detachable colour window
- Layers: show/hide, reorder, opacity. The grid is a special bottom layer.
- Shapes: rectangle, oval, arc, triangle. Arcs have a bulge handle to change their depth, and a radial handle at each end to move that end round the circle (up to 350 degrees, and past the other end to a reversed arc). The centre handle turns the whole arc about its centre; tapping it locks the centre in place. With the lock on, an end handle places its end anywhere, snapping to other ends or the grid. An arc's radius is limited to 10 inches.
- Dimension lines on rectangles, ovals, arcs and triangles: Dims shows them on all shapes, Shape dims shows them on the selected one. Circles and arcs show their diameter.
- Brush: round, soft, square, flat and spray shapes, with size, opacity, colour and Pencil pressure (harder means bigger and darker). Brush strokes are undoable but not editable.
- Fill, text (font, size, colour, bold), and pictures (SVG, PNG, JPEG, WebP, GIF)
- Select, move, resize, rotate, cut, copy, paste, delete
- Grid: inches or centimetres, snap to grid, spacing changeable at any time
- Dimension lines on rectangles and ovals, and a measure tool
- Scale calibration with an on-screen 150 mm ruler and a credit card
- Project save and open (.pendraw), New project with Cancel / Delete / Save
- PNG export and PDF export at true size on US Letter (300 dpi, visible layers only)
- Undo and redo, limited to 15 steps

## Next

- **Pixel selection on pictures.** Two tools, rectangle and lasso. Cut makes a new picture and leaves a hole. Copy makes a new picture and leaves the original. Delete erases the selected pixels. Fill paints the selection with the current colour.
- **Scale in project files.** Save the scale with each project. When a project with a different scale is opened, ask whether to use the project's scale or this device's.
- **PDF options.** Choose the page position, and add an optional print margin.
- **iPad testing.** Check the arc frame, the colour window, and the drawer behaviour on a real device.

## Ideas, not yet planned

- Free painting limited to a selection. Not needed for now.
- Printing the grid at a chosen spacing, separate from the on-screen grid.
- Using the calibrated scale to set a default grid spacing.

## Known limits

- Undo keeps 15 steps.
- Imported pictures are a single object. Their parts cannot be selected separately, until pixel selection is added.
- Scale is saved on this device only, until scale-in-project is added.
- Dimension lines can only be turned on before drawing a rectangle or oval.
- Measurements are not saved with the drawing.

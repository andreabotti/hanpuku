# com.sci.iD3 #

Adding support for using d3.js code directly in Illustrator, with some nuances.

### Panels:
- Data
 - Tasks
  - Load, edit data
 - Views
  - Raw data editor + data list preview
- Connections
 - Tasks
  - Connect / disconnect data and graphic items
  - Connect / disconnect graphic items and data
  - Inspect which datum-graphic item connections exist
  - Duplicate existing graphic items based on the data
  - Modify the current selection based on connected data
 - Views
  - Selection list + dom preview (linked highlighting)
  - Selection list + data list preview (drawn links, linked highlighting)
  - Linked highlighting (Selection list + Dom preview), Drawn link (Selection list + data list preview) Overlay
  - Selection Query tools
- Influence
 - Tasks
  - Perform basic manipulations of graphic items' attributes with respect to their connected data
 - Views
  - Position, Scale, Rotation, Color, Shape influence tools + dom preview
- JS, CSS, Sample menu
 - Tasks
  - Reuse existing D3 visualization techniques / code ("Import")
  - Connect / disconnect data and graphic items in a more automated way
  - Perform advanced manipulations of graphic items' attributes (e.g. techniques that require interactivity, like a force-directed layout)
  - Reuse advanced connections / manipulations on the web ("Export")
 - Views
  - JS code editor + dom preview (+ Chrome debugging widget?)
  - CSS code editor + dom preview
  - Sample library (+ documentation?)

### TODO:

#### High priority
- Fix Isolation Mode bug
- Support text
- Documentation, iD3-specific Examples
- Import directly from Examples tab
- Bundle for user testing (start a release cycle?)

#### Medium priority
- Support HTML conversion to SVG + a more elegant way to incorporate new SVG elements
- Regex search/replace in text editors (esp. data)
- Replace textareas with ace editors
- Embed the Chrome debugging window as a view
- Export as/to web page tool
- Embed data, js, css files inside the .ai file (preserve layer-level properties while I'm at it)
- Load multiple js, css files, distinguish between js libraries and scripts (run the former immediately)

#### Low priority (probably next paper)
- Bindings tab
- Selection query tools
- Dom preview selection functionality
- Influence tab
- Add some kind of placeholder for unsupported items like blends or graphs?
- Support Text, Gradients, CMYK color, stroke properties (dashes, cap, etc.), Masks
- Support binding to path points (you can get around this by being creative
  with your data abstraction!)
- Walk through HBO Example

#### Very low priority
- Investigate what it would take to make an Inkscape clone
- It would be cool to convert between canvas elements / bitmaps
- Windows support
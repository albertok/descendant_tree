Draws a family tree in a descendant chart format (all descendants of an individual).

Click on a node to expand/collapse all descendants. 

Also includes a family book that shows the same data in a different format (see book.html).

Use #sourcename to load a specific JSON file.
  - For example, 0.0.0.0:8000#stark loads json/stark.json

Trees are stored in a simple JSON format, and repeating portions can be handled using the "source"
attribute.

  - For example, { "name":"John Smith", "source":"json/children_of_john_smith.json" }

  - This is useful for trees with cycles (cousins marrying each other) and multiple trees 
    sharing the same descendants (this is common if you have trees for more than one of your
    ancestors).

Uses d3.js to draw the tree.

  - Based on Rob Schmuecker’s example: http://bl.ocks.org/robschmuecker/7880033

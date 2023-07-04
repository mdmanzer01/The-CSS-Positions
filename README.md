# The-CSS-Positions
Example code snippet that demonstrates the different CSS positions:

html
Copy code
<!DOCTYPE html>
<html>
<head>
  <style>
    .container {
      height: 200px;
      width: 400px;
      background-color: lightgray;
      border: 1px solid black;
    }

    .box {
      height: 50px;
      width: 50px;
      background-color: yellow;
      border: 1px solid black;
      margin: 10px;
    }

    .static {
      position: static;
    }

    .fixed {
      position: fixed;
      top: 10px;
      right: 10px;
    }

    .sticky {
      position: sticky;
      top: 10px;
    }

    .relative {
      position: relative;
      top: 10px;
      left: 10px;
    }

    .absolute {
      position: absolute;
      bottom: 10px;
      right: 10px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="box static">Static</div>
    <div class="box fixed">Fixed</div>
    <div class="box sticky">Sticky</div>
    <div class="box relative">Relative</div>
    <div class="box absolute">Absolute</div>
  </div>
</body>
</html>
Let's go through each CSS position:

position: static; - This is the default position. Elements with position: static; are positioned according to the normal flow of the document. They are not affected by the top, bottom, left, or right properties. In the example, the "Static" box is positioned normally within the container.

position: fixed; - Elements with position: fixed; are positioned relative to the browser window. They do not scroll with the page. The top, bottom, left, and right properties can be used to control the exact position. In the example, the "Fixed" box is fixed to the top-right corner of the window.

position: sticky; - Elements with position: sticky; are positioned based on the user's scroll position. They are initially positioned according to the normal flow, but become "sticky" when they reach a specified threshold (e.g., the top of the viewport). The top, bottom, left, and right properties can be used to control the position. In the example, the "Sticky" box is initially positioned normally but becomes sticky when scrolling down.

position: relative; - Elements with position: relative; are positioned relative to their normal position in the document flow. The top, bottom, left, and right properties can be used to offset the element from its normal position. In the example, the "Relative" box is positioned 10 pixels down and 10 pixels to the right from its normal position.

position: absolute; - Elements with position: absolute; are positioned relative to their nearest positioned ancestor. If there is no positioned ancestor, they are positioned relative to the initial containing block (usually the window). The top, bottom, left, and right properties can be used to specify the exact position. In the example, the "Absolute" box is positioned 10 pixels up from the bottom and 10 pixels from the right edge of the container.

These CSS positions provide flexibility in controlling the layout and positioning of elements on a web page.

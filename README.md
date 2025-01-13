<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hover GIF Animation</title>
  <style>
    /* Style for the container of the GIF */
    .gif-container {
      display: inline-block;
      overflow: hidden;
      position: relative;
      cursor: pointer;
    }

    /* Style for the GIF/image */
    .gif-container img {
      transition: transform 0.3s ease;
      width: 100%; /* Adjust the width as needed */
    }

    /* Animation when hovered */
    .gif-container:hover img {
      transform: scale(1.2) translateX(10px) translateY(-10px);
    }
  </style>
</head>
<body>
  <h1>Hover over the GIF to see the animation!</h1>

  <!-- GIF container -->
  <div class="gif-container">
    <img src="https://www.teahub.io/photos/full/288-2886370_illustration.gif" alt="Black Panther GIF">
  </div>
</body>
</html>

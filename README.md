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
    }

    /* Style for the GIF/image */
    .gif-container img {
      width: 100%; /* Adjust the width as needed */
      transition: transform 0.5s ease; /* Smooth transition for the hover effect */
    }

    /* Hover effect */
    .gif-container:hover img {
      transform: scale(1.2) translate(20px, -20px); /* Adjust the movement and zoom */
    }
  </style>
</head>
<body>
  <h1>Hover over the GIF to see the effect!</h1>

  <!-- GIF container -->
  <div class="gif-container">
    <img src="https://www.teahub.io/photos/full/288-2886370_illustration.gif" alt="Cyberpunk GIF">
  </div>
</body>
</html>

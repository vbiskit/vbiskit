<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hover Image Animation</title>
  <style>
    /* Style for the container of the image */
    .image-container {
      display: inline-block;
      overflow: hidden;
      position: relative;
    }

    /* Style for the image */
    .image-container img {
      width: 100%; /* Adjust the width as needed */
      transition: transform 0.5s ease; /* Smooth transition for the hover effect */
    }

    /* Hover effect */
    .image-container:hover img {
      transform: scale(1.2) translate(20px, -20px); /* Adjust the movement and zoom */
    }
  </style>
</head>
<body>
  <h1>Hover over the image to see the effect!</h1>

  <!-- Image container -->
  <div class="image-container">
    <img src="https://via.placeholder.com/500" alt="Placeholder Image">
  </div>
</body>
</html>

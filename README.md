# Interactive Black Panther Mouse Move Effect

## Description
This project demonstrates an interactive mouse movement effect applied to an image, such as the Black Panther image. The image and eyes move in response to the mouse's position, creating a dynamic, engaging user experience. It also includes a cool typing SVG animation and a badge linking to my repositories.

## Features
- Interactive image with mouse move effect.
- Eyes follow the mouse cursor inside the image.
- Cool typing animation using SVG.
- Badge for exploring my GitHub repositories.
- Fun GIF showcasing the effect.

## Demo

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&pause=1000&color=7B00FF&center=true&vCenter=true&width=380&lines=Script+Kiddie" alt="Typing SVG">
</p>

<p align="center">
  <a href="https://github.com/biskit069?tab=repositories"><img src="https://img.shields.io/badge/-Explore%20my%20Repos-24292e?style=for-the-badge&logo=Github"></a>
</p>

<!-- Add an interactive GIF or image that will move -->
<div style="position: relative; width: 300px; height: 300px;">
  <img src="https://via.placeholder.com/300x300" alt="Black Panther" class="image" style="width: 100%; height: 100%; object-fit: cover;">
  <div class="eye left" style="position: absolute; top: 40%; left: 30%; width: 30px; height: 30px; border-radius: 50%; background-color: white;"></div>
  <div class="eye right" style="position: absolute; top: 40%; right: 30%; width: 30px; height: 30px; border-radius: 50%; background-color: white;"></div>
</div>

<script>
  const eyes = document.querySelectorAll('.eye');
  const image = document.querySelector('.image');

  document.addEventListener('mousemove', (e) => {
    const { clientX: mouseX, clientY: mouseY } = e;
    const { left, top, width, height } = image.getBoundingClientRect();

    const relX = (mouseX - left) / width;
    const relY = (mouseY - top) / height;

    // Move eyes
    eyes.forEach((eye) => {
      const offsetX = (relX - 0.5) * 50;
      const offsetY = (relY - 0.5) * 50;
      eye.style.transform = `translate(${offsetX}px, ${offsetY}px)`;
    });

    // Optional: Add a slight movement effect to the image itself
    const moveX = (relX - 0.5) * 20;
    const moveY = (relY - 0.5) * 20;
    image.style.transform = `translate(${moveX}px, ${moveY}px)`;
  });
</script>

## Installation

To use this interactive effect, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/biskit069/interactive-mouse-move-effect.git

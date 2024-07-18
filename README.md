<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Troll Button</title>
    <style>
      #trollButton {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        padding: 10px 20px;
        background-color: #4caf50;
        color: white;
        border: none;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <button id="trollButton">Click me!</button>

    <script>
      const button = document.getElementById("trollButton");
      button.addEventListener("mouseover", () => {
        const x = Math.random() * window.innerWidth;
        const y = Math.random() * window.innerHeight;
        button.style.left = `${x}px`;
        button.style.top = `${y}px`;
      });
    </script>
  </body>
</html>

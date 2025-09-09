🎯 Custom Cursor Effect

This project demonstrates how to create a custom cursor using HTML, CSS, and JavaScript.
Instead of the default mouse pointer, a circle follows the mouse movement across the screen.

🚀 Features

🖱️ Real-time mouse tracking

🎨 Customizable cursor (size, color, border)

⚡ Smooth and lightweight (pure JS, no libraries)

💻 Beginner-friendly

🛠️ Tech Stack

HTML5 → Structure of the page

CSS3 → Styling & cursor design

JavaScript (Vanilla JS) → Mouse tracking functionality

📂 Project Structure
📁 Custom-Cursor
 ┣ 📄 index.html
 ┣ 📄 style.css
 ┗ 📄 script.js

📝 Code Overview
HTML
<div id="main">
  <div class="cursor"></div>
</div>

CSS
.cursor {
  width: 30px;
  height: 30px;
  border: 2px solid red;
  border-radius: 50%;
  position: absolute;
  pointer-events: none;
  transform: translate(-50%, -50%);
}

JavaScript
var main = document.querySelector("#main");
var crsr = document.querySelector(".cursor");

main.addEventListener("mousemove", function (dets) {
  crsr.style.left = dets.clientX + "px";
  crsr.style.top = dets.clientY + "px";
});

🎥 Demo
<img width="1918" height="865" alt="image" src="https://github.com/user-attachments/assets/b58d1411-8fbc-4f02-b429-d7656f678fc5" />


👉 Move your mouse around and see the custom cursor follow it.

📌 How to Run

Clone this repository

git clone https://github.com/your-username/custom-cursor.git


Open index.html in your browser

Move your mouse and enjoy the effect! 🎉

🌟 Future Enhancements

Smooth animation with GSAP or CSS transitions

Different cursor styles (glowing, pulsing, trailing effect)

Interactive hover effects on elements

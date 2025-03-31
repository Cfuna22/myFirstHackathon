.

📌 README.md
md
Copy
Edit
# 🍔 Responsive Mobile Menu with Animated Hamburger  

This project implements a **responsive mobile navigation menu** using **HTML, CSS, and JavaScript**. The menu includes an **animated hamburger icon** that transforms into an "X" when clicked.  

## 🚀 Features  
✅ Animated **hamburger menu** (opens/closes smoothly)  
✅ **Responsive design** for mobile & desktop  
✅ **CSS animations** for visual effects  
✅ **Vanilla JavaScript** for interactivity  
✅ **Lightweight & easy to customize**  

## 📸 Preview  
![Mobile Menu GIF](preview.gif) *(Add a screenshot or GIF here!)*  

## 🛠️ Technologies Used  
- **HTML5** – Structure of the menu  
- **CSS3** – Styling & animations  
- **JavaScript (ES6)** – Menu toggle functionality  

## 🏗️ Installation & Usage  
### 1️⃣ Clone the Repository  
```
git clone https://github.com/your-username/mobile-menu.git  
cd mobile-menu
2️⃣ Open index.html in a browser
No installation needed! Just open the file in a browser and test it.
```
```
📝 Code Overview
HTML Structure (index.html)
html
Copy
Edit
<nav>
    <div class="navbar__toggle" id="mobile-menu">
        <span class="bar1"></span>
        <span class="bar2"></span>
        <span class="bar3"></span>
    </div>
    <ul class="navbar__menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
    </ul>
</nav>
CSS Styles (styles.css)
css
Copy
Edit
.navbar__toggle {
    position: absolute;
    top: 20px;
    right: 20px;
    width: 30px;
    height: 25px;
    cursor: pointer;
    z-index: 1000;
}

.navbar__toggle span {
    display: block;
    background: black;
    height: 4px;
    width: 100%;
    margin: 5px 0;
    transition: all 0.3s ease;
}
```
```
/* Animation when menu is active */
.is-active .bar1 {
    opacity: 0;
}
.is-active .bar2 {
    transform: translateY(8px) rotate(45deg);
}
.is-active .bar3 {
    transform: translateY(-8px) rotate(-45deg);
}
JavaScript (app.js)
js
Copy
Edit
const menu = document.querySelector('#mobile-menu');
const menuLinks = document.querySelector('.navbar__menu');

menu.addEventListener('click', function () {
    menu.classList.toggle('is-active');
    menuLinks.classList.toggle('active');
});
```
📜 License
This project is open-source and available under the MIT License.

🤝 Contributing
Feel free to submit issues or pull requests to improve this project!

🔗 Connect
👤 Abel Sifuna

GitHub: https://github.com/Cfuna22

Twitter: https://www.twitter.com/sifuna_abe71661


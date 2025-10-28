# 🌌 Hacktoberfest Code Galaxy

![Hacktoberfest Badge](https://img.shields.io/badge/Hacktoberfest-2025-blueviolet?style=flat-square&logo=github)
![HTML](https://img.shields.io/badge/HTML-5-orange?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS-3-blue?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?style=flat-square&logo=javascript)

**Hacktoberfest Code Galaxy** is a CSS and JavaScript art project inspired by the creativity of open-source.  
It visualizes a glowing galaxy of animated orbs, celebrating the spirit of collaboration and code during Hacktoberfest 🌠.

---

## 🚀 Live Demo
[GitHub Pages Link][(https://couragecodejourney.github.io/hacktoberfest-code-galaxy)](https://couragecodejourney.github.io/hacktoberfest-code-galaxy/)

---

## 🧩 Features
- Pure **HTML**, **CSS**, and a touch of **JavaScript**
- Smooth galaxy-inspired animations
- Lightweight and fully responsive design
- Hacktoberfest-themed color palette and energy ✨

---

## 🛠️ Tech Stack
- **HTML5** for structure  
- **CSS3** for styling, gradients, and animations  
- **JavaScript** for dynamic interactivity  

---

## 🖥️ Running Locally

To run this project locally on your computer:

```bash
# Clone this repository
git clone https://github.com/CourageCodeJourney/hacktoberfest-code-galaxy.git

# Navigate to the project directory
cd hacktoberfest-code-galaxy

# Open index.html in your browser
````

No dependencies or installations required — it’s pure frontend code 💻

---

## 🎯 Contributing

Contributions are welcome — this project is open for **Hacktoberfest**!
You can contribute by:

* 🌈 Adding new color themes
* ✨ Improving animations
* 🪐 Adding stars, constellations, or visual effects
* 🧠 Refactoring or cleaning CSS
* 🧩 Adding interactivity (e.g., mouse hover galaxy trails)

### How to Contribute

1. **Fork** this repository
2. **Create a new branch**

   ```bash
   git checkout -b feature-name
   ```
3. **Make your changes and commit**

   ```bash
   git commit -m "Add new galaxy animation"
   ```
4. **Push to your fork**

   ```bash
   git push origin feature-name
   ```
5. **Submit a Pull Request**

All valid pull requests during October count toward your Hacktoberfest goals ✅

---

## 🪩 Hacktoberfest

This project proudly participates in [Hacktoberfest 2025](https://hacktoberfest.com/) —
an annual celebration of open-source software hosted by **DigitalOcean**, **Appwrite**, and **GitHub**.

Make your contribution between **October 1–31** and join thousands of developers in building the open web 🌍

---

## 📸 Preview (Coming Soon)

![Project Preview](assets/hacktoberfest.jpg)


---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
You’re free to use, remix, and improve — just give credit where it’s due 🌟

---

## 💫 Author

Built with passion by **[Courage Paul (CourageCodeJourney)](https://github.com/CourageCodeJourney)**

> “Creativity begins when you turn logic into art.” 🌌
## ✨ Shining Stars Animation

This animation adds a beautiful shining stars effect to the background of the webpage, creating a galactic theme for the project.  

### 🪐 Preview
![Stars Animation Preview](https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif)

### 💻 How It Works
The effect uses CSS animations with multiple layers of moving star textures to simulate a galaxy-like motion.

```html
<!-- Shining Stars Animation -->
<div class="stars"></div>
<div class="twinkling"></div>

<style>
  .stars, .twinkling {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: block;
    z-index: -1;
  }

  .stars {
    background: url('https://www.script-tutorials.com/demos/360/images/stars.png') repeat;
    animation: moveStars 200s linear infinite;
  }

  .twinkling {
    background: url('https://www.script-tutorials.com/demos/360/images/twinkling.png') repeat;
    animation: moveTwinkling 200s linear infinite;
  }

  @keyframes moveStars {
    from {background-position: 0 0;}
    to {background-position: -10000px 5000px;}
  }

  @keyframes moveTwinkling {
    from {background-position: 0 0;}
    to {background-position: 10000px 5000px;}
  }
</style>

---

## 🎵 Galaxy Music / Sound Toggle

This feature adds background galaxy music that users can toggle on or off using a floating button in the webpage.

### 🎧 Preview
![Galaxy Music Toggle Demo](https://github.com/sania28/hacktoberfest-code-galaxy/assets/your-github-username/demo-music-toggle.gif)

*(Replace with your actual preview GIF or screenshot if available.)*

### ⚙️ How It Works
- A background music file (royalty-free) is embedded in the webpage using the HTML `<audio>` tag.  
- A JavaScript toggle button lets users **play or pause** the sound.  
- The button is styled to match the **galactic theme** of the project.  

### 🧠 Code Snippet

```html
<audio id="bgMusic" loop>
  <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
</audio>
<button id="musicToggle">🔊 Play Music</button>
<script>
  const music = document.getElementById("bgMusic");
  const toggleBtn = document.getElementById("musicToggle");
  let isPlaying = false;
  toggleBtn.addEventListener("click", () => {
    if (isPlaying) {
      music.pause();
      toggleBtn.textContent = "🔇 Play Music";
    } else {
      music.play();
      toggleBtn.textContent = "🔊 Pause Music";
    }
    isPlaying = !isPlaying;
  });
</script>




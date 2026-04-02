# 🖥️ Interactive Terminal Portfolio

A highly dynamic, interactive, terminal-themed developer portfolio designed for zero-maintenance and easy updates. Built entirely with HTML, Tailwind CSS, and Vanilla JavaScript. 

![Portfolio Preview](https://via.placeholder.com/800x400/0b0e14/2b6cee?text=Terminal+Portfolio+Preview)

## ✨ Features

* **Zero Hardcoding:** 100% of the content (text, links, images, colors, and CV) is loaded dynamically from JSON files.
* **Realistic Terminal Engine:** Features a custom typewriter effect, CRT scanlines, blinking block cursor, and `Tab` autocomplete.
* **Interactive Physics UI:** A draggable, swinging ID badge with a physical lanyard string.
* **Light / Dark Mode:** Fully responsive theme toggler for accessibility and recruiter preference.
* **Offline Ready CV Download:** The CV is embedded as a Base64 string, allowing instant PDF generation and download without external servers.
* **Self-Contained:** No external backend required. Hosted perfectly on **GitHub Pages**.

---

## 🚀 How to Set Up & Deploy

1. **Create a Repository:** Create a new repository on GitHub and upload all the project files (`index.html`, `data.json`, `photo.json`, `cv.json`).
2. **Enable GitHub Pages:**
   * Go to your repository **Settings**.
   * Navigate to the **Pages** section on the left sidebar.
   * Under "Source", select the `main` branch and click **Save**.
3. **Visit Your Site:** Your terminal portfolio is now live at `https://yourusername.github.io/your-repo-name/`.

---

## 📝 How to Update Your Portfolio

You never need to touch the `index.html` file. Whenever you learn a new skill, get a new job, or want to update your resume, simply edit the JSON files. You can even pass your resume to an LLM (like ChatGPT or Gemini) and ask it to update these files for you!

### 1. `data.json` (Main Content)
This file controls the theme color, terminal boot sequence, social media links, and all terminal commands (about, experience, skills, etc.).
* *Note: Leave a social URL empty (`""`) and the icon will automatically hide itself.*

### 2. `photo.json` (Profile Image)
Contains the Base64 string of your profile picture to ensure instant loading.
```json
{
  "photo_base64": "data:image/jpeg;base64, ... [YOUR_BASE64_STRING_HERE]"
}

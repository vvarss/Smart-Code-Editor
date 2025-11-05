# ◻️Smart-Code-Editor
## 📱Overview
A sleek, real-time HTML/CSS/JS code editor built with pure HTML, CSS, and JavaScript. Designed for beginners, students, and web dev enthusiasts who want a smooth in-browser coding experience.

## 🚀 Features
* Live Preview — See your code output instantly inside an iframe.
* Three-Panel Layout — Separate editors for HTML, CSS, and JavaScript.
* Minimal & Clean UI — Dark theme, clean layout, easy to use.
* FontAwesome Icons for a modern tool-like feel.
* No frameworks needed — Runs entirely on the browser.

## 🧠 How It Works
The editor listens for user typing events (onkeyup) and updates the iframe output dynamically:
* Inserts HTML into iframe.body
* Injects CSS using a <style> tag
* Executes JavaScript inside the iframe sandbox


This creates a safe, isolated environment where users can test HTML/CSS/JS without affecting the main site.

## 📜 Code Snippet (Core Logic)
```
function run(){
let htmlCode = document.getElementById("html-code").value;
let cssCode = document.getElementById("css-code").value;
let jsCode = document.getElementById("js-code").value;
let output = document.getElementById("output");


output.contentDocument.body.innerHTML =
htmlCode + "<style>" + cssCode + "</style>";


output.contentWindow.eval(jsCode);
}
```

## 🎨 UI Highlights
* Full‑screen editor
* Flexible layout using CSS flex
* Clean textarea panels
* Dark coding environment for comfort
* Polished labels with icons

## ✨Output


https://github.com/user-attachments/assets/23dad924-ee83-4ca1-87ab-8b0c6858755d



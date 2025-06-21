# Web Application Programming and Hacking (WAPH) - Project 1 Report

**Instructor:** Dr. Phu H. Phung  
**Student:** Akhila Mohanan  
**Email:** mohanana2@udayton.edu  

![Headshot](Akhila.jpg)

---

## Overview

This project involved building a professional profile website using HTML, CSS, Bootstrap, JavaScript, and GitHub Pages. The website includes personal information, resume, API integrations, JavaScript cookies, and interactive features. Through this assignment, I learned how to build and deploy a responsive web application and apply core web programming concepts such as DOM manipulation, event handling, and web API integration.

- ✅ **GitHub Pages Live URL**: [https://mohanana2.github.io](https://mohanana2.github.io)
- 📁 **GitHub Repository**: [GitHub Project Folder](https://github.com/mohanana2/mohanana2.github.io)

---

## Task 1: Professional Profile Webpage

- I created an `index.html` file using Bootstrap layout.
- Added personal details, a sidebar, headshot photo, and styled content using custom CSS.
- Included sections like About, Summary, Education, Skills, Experience, and Contact.

---

## Task 2: WAPH Course Page

- Created a new `waph.html` page linked from the homepage.
- Added course overview, goals, and learning outcomes using HTML and Bootstrap cards.

---

## Task 3: JokeAPI Integration

- Used JavaScript `fetch()` to pull random programming jokes from [JokeAPI](https://v2.jokeapi.dev/joke/Programming?type=single).
- Displayed the joke in a styled section that auto-updates every 60 seconds.

```javascript
fetch("https://v2.jokeapi.dev/joke/Programming?type=single")
  .then(response => response.json())
  .then(data => {
    document.getElementById("joke-text").innerText = data.joke;
  });

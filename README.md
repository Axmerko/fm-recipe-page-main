# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### Screenshot

![](design\desktop-design.jpg)

*(Note: Don't forget to add a screenshot of your finished design to the root folder and name it `screenshot.jpg`, or update this path!)*

### Links

- Solution URL: [Solution](https://github.com/Axmerko/fm-recipe-page-main)
- Live Site URL: [Live url](https://fm-recipe-page-main-axmerko.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow (via media queries)
- [Google Fonts](https://fonts.google.com/) - Outfit & Young Serif

### What I learned

Working on this project reinforced several core CSS concepts for me. I spent a lot of time perfecting the layout and fixing small syntax issues that were breaking my code formatter (Prettier). 

Here are some specific things I learned and applied:

**1. CSS Selectors and the Comma Trap:**
I realized that using a comma in CSS creates entirely independent rules. Initially, I tried to target `h1` and `h2` inside a specific container using `.photoAndTitle h1, h2`, but this inadvertently targeted *all* `h2` elements on the page. I learned to separate them properly or structure my typography globally.

```css
/* Global typography approach */
h1 {
  font-family: "Young Serif", serif;
  color: #312e2c;
}

h2 {
  font-family: "Young Serif", serif;
  color: #854632; 
}
```

**2. Styling List Markers:**
I learned how to target and style the default bullets and numbers in lists using the `::marker` pseudo-element without needing complex spans or custom images.

```css
.preparation li::marker {
  color: #7a284e; 
}

.ingredients li::marker, .instructions li::marker {
  color: #854632;
  font-weight: bold;
}
```

**3. Responsive Images within Padding:**
I learned how to make an image fully responsive within a padded card, ensuring it scales correctly without breaking its aspect ratio or overflowing the container.

```css
.photoAndTitle img {
  width: 100%;
  height: auto;
  border-radius: 12px;
  display: block;
}
```

### Continued development

Moving forward, I want to speed up my HTML/CSS workflow. While I appreciate learning how to execute a pixel-perfect design, I plan to dedicate more of my upcoming study time to Codecademy to focus on programming logic and JavaScript, moving beyond purely visual structuring. 

### AI Collaboration

- **Tool used:** Google's AI Assistant (Gemini)
- **How I used it:** - **Debugging:** I used the AI to help me parse Prettier error logs. It quickly pointed out unclosed HTML tags (like a missing `rel` attribute in a `<link>` tag) and stray characters (like an accidental `/` in my CSS) that were preventing my code from formatting.
  - **Concept Explanation:** The AI helped explain CSS inheritance, specifically how to load two different Google Fonts and apply them cleanly to headings versus body text.
  - **Code Generation:** When I got bogged down by CSS styling and wanted to move on to my coding courses, I collaborated with the AI to generate the final layout and spacing adjustments based on my existing HTML structure.
- **What worked well:** The AI was excellent at spotting tiny syntax errors that are easy to miss with the human eye and explaining *why* certain CSS rules weren't behaving as expected.

## Author

-Miroslav Adrian Axmann
- GitHub - [@Axmerko](https://github.com/Axmerko)
- Frontend Mentor - [@Axmerko](https://www.frontendmentor.io/profile/Axmerko)
# Assignment #1 – HTML & CSS Basics

**Name:** Meiyrkhan Abilda
**Group:** IT-2503
**Course:** Web Technologies (Front-End Development)

## About this repo

This is my first webpage assignment for the Web Technologies course. The task was to build a simple personal webpage step by step, starting from basic HTML tags and ending with CSS layout stuff like positioning, sizing units, and floats. Everything is in `index.html` and `styles.css`.

Live version:<img width="1470" height="690" alt="full page" src="https://github.com/user-attachments/assets/908e27a2-6347-41b5-9489-0a3e2aa4e6eb" />


## Part 1 – Introduction to HTML

**Step 0-1. Boilerplate + text structure**
Basic HTML skeleton with `<!DOCTYPE html>`, `<head>`, `<title>` set to "My First Webpage". Added `<h1>`-`<h3>` for my name, group, and "About Me", plus a short paragraph about myself.
<img width="916" height="192" alt="header" src="https://github.com/user-attachments/assets/bf783501-e6fc-4506-adc4-1fe1940e63c4" />


**Step 2. Lists**
Ordered list `<ol>` for my hobbies, unordered list `<ul>` for my favorite websites.
<img width="233" height="96" alt="hobbies" src="https://github.com/user-attachments/assets/6b273314-67bb-4892-8106-5658ce0f1b7d" />

**Step 3. Images and links**
Added my profile picture with `<img>` and three links with `<a>` (YouTube, Codeforces, Telegram).
<img width="96" height="95" alt="links" src="https://github.com/user-attachments/assets/89510917-cf41-492f-a303-b07c0be342ae" />


**Step 4. Button**
Just a plain "Click Me" button, no JS functionality yet.
<img width="96" height="95" alt="links" src="https://github.com/user-attachments/assets/868fc1f0-92f9-46d9-8b4b-dda52331151c" />


## Part 2 – Intermediate HTML

**Step 5. Table**
Weekly class schedule table with Subject / Day / Time columns.
<img width="1465" height="206" alt="table" src="https://github.com/user-attachments/assets/7833428b-5937-4c0c-8922-fa8ff7c3cb63" />


**Step 7. Emojis**
Added a mood paragraph with 3 emojis (`#idname`).
<img width="1445" height="97" alt="emojis" src="https://github.com/user-attachments/assets/5cc4d17b-7455-4454-a343-be4c4423c07b" />


**Step 8. Form**
Form with first name, last name, email, favorite color (color picker) and a submit button.
<img width="679" height="93" alt="form" src="https://github.com/user-attachments/assets/cb3ac61f-fce3-444e-a8f9-9debf3662913" />


## Part 3 – Introduction to CSS

**Step 9-13. Inline / Internal / External CSS + selectors**
- Internal CSS in the `<style>` tag inside `<head>` (body background).
- External stylesheet `styles.css` linked with `<link rel="stylesheet">`.
- Used an element selector (`p`), a class selector (`.highlight`), and an ID selector (`#idname`, `#main-heading`) to show the difference between them.

**Step 14. Classes vs IDs**
`.highlight` class is used on the table row for my WEB Technologies class. `#main-heading` styles my `<h1>` with a custom color, margin and padding.

## Part 4 – Intermediate CSS

**Step 15. Favicon**
Linked a favicon with `<link rel="icon" href="iconweb.png">`.

**Step 16. Divs**
Wrapped the intro section in `.header`, used more divs for layout later on.

**Step 18. Positioning**
Three boxes to show the difference between position types:
- `.static-box` – normal flow, holds my schedule table
- `.relative-box` – shifted slightly with `top`/`left`, holds my mood paragraph
- `.absolute-box` – positioned absolutely inside `.position-container`, holds the form
<img width="1461" height="444" alt="boxes" src="https://github.com/user-attachments/assets/b95e8bb6-2764-4dea-8a67-e90e18062396" />


**Step 19. Sizing units**
`#main-heading` uses `rem`, `h2`/`h3` use `rem`/`em`, and the profile image width is set in `%` with a `px` max-width so it doesn't get too big.

**Step 20. Float and clear**
`.left-box` and `.right-box` floated left/right inside `.float-container`, with `.clear-fix` (`clear: both`) after them so the layout doesn't break.
<img width="1470" height="153" alt="float2" src="https://github.com/user-attachments/assets/d802a767-c726-43f5-9c4e-96927a84dbd5" />


**Step 21. Publish**
Published using GitHub Pages, link is at the top of this file.

## Work process / summary

Honestly the hardest part for me was CSS positioning — I kept mixing up `relative` and `absolute` and couldn't figure out why my absolute box was jumping to a weird spot until I understood that it positions itself relative to the nearest ancestor that has `position: relative` (in my case `.position-container`). Once that clicked it made a lot more sense.

The float/clear part was also a bit confusing at first because without the `clear-fix` div, everything below the floated boxes was overlapping. Adding `clear: both` fixed it right away.

Everything else (lists, table, form, links) was pretty straightforward, just took some time to get the styling to look decent instead of default browser ugly.

## Resources used
- Abitova G.A., Web Technologies Front-End Development, Part 1 (2022)
- https://www.w3schools.com/html/html_basic.asp
- https://www.w3schools.com/css/css_syntax.asp

# Raymond Wong Portfolio

This is my personal portfolio website for Assignment 1. It is a four-page website built with HTML5 and CSS3. It introduces who I am, shows my future projects, and lets visitors contact me.

## Links
- GitHub: (https://github.com/Raymond9x22/INFR3120_Asm_1)

## Pages

The website has four separate HTML pages. Every page has the same navigation (Home, About me, Projects, Contact me) and the same footer with my contact email and copyright.

| File | Page | What is on the page |
|---|---|---|
| index.html | Home | My avatar, my name, a short introduction, and four large buttons that link to every page |
| about.html | About me | My photo, a "Hello!" paragraph about myself, some facts about me, and a video introduction.|
| projects.html | Projects | My upcoming project will post here.|
| contact.html | Contact me | A contact form with name, email, phone number, comments, an "I am not a robot" checkbox, and Send message / Clear form buttons |

### Semantic tags

I used semantic tags to describe each part of the page:

- header – avatar, name and navigation at the top of every page
- nav – the navigation menu
- main – the main content of each page
- article – the main content block on About, Projects and Contact
- section – each project box, and the "about" and "video" parts of the About page
- figure – my photo on the About page
- address – my contact email in the footer
- footer – email and copyright at the bottom of every page

## Folder structure

- index.html, about.html, projects.html, contact.html – the four pages
- css/style.css – shared styles for every screen size (colours, fonts, gradients, footer, form)
- css/laptop.css – layout for laptops and desktops
- css/tablet.css – layout for tablets
- css/phone.css – layout for phones
- images/ – my avatar, my photo, and the video poster
- video/ – my video introduction
- README.md – this file

## Responsive design

My website uses **fluid design** and **media queries**.

Every page has the viewport meta tag, so phones and tablets report their real screen width instead of pretending to be a desktop. Every page loads style.css on all screens.

| Viewport | Screen width | CSS file | Why I chose this size |
|---|---|---|---|
| Phone | 480px and below | phone.css | Most phones are about 360px to 430px wide. |
| Tablet | 481px to 960px | tablet.css | Most tablets are about 768px to 834px wide. |
| Laptop | 961px and above | laptop.css | Laptops are usually 1280px wide or more. The page is a 960px box in the centre (the 960 grid from Week 1), with the photo and text side by side and two project boxes per row. |

I also made the footer always stay at the bottom of the window. So it doesn't have empty space under the footer.

## Gradients

| Gradient | Where I used it | File and selector |
|---|---|---|
| Linear gradient (top to bottom) | The whole page background fades from white at the top to light grey at the bottom, on all four pages | style.css, #wrapper |
| Linear gradient (left to right) | The footer fades from dark slate to soft blue, on all four pages | style.css, footer |
| Angled linear gradient (45 degrees) | The contact form box on the Contact me page | style.css, .form-box |

## Colour scheme

![My colour scheme]

| Colour | Hex code | Where I used it |
|---|---|---|
| Dark slate | #2B2D42 | Text, headings, the footer |
| Soft blue | #4A6FA5 | Links, borders, buttons, the avatar border |
| Grey blue | #8D99AE | Lines under the header, form field borders, photo border |
| Light grey | #EDF2F4 | Page background and the bottom of the fade |
| Warm orange | #F2A541 | Hover colour for links and buttons |

I chose blues and greys because I wanted my portfolio to look clean and simple. I used one warm colour (orange) for hover effects, so it is easy to see which link or button the mouse is on.

## Contact form validation

- **Name** – required.
- **Email** – required. It uses the email input type, so the user have to input vaild email address.
- **Cell number** – required. It uses the tel input type with a pattern that needs exactly 10 digits.
- **Comments** – required.
- **"I am not a robot" checkbox** – must be ticked before the form can be sent.

When the visitor clicks **Send message**, the form uses a mailto action. This redirect to the visitor's email app and send the emial. **Clear form** empties all the fields.

The email link in the footer also uses mailto, so clicking it opens a new email to me.

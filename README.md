# Project 0

**Web Programming with Python and JavaScript**

#### DIY Home Server is a website, built just with HTML, Bootstrap and Sass/Css.
##### It contains 4 Html pages with informations about building of openSSH server for storing files.

## 1. index.html
  It is used for "home page".
  Header: defines name of website, bootstrap link and stylesheet link (to
  index.css file)
  Body: Content is wrapped in bootstrap container class.
  For headings are used bootstrap flex classes.
  There are two headings: one (h1) for defining website title and second (h2)
  for explaining its content.
  Three buttons which are styled with bootstrap/Layout/Grid classes. Each button
  has a specific link to open specific page of website (hardware.html, software.html, procedure.html)

### 1.1 index.css
    Set whole body background-color to light gray (#c9c9c9).
    Id to move main title (h1) lower from the top.
    Add more space on top and bottom of h3.
    "@media" to hide content of h3 on smaller screens (< 575px)

## 2. hardware.html
  Represents some of the hardware components I used for building server.
  Header: page title, bootstrap and css link (to styles/hardware.css).
  Body:
    Navigation bar - It is built with Bootstrap/Components/Navbar, with small changes to fit my needs. First component is "home button" whit link to index.html. It is always on page, even on smaller screens where other buttons collapse into "sandwich button". Each of the button (Hardware, Software, Procedure) has a specific link to open specific page on website.
    Content - four images, showing hardware components and short description of each image. For their position on page are used classes from bootstrap/Layout/Grid templates.
    At the end of the body, last three script tags are from bootstrap page, to make bootstrap components dynamic (navigation bar collapsing into sandwich)

### 2.1 hardware.scss
    color-body variable is set to light gray (#c9c9c9) and is used for defining body background.
    Positioning whole section of pictures 25px below navigation bar.
    Custom class ".center-img" puts the content/description of each image in the center of the image.
    With "@media" making the text on images bigger on bigger screens (> 992 px).

## 3. software.html
  Shows the table of softwares and short information of which version to pick.
  Header: page title, bootstrap and css link (to styles/software.css).
  Body:
  Navigation bar - it is the same for all three pages (hardware, software and
  procedure) - for more information, check 2. hardware.html-Body-Navigation bar.
  Content - one table with two columns and 6 rows, first of that 6 rows are table header tag (<th>), others are <td>. For this content bootstrap is not used, just plain html tags.
  At the end of the body, last three script tags are copied from bootstrap page, to make bootstrap components dynamic (navigation bar collapsing into sandwich).

### 3.1 software.scss
    Here is the example of using Nesting in sass.
    Table is nested into body and th, td are nested into table.
    Background color of table is white, border - 2px solid black, inner lines are 1px solid black, text color of header (Software and info) is dark blue (#2754db), text color of software names are green (#2a7507), text of "Info" column is italicized, black. Table is centered horizontally.

## 4. procedure.html
  Contains the step by step procedure of how server was set up.
  Header: page title, bootstrap and css link (to styles/procedure.css).
  Body:
  Navigation bar - it is the same for all three pages (hardware, software and
  procedure) - for more information, check 2. hardware.html-Body-Navigation bar.
  Content - Main header, describing content of page. Then two unordered lists containing steps of setting up server and two paragraphs used for comment on set up. Then two sections explaining how to use previous set ups.
  For better visual separating code from the text, class "command" is used.
  At the end of the body, last three script tags are copied from bootstrap page, to make bootstrap components dynamic (navigation bar collapsing into sandwich).

### 4.1 procedure.scss
    Here is the example of using inheritance.
    In %instruct-text is a set of css properties used for each instruction text on this page (letter-spacing: 1px; font-style: normal;).
    For visually separating code and other text in ul there are some additional styling for "ul" and ".command".

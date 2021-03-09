# Clone Instagram -- With SASS

## 🔮 Overview 🔮
Sass (which stands for 'Syntactically awesome style sheets) is an extension of CSS that enables you to use things like variables, nested rules, inline imports and more. It also helps to keep things organised and allows you to create style sheets faster.

This project is done to put the basic foundations of SASS into practice.

<br></br>

## 💡 Main objetives of this project 💡

●	Learn the basics of SASS
●   Improve your HTML skills
●   Learn how to work with HTML and SASS
●   Improve your frontend knowledge
●   Improve your SASS knowledgeUnderstand what it is an architecture pattern, what it is used for, and what advantages it can bring to the project
<br></br>

## 💡 Investigation phase 💡

Before starting the practice, it is necessary to understand the conceptual part of SASS and its different functionalities. To do this, we are going to search information to answer some question about SASS.
The question's answers are in the theory document ![Theory](THEORY.md)

<br></br>

## 💡 Project requirement 💡

Create a small HTML website in which SASS styles will be applied.
All the content that you must show in the view must be static.
This website will consist of an Instagram clone with two HTML pages:
●	Login page
    ○	Two content area
        ■	Instagram photos
        ■	Login form
    ○	Footer
●	Home page
    ○	Navbar
    ○	Posts

<br></br>

## 💡 Project developed description 💡
To develop the project you must take into account the following guidelines:
1. The login page will be made up of the following sections:
    ●	Left content
        ○	There will be the instagram previews located on the left of the page
    ●	Right content
        ○	Here there will be a login form identical to instagram.
    ●	Footer
        ○	Here there will be a login form identical to instagram.
    The structure of this page will be as follows:
    [Login page structure](/assets/img/LoginStructurePage.png)

2. The home page will be made up of the following sections
    ●	Navbar must contain:
        ○	Instagram logo
        ○	Search engine
        ○	Three icons:
            ■	Home icon
            ■	New post icon
            ■	Profile icon

    ●	Posts
        ○	Photo and name of who posted
        ○	Image
        ○	Two icons:
            ■	Heart icon
            ■	Comment icon
        ○	Number of likes
        ○	Comments:
            ■	Name of who commented
            ■	The comment
        ○	Publication datej
<br></br>

### ⚙️ Project architecture ⚙️
It has been used the architecture known as the 7–1 pattern. It is a widely-adopted structure that serves as a basis for large projects. It consists in have all your partials organised into 7 different folders, and a single file sits at the root level (usually named main.scss) to handle the imports — which is the file you compile into CSS.

For example: 

sass/
|
|– abstracts/ (or utilities/)
|   |– _variables.scss    // Sass Variables
|   |– _functions.scss    // Sass Functions
|   |– _mixins.scss       // Sass Mixins
|
|– base/
|   |– _reset.scss        // Reset/normalize
|   |– _typography.scss   // Typography rules
|
|– components/ (or modules/)
|   |– _buttons.scss      // Buttons
|   |– _carousel.scss     // Carousel
|   |– _slider.scss       // Slider
|
|– layout/
|   |– _navigation.scss   // Navigation
|   |– _grid.scss         // Grid system
|   |– _header.scss       // Header
|   |– _footer.scss       // Footer
|   |– _sidebar.scss      // Sidebar
|   |– _forms.scss        // Forms
|
|– pages/
|   |– _home.scss         // Home specific styles
|   |– _about.scss        // About specific styles
|   |– _contact.scss      // Contact specific styles
|
|– themes/
|   |– _theme.scss        // Default theme
|   |– _admin.scss        // Admin theme
|
|– vendors/
|   |– _bootstrap.scss    // Bootstrap
|   |– _jquery-ui.scss    // jQuery UI
|
`– main.scss              // Main Sass file

## ⚓ Wireframe ⚓
    [Login page](/assets/img/LoginWireframe.png)
    [Home page](/assets/img/HomeWireframe.png)

## ⚙️ Requirements ⚙️

●	You must use variables at least once in the project.
●	You must use nesting.
●	You must use inheritance at least once in the project.
●	You cannot use third party libraries for the development of this pill
●	You must take screenshots of the main browsers to ensure that the content is displayed correctly
●	Both the code and the comments must be written in English
●	The code of the different programming languages that you will use should be stored in a different file with the appropriate extension (html => file.html, sass => main.scss). You should not mix html and CSS code in the same file


<br></br>


## ⏳ Work estimates ⏳

This project estimation delivery is for 3 work days. Including all the documentation and learning phase.

<br></br>
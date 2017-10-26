![CF](https://camo.githubusercontent.com/70edab54bba80edb7493cad3135e9606781cbb6b/687474703a2f2f692e696d6775722e636f6d2f377635415363382e706e67) Lab 03: jQuery Events
===

## Submission Instructions
Follow the submission instructions from Lab 01.

## Resources  
[jQuery cheatsheet](https://oscarotero.com/jquery/)

[Template Literals MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

## Configuration
_Your repository must include:_

```
03-jquery-with-events
├── .eslintrc.json
├── .gitignore
├── LICENSE
├── README.md
├── index.html
├── scripts
│   ├── article.js
│   ├── articleView.js
│   └── blogArticles.js
├── styles
│   ├── base.css
│   ├── fonts
│   │   ├── icomoon.eot
│   │   ├── icomoon.svg
│   │   ├── icomoon.ttf
│   │   └── icomoon.woff
│   ├── icons.css
│   ├── layout.css
│   └── modules.css
└── vendor
    └── styles
        └── normalize.css
```

## User Stories and Feature Tasks

- Continue styling the app using SMACSS practices. Take a few minutes for code review of your partner's CSS and decide how to incorporate it into your paired lab. You can choose one partner's CSS structure, or you can combine them as you see fit. Seek to optimize and organize your CSS as much as possible!

*As a user, I want to be able to filter my articles so that I can selectively view articles by author or by category.*

- Complete the new requirements for setting `data-<attributes>` in your `toHtml()` method.
- Complete the methods for handling filter events when selecting an option from a drop down menu via Authors and Categories so that only the selected articles are displayed on the screen.

*As a user, I want to be able to preview each article so that I can easily view the results and select the one I want to read further.*

- Add an event to reveal a complete article if the user would like to see more of it beyond the teaser.

*As a user, I want tab-based navigation so that I can easily visit other sections of my site.*

- Complete the method `articleView.handleMainNav()` for implementing tab-based event navigation on the page.

*As a developer, I want my code to be thoughtfully organized, easy to read, and executing efficiently.*

- Review and understand the new JS file, `articleView.js`
- Add any new script tags to your HTML.
- Refactor concatenation using template literals.
- Render the app upon page load.

### Stretch Goal

*As a user, I want to be able to collapse an expanded article to the teaser view so that I can more easily scan over a series of articles.*

- Build in functionality such that a user can click on "Show Less" to collapse a full article into a teaser.

## Documentation
_Your README.md must include:_

```md
# Code Fellows 301 Day 3 -- jQuery Events

**Author**: Will Reid & Matt Iwicki
**Version**: 1.0.2

## Overview
Our goal with this project was to build on a mobile-first site, using jQuery to dynamically render blog posts sorted by most recent publication date and allow dynamic filtering in response to user preference for particular authors or categories.  We also enabled teaser functions to allow the user to view more articles in a glance and expand articles of interest, and we enabled tabbing between articles and the About Me section without a page reload.

## Getting Started
To build this app on your own machine, clone this repo and launch the html page in your browser.

## Architecture
We are using a SMACSS organization of our CSS. We are using some light CSS animations to display and hide the menu, and we are using link tags to call the CSS in.  The index.html file reveals the basic template for each article; the blogArticles.js holds all the text content; the article.js file constructs each article and makes the posting available to the DOM; and the articleView.js file allows the user to interact with the elements on-screen.

## Change Log
10-26-2017 10:00am -- enabled
10-26-2017 12:30pm -- enabled article filter logic
10-26-2017 1:00pm -- enabled teaser hide/show logic

## Credits and Collaborations
Created by Will Reid and Matt Iwicki, based off of source code from the Code Fellows 301 lab repo. We used the clearfix CSS convention from CSS Tricks: https://css-tricks.com/snippets/css/clear-fix/, the normalize.css from github.com/miwicki/normalize.css and the jQuery v3.2.1 library.  Matt LeBlanc helped build the CSS on the previous day's assignment. Ron Dunphy and Dustin Byers assisted in troubleshooting filter performance, and Ariel and Nicholas C provided insight on teaser functionality.

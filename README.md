# Horiseon Social Solution Services - Code Refactor Assignment

![alt text](assets/images/screenshot.png)

> <h2 align="center"><a  href="https://kevin-aminzadeh.github.io/01-bootcamp-code-refactor/">Live Demo</a></h2>

## Table of Contents

- [Introduction](#introduction)
- [Overview](#overview)
- [Approach](#approach)
- [License](#license)

## Introduction

This project is an exercise in refactoring a pre-exisiting codebase in order to address given requirements or feature requests.

The focus of this particular code refactor exercise is addressing accessibility concerns through the use of semantic HTML elements and attributes; while also reenforcing basic Git and CSS concepts.

## Overview

Horiseon Social Solution Services, a fictional digital marketing agency, have presented the existing codebase for their website and requested that the code be refactored due to accessibility and technical SEO concerns with the current implementation.

## Approach

To achieve the project's accessiblity and SEO goals, the following changes were made to the exisiting codebase:

### **Semantic HTML**

Initially, the existing HTML structure of the page was analysed revealing a lack of semantic HTML tags to describe the page's information architecture for screenreaders and web crawlers. This issue was addressed by seperating logical sections of the page using semantic HTML tags such as `<section>`, `<nav> `, `<aside>` etc.

As part of this process, comments were added to clearly denote each logical section of the page, the title of the page was updated to reflect its content, and a number of meta tags were also added.

### **Image Alt Attributes**

Image alt attributes are an important consideration both in terms of accessibility and SEO. Alt attributes or alt text are used to describe the contents/function of images on a page.

Generally speaking, alt text should always be provided for images in order to provide context to assitive technologies and webcrawlers, thereby imporving page accessibility and SEO.

In the case of decorative images ( i.e. images which don't add any additional information to the contents of a web page and/or are used decoratively ) however, best practice guidelines provided by [W3C](https://www.w3.org/WAI/tutorials/images/decorative/) recommend the use of null alt text so that such images can be ignored by assistive technologies and crawlers.

In the context of this particular project, the author strongly believes that all images used on the page are purely decorative and do not provide any additional information to its content.

As such, the alt attributes added to the images in each section were intentionally given a value of null ( `alt=""` ); as opposed to a descriptive alt text in the case of images which add information to the content of the page.

### **CSS Reusability & Maintainability**

To improve the reusability and maintainability of the project's CSS the following changes were made:

- the existing CSS codebase was reorganized to follow the semantic structure of the page's HTML elements.
- Comments were added to seperate the various sections and make the CSS easier to read and traverse.
- The existing styling rules and classes were updated with the aim of reducing duplication and encouraging modularity/reusability of components.

## License

This project is licensed under the terms of the MIT license.

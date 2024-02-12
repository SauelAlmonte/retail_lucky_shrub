# Coursera Project

## Retail: Lucky Shrub

## Webpage Overview

### Enhancing Accessibility through HTML Structure, Attributes, and Meta Tags

### HTML Meta Tags

#### Open Graph (OG) Meta Tags for Social Media Sharing

The HTML head section undergoes meticulous organization to optimize the presentation, accessibility, and discoverability of the webpage.

##### Open Graph (OG) Meta Tags for Social Media Sharing

- **og:title**: Specifies a captivating title for social media sharing.
- **og:description**: Succinctly describes content for social media previews.
- **og:type**: Indicates content type, set as a website.
- **og:url**: Defines content URL for accurate linking.
- **og:image**: Specifies an associated image, enhancing visual appeal.
- **og:site_name**: Ensures consistent branding in social media shares.
- **og:locale**: Tailors content presentation for specific languages.
- **article:author**: Attributes content to a specific author.
- **article:published_time**: Provides the article's published timestamp.

##### Metadata for Character Set, Language, Description, Subject, Copyright, Date, Keywords, and Viewport

- **charset**: Sets character encoding to UTF-8.
- **language**: Specifies content language as Spanish (ES).
- **description**: Offers a concise content overview.
- **subject**: Specifies primary subject or theme.
- **copyright**: Defines ownership and usage rights.
- **date**: Specifies content date for context.
- **news_keywords**: Provides keywords for news-related searches.
- **viewport**: Defines settings for responsive web design.

##### Favicon and Stylesheet Links

- **shortcut icon**: Specifies website favicon using an ICO image.
- **stylesheet**: Links to external CSS files, including "reset.css" and "styles.css" for consistent styling.

##### Title of the Document

- **title**: Sets HTML document title, influencing browser tabs and search engine results.

Collectively, this meticulous setup optimizes the webpage's appearance on social media, improves search engine visibility, ensures consistent branding, and enhances user experience.

### HTML Structure and Attributes for Accessibility

The HTML structure and attributes within the `<body>` of this webpage are meticulously designed with accessibility in mind, ensuring an inclusive user experience. Here's how:

#### Header Section

The main header (`<header>`) incorporates semantic elements like `<h1>` and `<nav>` with appropriate roles and ARIA attributes. Navigation links are organized using an unordered list (`<ul>`) to facilitate screen reader navigation.

#### Hero Section

The hero section (`<main>`) utilizes semantic HTML and an `aria-labelledby` attribute to associate the content with an accessible label. This ensures screen readers convey meaningful information about the hero section.

#### Second Header Section

The second header (`<header>`) replicates key accessibility features from the main header, including ARIA attributes, semantic elements, and accessible links for navigation.

#### Section 1: History

The history section (`<section>`) is structured with semantic elements and ARIA attributes. Headings and paragraphs include appropriate labeling and numbering for screen reader users.

#### Carousel Section

The carousel (`<div>`) is crafted with navigational elements (`<div id="prev">` and `<div id="next">`) and pagination, enhancing accessibility for keyboard users and providing meaningful labels for screen reader users.

#### Section 2: Climb

The climb section (`<section>`) employs semantic HTML elements and ARIA attributes, featuring an accessible heading (`<h2>`), a numbered paragraph, and descriptive content.

#### Section 3: Schedule

The schedule section (`<section>`) showcases semantic HTML, ARIA attributes, and a well-organized list of dates and corresponding activities. Tabs for Mountain 1 and Mountain 2 are accessible and clearly labeled.

#### Footer Section

The footer (`<footer>`) integrates a logo with an accessible link, copyright information, and semantic HTML elements. The copyright information dynamically updates with the current year for accuracy.

#### Scripts

The inclusion of a script (`<script>`) with a `defer` attribute ensures that the JavaScript file is executed after the HTML content is parsed, contributing to a smoother user experience.

By adhering to proper HTML structure, utilizing semantic elements, and incorporating ARIA attributes, this webpage aims to provide an accessible and inclusive experience for all users, including those with disabilities who rely on assistive technologies.

## CSS Media Queries

#### The Impact of CSS Styles on Webpage Design

##### Font Import

The Font Import section is pivotal for enhancing the visual appeal of the webpage by importing specific fonts from Google Fonts. Choosing appropriate fonts can significantly contribute to a better user experience and aesthetic presentation, making the content more readable and engaging.

##### Global Styles

Global Styles play a pivotal role in maintaining consistency and coherence throughout the entire webpage. By establishing default font families, defining a minimum height for the body, specifying a background color, and adjusting font sizes, these styles create a unified visual identity. Consistency is paramount for a professional and polished look, ultimately improving overall user satisfaction.

##### Media Queries

In the era of diverse devices, Media Queries become indispensable for responsive design. The inclusion of media queries ensures that the webpage adapts seamlessly to various screen sizes. This optimization enhances the user experience across a multitude of devices by providing styles tailored to multiple screen sizes. Specific adjustments for headers, logos, and navigation links cater to the unique needs of today's user, contributing to a friendly and accessible design.

## JavaScript Functions for Webpage Interaction

### Selection of DOM Elements

In this section, DOM elements for carousel, pagination, and buttons are selected using various methods, such as `document.querySelector` and `document.getElementById`. Each variable (`carouselInner`, `pagination`, `prevButton`, `nextButton`, and `currentYearElement`) represents a key element on the webpage.

### Tracking Current Index and Total Images

The code initializes two variables - `currentIndex` and `totalImages`. `currentIndex` keeps track of the current index of the displayed image in the carousel, while `totalImages` is calculated based on the screen width using the `calculateTotalImages` function.

### Calculate Total Images Function

The `calculateTotalImages` function dynamically determines the total number of images to be displayed based on the screen width. It returns 2 for larger screens and 8 for smaller screens.

### Update Pagination Function

The `updatePagination` function dynamically modifies the pagination based on the current index and total images. It clears existing pagination elements, creates new elements, and adds event listeners for intuitive navigation. It also highlights the active pagination element.

### Event Listeners for Navigation

Event listeners are attached to the previous and next buttons, allowing users to navigate through the content. These listeners trigger the `updateCarousel` and `updatePagination` functions, updating both the carousel display and pagination.

### Update Carousel Function

The `updateCarousel` function adjusts the position of the carousel based on the current index. It calculates the translation value and applies it to the `carouselInner` element, creating a smooth sliding effect.

### Update Current Year Function

The `updateCurrentYear` function retrieves the current year and updates the content of `currentYearElement` in the footer.

### Event Listener for Window Resize

An event listener is set for window resize, triggering the recalculation of `totalImages` and updating the pagination display accordingly.

### Initial Setup

The `updatePagination` function is initially called upon page load to set up the pagination. Additionally, the `updateCurrentYear` function is called to dynamically display the current year.

The webpage seamlessly integrates HTML structure, CSS styling, and JavaScript functionality to deliver a visually appealing, accessible, and responsive user experience.

# Structure Web Pages with HTML
## Process and Design
### Who is the site for?
Sites should be designed for a target audience, and as such it is important to understand your target audience and what they would like.  
Try asking people who you know would be interested in the site what they want to see.  
Not everyone is going to have interest in the site, so even if it has a wide appeal, work towards the target demographic the most.
#### Target Individuals
* How old are they?
* Are you more appealing to women or men?
* Which country are they from?
* Do they live in urban or rural areas?
* etc
#### Target Companies
* What is the size of the company or relevant department?
* What is the position of the people within the company?
* How large is the budget they control?
* etc

Invent fictional visitors from your target audience and use the idea of them to help influence design choices.
### Why People Visit Your Website
To help determine the reason people are visiting, there are two basic types of questions,
1. What are their underlying motives for their visit?
2. What are the visitors' goals?  
#### Key Motivations
* Are they looking for something general or specific?
* If specific is it personal or professional?
* Is spending time on this a necessity or a luxury?
#### Specific Goals
* Do they want general or specific information?
* Are they already familiar with your product or does it need to be introduced?
* Is their request time sensitive?
* Does it have to do with whether or not they decide to purchase something?
* Do they need to contact you? And if so how?
### What Your Visitors are Trying to Achieve
Create a list of reasons people might want to come to your site and try assigning them to your fictional visitors.  
It is difficult to think of every reason, but come up with the main ones you believe in.  
### What Info Your Visitors Need
Figure out what info they are there for, then offer additional info you believe they may want or need.  
Go back through the reasons people may visit the site and think about what all of them need to achieve that.  
Prioritize information based on how essential it seems.  
Your site will seem more relevant to visitors if the info they need is readily available.  
### How Often Will People Visit Your Site
Determine whether the content of your site would benefit from being updated more regularly.  
If people are regularly at the site, or if the information therein changes over time, work out how often it should be updated to ensure people return.
### Site Maps
Orgainze the information you have into sections or pages to create a diagram of the site's structure.  
Try to group like subjects together. If you ask people from the target audience, it can be more helpful in organizing the site in a good way.  
Some info may need to be duplicated for different pages if it is a part of multiple subjects.
### Wireframes
A wireframe is a sketch of the key info required on each page of a site.
### Getting Your Message Across Using Design
Organizing and prioritizing info helps users understand their signifigance and what order to go through them in.  
Make parts of the page look distinct so they will stand out and be easier to understand.  
Grouping related content into chunks simplifies the design and makes it more accessible to users. Using a similar visual style among the same types of content will make the user associate the two and make them easier to understand.  
Use Visual Hierarchy to draw attention to the main point of something. If it's relevant to the user, they will look closer to see the rest of the info on it. Size, color, and style are the three main points of difference in establishing a visual hierarchy, which is the order in which your eyes percieve things. Images are also very useful for this.
### Grouping and Similarity
Ways of organizing elements of a page to show relation.
* Proximity
    * When several items are placed close together
* Closure
    * A real or imaginary box can be formed around elements due to proximity or allignment
* Continuance
    * When elements are place in a line or a curve
* White Space
    * Placing relative items closer together and leaving a bigger gap between unrelated items
* Color
    * A background color placed behind related items
* Borders
    * A line can be drawn around the border of the group or between it and its neighbors
* Repetition
    * Items of similar size, color, font, orientation, or shape suggests matching elements have similar importance or meaning.  
* Consistancy
    * Using a consistant style suggests other items of the same structure type will have similar info
* Headings
    * Giving a chunk of info a heading tells the user immediately whether or not it relates to them
### Designing Navigation
Good navigation tends to follow three principles
* Concise
    * Should be quick and easy to read with a limited number of options
* Clear
    * Users should be able to predict what they will find before clicking the link
* Selective
    * Primary navigation should only reflect content, not things like login, search, or legal info
Good sites often have primary and secondary modes of navigation, for bigger sections and their subcategories.  
Some other good things to consider
* Context
    * Good navigation tells the user where they are on the site
* Interactive
    * Each link should be big enough to click on and should change when interacted with by the user
* Consistent
    * It is best to keep primary navigation the same across the site, even if secondary navigation changes from page to page.

## Structure
The use of headings and subheadings is important in structuring word documents.  
HTML uses elements to describe the structure of pages, using tags like containers for the different pieces.  
Attributes tell us more about specific elements and are made up of a name and a value separated by an equals sign.  
`<body>` contains things shown in the browser  
`<head>` contains info about the page  
`<title>` is shown at the top of the browser on the tab for the page  
HTML stands for hypertext markup language, which is named as such because it allows users to create hyperlinks to external or internal sources.  
Coding in a content management system usually means you will not be able to edit things like the HTML of a page, just the contents of specific areas of the page itself.  
To look at how other sites are built, you can view their source code.
## HTML5 Layout
### Traditional HTML Layouts
Many web page authors used to only use `<div>` to group elements together, and would add a class or id attribute to identify them.
### New HTML5 Layout Elements
HTML5 introduces new element that indicate the type of content that can be found in them.
### Headers and Footers
The `<header>` and `<footer>` elements can be used for the main header and footer at the top and bottom of the page, or for ones on individual articles.
### Navigation
The `<nav>` element contains the major navigational blocks on the site.
### Articles
The `<article>` element contains any section of a page that can stand alone. They can also be nested inside of each other.
### Asides
The `<aside>` element, when inside of an article, should retain information related to, but not essential in its overall meaning.  
When not within an article, it contains content related to the page as a whole.
### Sections
The `<section>` element groups related content together; it can contain multiple articles, or it can be used to break up a long article.
### Heading Groups
The `<hgroup>` element groups together `<h1>` through `<h6>` headings to treat them as one heading.
### Figures
The `<figure>` element can contain anything referenced from the main flow of an article. It should only be used when the content references only the element, and isn't integral to the page. It should also inclue a `<figcaption>` element, which decribes the content of the figure.
### Sectioning Elements
The `<div>` element can be used to group together related elements.
### Linking Around Block-Level Elements
Placing an `<a>` element around an block containing child elements allows you to turn the entire block into a link.
### Helping Older Browsers Understand
Older browsers have trouble reading HTML5, and will treat new elements as inline elements, so to fix this, you should include `header. section. footer. aside. nav. article. figure {display: block;}` as code in your CSS file.  
To style these elements for earlier versions of Internet Explorer, you neeed to use HTML5 shiv or HTML5 shim.
## Extra Markup
### The Evolution of HTML
Each new version of HTML has been designed to improve on its predecessor, however, some older browsers cannot process elements of the newer versions.
* HTML 4
    * With a few exceptions, many of the things that have been covered by HTML5 were in HTML 4. Although it had some presentational elements, it is no longer recommended.
* XHTML 1.0
    * XML was a language that allowed people to create their own languages. HTML 4 was reformulated to follow XML and was renamed XHTML, which created stricter rules, but allowed XHTML to work with other programs used for XML documents.
    * XHTML 1.0 was the creation of different versions that could allow authors transition into the new stricter syntax.
* HTML5
    * Authors were not required to close all tags, and new elements and attributes were introduced. HTML5 is not, complete, but the new features can be taken advantage of.
### Doctypes
Each web page should begin with a doctype to let the browser know which version of HTML is being used.
### Comments in HTML
To add a comment in the code that is not visible in the browser, you use `<!--These symbols-->`  
Comments are useful to remind you of things returning to your code after a time, or to help people looking at your code to understand it.  
It can also be used to comment out blocks of code you don't want to run currently.
### ID Attribute
Every HTML element can carry the ID attribute. It is used to identify that element against other elements on the page. The value should begin with a letter or an underscore and should not match any other ID on the page.  
It is known as a global attribute, because it can be used on any element.
### Class Attribute
Every HTML element an also carry a class attribute. You can use this to identify several elements as being different from the other elements on the page.
### Block Elements
Elements that always appear to start on a new line.
### Inline Elements
Elements that always appear to continue on the same line as the neighboring elements.
### Grouping Text & Elements Inline
The `<span>` element is an inline equivalent of the `<div>` element. It can contain a section of text or a number of inline elements.
### Iframes
The `<iframe>` element acts like a window cut into your page through which you can see another, commonly used to add google maps.
* The src attribute specifies the URL of the page within the frame
* The height attribute specifies the height of the iframe
* The width attribute specifies the width of the iframe
* Scroll bars are not supported by HTML5, but in the others you can add the value yes, no, or auto
* The frameborder attribute will not be supported in HTML5, but in the others it indicates whether the frame should have a border or not, with 0 being no and 1 being yes
* Seamless does not require a value, but is often given the value seamless, it removes the requirement for scroll bars, but will not work in older browsers
### Information About Your Pages
The `<meta>` element lives inside the `<head>` and contains info about the page. It is invisible to users, but informs search engines about your page. It is an empty element, so a closing tag isn't required. The most common attributes included are the name and content attributes, which specify properties of the entire page. Some commonly used elements are:
* description
    * Contains a description of the page, commonly used by the search engine
* robots
    * This indicates whether search engines should add this page to their results or not. `noindex` means it should not be added. `nofollow` means it can be, but no page that it links to.  
Meta also uses `http-equiv` and content attributes in pairs.
* author defines the author of the page
* pragma prevents the browser from caching the page
* expires indicates when the page should expire and can no longer be cached
### Escape Characters
If you want to use a character that has been reserved by HTML, such as the angle brackets, an escape character is needed. These are codes like `&amp;` for an ampersand, or `&copy;` for a cpoywright symbol.

[back](READNE.md)
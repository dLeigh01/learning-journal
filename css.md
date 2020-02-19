# Design Webpages With CSS
## Introducing CSS
### Understanding CSS
The key to understanding CSS is to imagine there is an box around every HTML element. CSS allows you to create rules that control the way each box is presented.
### CSS Associates Style Rules with HTML elements
CSS assigns rules to HTML elements, which governs how the content should be displayed using a selector -indicating which element it applies to- and a declaration -indicating how the element should be styled.
### CSS Properties Affect How Elements Are Displayed
CSS declarations are made up of a proerty -indicating the  aspects you want to change- and a value -specifying the settings you want to use- seperated by a colon between them and a semicolon between others within curly bracers.
### Using External CSS
`<link>` is used in HTML to tell the browser where to find the CSS file.  
`href` specifies the path to the CSS file.  
`type` specifies the type of document being linked to.
`rel` specifies the relationship between the HTML and the linked file.
### Using Internal CSS
`<style>` can be placed within the `<head>` to include CSS in an HTML file.
### How CSS Rules Cascade
If there are two or more rules relating to the same thing, one will take precedence.
* Last Rule
    * If identical, the last rule will take precedence
* Specificity
    * If one is more specific it will take precedence
* Important
    * Adding `!important` after a property value will signify it should take precedence
### Inheritance
If you specify a font or color on the body element, it will apply to all child elements
### Why Use External File Sheets?
All of your web pages can use the same style sheet. If you want to make a change, you only need to change one file instead of multiple, and the HTML code will be easier to edit.
## Color
### Foreground Color
The color property allows you to specify the color of text inside an element in one of three ways:
* RGB Values
* Hex Codes
* Color Names
### Background Color
CSS treats each HTML element as a box, and background-color changes what color that box is. You can specify your color choice in the same way you did foreground colors
### Understanding Color
Every color on a computer screen is created by mixing amounts of red, green, and blue.
* RGB Values
    * Values for red, green, and blue expressed as a number between 0 and 225.
* Hex Codes
    * Represent values for red, green, and blue in hexadecimal.
* Color Names
    * Colors are represented by pre-defined names.
* Hue
    * Hue is near to the colloquial idea of color.
* Saturation
    * Refers to the amount of grey in a color.
* Brightness
    * Refers to how much black is in a color.
### Contrast
When picking foreground and background colors, there must be enough contrast for the text to be visible.
* Low contrast
    * Text is harder to read and becomes a problem for those with visual impairment.
* High contrast
    * Text is easier to read, but is difficult to concentrate on for long periods of time.
* Medium contrast
    * For long spans of text, reducing the contrast makes for easier readability.
### CSS3 Opacity
The opacity property allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0.
### CSS3 HSL & HSLA
HSL uses the hue -expressed as an angle between 0-360- , saturation -expressed as a percentage- , and lightness -expressed as a percentage with 0% as white and 100% as black- values as a way to specify colors. Lightness is different from brightness because it can add white and black rather than just black.  
HSLA adds a fourth property to color picking that changes transparency known as alpha, which is expressed as a number between 0.0 and 1.0.

[back](README.md)
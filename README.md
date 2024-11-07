# css_cascade
This project demonstrates the CSS Cascade and how styles are inherited, overridden, and applied based on the specificity of CSS selectors. The HTML structure consists of multiple nested div elements with various classes and IDs to showcase how different styles interact.

# Project Structure
The project includes an HTML file (index.html) that demonstrates the cascade of styles.
The style.css file contains the CSS rules that style the elements.
The project uses a combination of class, ID, and element selectors to style the content.
# HTML Code
The HTML file consists of a series of nested div elements with classes and an ID to demonstrate how CSS rules cascade and override each other.

# Key Elements:
#outer-box: The outermost container with a border.
.box: A class used for styling multiple boxes with a blue background.
.inner-box: A nested class inside .box with a red background.
p: Paragraph elements with yellow text by default, except for those with the .white-text class.
.white-text: A class applied to paragraphs to change the text color to white.

# CSS Code
The style.css file defines the styles for the HTML elements. Here is a breakdown of the CSS:

# Key Styles:
.box: Applies a blue background and padding to any element with the box class.
p: Applies yellow text color, no margin, and no padding to all paragraph elements.
#outer-box: The ID selector applies a purple border to the outer container.
.inner-box: A specific class that applies a red background to nested boxes.
.white-text: A class that overrides the default yellow text color and sets it to white.

# How CSS Cascade Works in This Project
# The Cascade:
The cascading order is determined by:
**Source Order:** Styles defined later in the stylesheet (or in a more specific location) override earlier ones.
**Specificity:** ID selectors (#outer-box) have higher specificity than class selectors (.box), and class selectors have higher specificity than element selectors (p).
**Inheritance:** Styles like color are inherited from parent elements, but can be overridden by more specific styles.

# Example of Cascade in Action:
By default, all paragraphs (<p>) have yellow text.
The .white-text class applied to certain paragraphs overrides the default yellow text color and changes it to white.
The #outer-box has a purple border, which is applied because of the specificity of the ID selector.
The .box and .inner-box classes apply different background colors to the boxes, with .inner-box applying a red background that overrides the blue background of .box for nested boxes.

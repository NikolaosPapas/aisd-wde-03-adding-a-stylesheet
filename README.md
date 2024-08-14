
# WDE2 CSS BASICS

![Screenshot of the finished webpage](./assets/images/example.png)

### Description
Learn the basics of HTML structure and CSS styling by creating a simple webpage. You'll build an HTML document, link a CSS file, apply CSS for styling, and see the impact of each styling rule.

## Project Overview
In this assignment, you will create a basic webpage that outlines a typical day as a web developer. The project will demonstrate how to structure an HTML document and apply basic CSS styling. You will start by creating the HTML file, link a CSS file to style the page, and then break down the CSS into individual components to understand their functions.


## Project Structure

Your project should include the following files and folders:
- **index.html**: The main HTML file for the webpage.
- **styles.css**: The CSS file to style the HTML elements.
- **BasicCSS**: A folder to store your project files.

Here’s the file structure:
```
/BasicCSS
  index.html
  styles.css
```

## Setup Instructions

1. **Create the Project Folder and Files**
   - Create a folder named `BasicCSS` to store all your project files.
   - Inside the `BasicCSS` folder, create a file named `index.html`. This will be your main HTML file.
   - Also, in the `BasicCSS` folder, create another file named `styles.css`. This file will contain the CSS used to style your HTML content.

2. **Create the HTML File**  
   Now that you have your files set up, start by adding content to the `index.html` file.

   ### HTML Boilerplate
   First, set up the basic structure of an HTML document. This is known as the boilerplate:

   ```html
   <!DOCTYPE html>
   <html lang="en">

   <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>My Day as a Web Developer</title>
     <!-- link your CSS here  -->
   </head>

   <body>

    <!-- content code goes here  -->

   </body>

   </html>
   ```

   ### Explanation:
   - The `<!DOCTYPE html>` declaration defines the document type as HTML5.
   - The `<html lang="en">` tag specifies the language of the document.
   - The `<head>` section includes metadata like character encoding and viewport settings for responsiveness.
   - The `<title>` tag sets the title of the webpage, which appears in the browser tab.

3. **Linking the CSS File**
   After setting up the HTML boilerplate, the next step is to link your CSS file to the HTML document. This allows you to apply styling to the HTML elements.

   You should add the following `<link>` code **under the `<title>` tag but inside the `<head>` section only** of your HTML document:

   ```html
   <link rel="stylesheet" href="styles.css">
   ```

   ### Explanation:
   - The `<link rel="stylesheet" href="styles.css">` tag connects the HTML file to the CSS file.
   - The `rel="stylesheet"` attribute tells the browser that the linked file is a stylesheet.
   - The `href="styles.css"` attribute specifies the path to the CSS file. Since the `styles.css` file is located in the same folder (`BasicCSS`) as the `index.html` file, the path is simply `"styles.css"`.
   - **Important**: Ensure this `<link>` code is placed under the `<title>` tag and within the `<head>` section of your HTML document. This allows the browser to correctly identify and apply the CSS before rendering the body content.

4. **Add Content to the Body**
   Next, you'll add the content that will be displayed on the webpage inside the `<body>` tags.

   ```html
   
     <h1 id="title">My Day as a Web Developer</h1>

     <div class="morning">
       <h2>Morning Routine</h2>
       <p>Start the day with a cup of coffee and check emails.</p>
     </div>

     <div class="afternoon">
       <h2>Afternoon Work</h2>
       <p>Work on coding projects and attend team meetings.</p>
     </div>

     <div class="evening">
       <h2>Evening Wrap-Up</h2>
       <p>Review the day's work and plan for tomorrow.</p>
     </div>
 
   ```

   ### Explanation:
   - The `<h1>` tag is used for the main title of the page.
   - The `<div>` tags create separate sections for different parts of the day (`morning`, `afternoon`, and `evening`), each with a corresponding `<h2>` header and `<p>` paragraph for the content.

5. **Test the HTML Structure**
   Before adding any CSS, open your `index.html` file in a browser to see how it looks. It should display plain text without any styling as seen below.

##
  <img src="./assets/images/example2.png" alt="Example of unstyled HTML" width="275" height="200">

##

## Now lets add CSS code to style your page
Open the `styles.css` file in the `BasicCSS` folder and add the following code to style your webpage:

### Styling the Body
The first step is to apply a background color and margin to the entire page:

```css
/* Style the body */
body {
    background-color: #f0f8ff; /* Light blue background */
    margin: 20px; /* Add margin around the page */
}
```

- The `background-color` property sets the background color of the page to light blue.
- The `margin` property adds space around the entire page, keeping the content away from the edges of the browser window.

### Styling the Title
Next, you'll style the main title to make it stand out:

```css
/* Change the text color of the title */
#title {
    color: darkblue;
    font-size: 36px;
    margin-bottom: 20px;
    text-align: center;
}
```

- The `color` property changes the text color of the title to dark blue.
- The `font-size` property increases the size of the title text to 36 pixels.
- The `margin-bottom` property adds space below the title to separate it from the following content.
- The `text-align` property centers the title on the page.

### Styling the Morning Section
Each section of your webpage will have its own unique style. Let's start with the morning section:

```css
/* Style the morning section */
.morning {
    background-color: lightyellow;
    font-size: 18px;
    padding: 10px;
    margin-bottom: 20px;
}
```

- The `background-color` property sets the background color of the morning section to light yellow.
- The `font-size` property sets the text size within this section to 18 pixels.
- The `padding` property adds space inside the section, keeping the text away from the edges.
- The `margin-bottom` property adds space below the morning section to separate it from the next section.

### Styling the Afternoon Section
Now, let's style the afternoon section:

```css
/* Style the afternoon section */
.afternoon {
    background-color: lightgreen;
    font-size: 18px;
    padding: 10px;
    margin-bottom: 20px;
}
```

- The `background-color` property sets the background color of the afternoon section to light green.
- The `font-size`, `padding`, and `margin-bottom` properties are the same as in the morning section, ensuring consistent spacing and layout.

### Styling the Evening Section
Finally, style the evening section:

```css
/* Style the evening section */
.evening {
    background-color: lightcoral;
    font-size: 18px;
    padding: 10px;
}
```

- The `background-color` property sets the background color of the evening section to light coral.
- The `font-size` and `padding` properties are the same as in the previous sections, maintaining consistency.

### Styling All Headers
The last step is to style all the `h2` headers in the sections:

```css
/* Change the text color for all h2 elements */
h2 {
    color: darkred;
}
```

- The `color` property changes the text color of all `h2` elements to dark red, making them stand out against the background colors of each section.

## Testing Your Project

After completing the HTML and CSS files, save them and refresh your browser to see the styled webpage. You should notice the background colors, text alignments, and other styles applied.

### Things to test:
- Ensure that the `h1` title is centered and in dark blue.
- Check that each section (`morning`, `afternoon`, `evening`) has the correct background color.
- Verify that the `h2` headers are dark red.

## Conclusion

By completing this project, you’ve learned how to:
- Structure a basic HTML document.
- Link an external CSS file to style your webpage.
- Apply fundamental CSS properties to enhance the appearance of a webpage.




© All rights reserved to ThriveDX


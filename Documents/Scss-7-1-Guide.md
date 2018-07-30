## written by Soreg

# 7-1 Pattern

I have modified the scss folder to work with the 7-1 pattern. commonly used when working with Sass / Scss.<br>
If you have any questions or comments, please mention me with your question in the custonote channel, and I will reply as a thread.
___
## Structure
The 7-1 pattern is one of the most popular patterns to structure SCSS files, which is also used a lot in the industry.<br>
The 7-1 pattern is basically 7 sub-folders, which is all imported into one main file (hence the 7-1 name).<br>
Every folder has a responsibility for a specific part of the application.<br>
The folders and responsibilities are as follows: 
* Abstracts<br>
The abstracts folder deals with all the abstracts of the project, such as variables, functions and mixins.

* Base<br>
The base folder deals with all the 'basics' of our project, such as resets, normalizers and typography.

* Componnets<br>
The components folder deals with all the individual components, such as buttons, dropdowns and covers. Note that _some_ components can be defined in the Pages  or Themes folder, if they are page/theme-specific, and are not reused.

* Layout<br>
The layout folder deals with the layout of the application itself. This includes styles for headers, footers, sidebars, forms and grid (if we make one).

* Pages<br>
The pages folder deals with page-specific styles for ex. landingpage, notespage, contact etc.

* Themes<br>
The themes folder deals with theme-specific styles - ex. theme.scss, light-theme.scss and admin.scss. These files tend to be small, as they mostly change color on div's etc.


* Vendors<br>
The vendors folder imports 3rd party stylesheets from ex. bootstrap, uikit or jquery.
___

## Example of workflow
The 7-1 structure is fairly simple to work with when you learn it. I suggest keeping this guide at hand, so you know where to create your .scss files.<br>
<b>Add file:</b><br>
Say you want to add a style for a button, which can be used across all pages. The button is a reusable component, so we put it in the components folder as a new file - ex. button.scss (all button styles should go in this file, not one file per button). To import the styles you write, you go to the "_all.scss" file, and import it. The _all.scss file is automatically imported to the main scss file.<br>
<b>Remove / modify file:</b><br>
When you remove a file or modify a style, please make sure everything works as expected afterwards - especually if it's a style that's been used across multiple pages, such as components.
___
## If we use styled-components in React..
ReactJS has the possibility of importing and using [styled components](https://www.npmjs.com/package/styled-components). _If_ we decide to use this, we should have a plan for how we implement this with the 7-1 pattern.<br>
<b>My suggestion:</b><br>
I suggest we use the 7-1 structure in most places, but switch to styled-components if we need a specific style for a specific component in a specific location - ex. if we want a reusable button on our homepage, but we want this particular button to have some more padding, or another color.<br>
This part is still up for debate, and I don't think the use of styled-components is 100% agreed upon yet :)

___
Sorry for the long "guide". Again, if there's any questions, ping me anytime.<br>
_Go make something awesome_<br>

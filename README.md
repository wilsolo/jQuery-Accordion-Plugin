# jQuery-Accordion-Plugin
An accordion plugin with default styles

In order for the plugin to work there are a few requirements to put in the HTML as well as the javascript files. 

Set up for html file

First put in a script tag linking to the javascript file in your html file. In order for the plugin to work you must first link to the jQuery library. Following the plugin script tag should come a script tag where you will write your own javascript code. 
To get the accordion panels that slide out to hid bey default link to the accordion.css file as well in the head of your html file, this will apply the default styles written in the accordion.css file as well which can be overwritten by linking to your own css file in the head below the link to accordion.css. 

The plugin works using two classes, one called “accordion-control” which is always visible and causes the panel to slide in and out of view when clicked, this must be an <a> tag, and “accordion-panel” which is the content that slides into and out of view. 
Both these classes must be nested in a container such as a <div> or a <ul> tag. For clearer code you may nest the accordion-control and accordion-panel elements together in a container such as an <li> or another <div> tag. 

Set up for Javascript file

The code must be written inside a jQuery ready function. Use a jQuery selector on your container that holds all the accordion-control and accordion-panel groups, then call the accordion function to that selector using dot notation like so: $(‘.container’).accordion(500);
The function takes one parameter, as shown by the 500 in the example. This sets the speed at which the accordion-panel slides into view, it accepts numbers. 


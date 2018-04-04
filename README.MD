This project provides examples of updating CSS variables using vanilla JS. Meaning, dynamically updating CSS variables at runtime rather than at compile time. Stated differently, when you update a CSS variable with JS, everywhere on that page where the variable is used, will be updated as well. It doesn't use less or sass to accomplish it (ie. better than compile time only).

This project originates from and is largely based on a tutorial from Wes Bos.

This project demonstrates a few things:

* Using a span element to define a class ('hl' for highligher) on a particular chunk of text within a string. This provides a mechanism to
show using and changing a single variable which is used in multiple 
locations, in this case in the 'hl' class and also on the image where
the same variable (ie. --base) is used in both cases.
* Using sliders (range) and a color picker input controls, all contained 
  within the same form.
* Declaring where we wish to apply CSS variables; we use the "root" element, along with the variables, and default values for each variable.
```
    :root {
      --base: #ffc600;
      --spacing: 10px;
      --blur: 10px;
    }
```
* An example usage of CSS image style, filter: blur(someValue);
* Performing a JS querySelectorAll to select all element tags using a particular class.
* Using forEach on a Node List (without converting to an array and thus
  requires a new version of JS).
* Event listeners for a value 'change' event, as well as 'mousemove'.
* Usage of the <element>.dataset property which gives us access to the "data-*" attributes that might exist on that element (note that we also 
specify a default value if that data- attribute doesn't exist). 
 

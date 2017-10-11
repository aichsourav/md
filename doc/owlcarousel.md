# owlcarousel.md

Information about the default JavaScript included in the project.

## owl.carousel.min.js

This file can be used to contain or reference your site/app JavaScript code.
If you're working on something more advanced you might replace this file
entirely. That's cool. 

## Assets

This file can be used to contain all your plugins, such as jQuery plugins and
other 3rd party scripts for a simple site.

   **owl.carousel.min**
  This directory can be used to slide contain . 
   
   **oowl.theme.default.min**
  default the  file contains a small script to avoid 
    errors in browsers that lack a  The script will make sure that, if
    a console method isn't available, that method will have the value of empty
    function, thus, preventing the browser from throwing an error.
  

One approach is to put jQuery plugins inside of a `(function($){ ...
})(jQuery);` closure to make sure they're in the jQuery namespace safety
blanket. Read more about [jQuery plugin
authoring](https://learn.jquery.com/plugins/#Getting_Started).


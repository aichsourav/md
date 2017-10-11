[Directory - Listing Templates](https://pixelaar.com/) | [Documentation
table of contents](TOC.md)

# The JavaScript

The JavaScript / jQuery plugins uses are stored in js/ folder. You do not need to edit these items.

The script(s) you can edit as needed are:

js/scripts.js - This contains the plugin setup / init and general information
    
    !-- main jQuery -->
    <script src="js/jquery-3.2.1.min.js"></script>
    
    <!-- bootstrap core js -->
    <script src="js/bootstrap.min.js"></script>
    
    <!-- wow.min.js -->
    <script src="js/wow.min.js"></script>
    
    <!-- smoothscroll -->
    <script src="js/jquery.easeScroll.js"></script>
    
    <!--owl carousel-->
    <script src="owlcarousel/owl.carousel.min.js"></script>
    
    <!--Custom Scroll Bar-->
    <script src="js/jquery.mCustomScrollbar.js"></script>
    
    <!-- scrolling nav -->
    <script src="js/jquery.easing.min.js"></script>
    
    <!--Sidenav js-->
    <script src="js/sidenav.min.js"></script>
    
    <!--animation text js -->
    <script src="js/animation-text.js"></script>
    
    <!--magnific popup js-->
    <script src="js/magnific-popup.min.js"></script>
    
    <!-- custom script -->
    <script src="js/scripts.js"></script>

## scripts.js

This file can be used to contain or reference your site/app JavaScript code.
If you're working on something more advanced you might replace this file
entirely. That's cool. 

    // ------------------------------------------------------------------
    // jQuery for back to Top
    // ------------------------------------------------------------------

    (function(){

        $('body').append('<div id="toTop"><span>Up</span></div>');

        $(window).scroll(function () {
            if ($(this).scrollTop() != 0) {
                $('#toTop').fadeIn();
            } else {
                $('#toTop').fadeOut();
            }
        });

        $('#toTop').on('click',function(){
            $("html, body").animate({ scrollTop: 0 }, 600);
            return false;
        });

    }());


## plugins.js



One approach is to put jQuery plugins inside of a `(function($){ ...
})(jQuery);` closure to make sure they're in the jQuery namespace safety
blanket. Read more about 

By default the `plugins.js` file contains a small script to avoid `console`
errors in browsers that lack a `console`. The script will make sure that, if
a console method isn't available, that method will have the value of empty
function, thus, preventing the browser from throwing an error.
##maps
This file can be used to contain all your website maps such as jQuery plugins and
other 3rd party scripts for a simple site.
 
 
     var map = new google.maps.Map(document.getElementById('map'), {
            zoom: zoomLevel,
            scrollwheel: scrollEnabled,
            center: new google.maps.LatLng(40.80, -73.70),
            mapTypeId: google.maps.MapTypeId.ROADMAP,
            zoomControl: false,
            mapTypeControl: false,
            scaleControl: false,
            panControl: false,
            navigationControl: false,
            streetViewControl: false,
            styles: [{
                "featureType": "poi",
                "elementType": "labels.text.fill",
                "stylers": [{
                    "color": "#747474"
                }, {
                    "lightness": "23"
                }]
            },
## vendor

This directory can be used to contain all 3rd party library code.

Minified versions of the latest jQuery and Modernizr libraries are included by
default. You may wish to create your own 

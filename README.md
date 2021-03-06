UpThing
=======

An intro to Composer and Silex that can accept image uploads and generate thumbnails.

This project is tied to the "Quick Web Apps" series of articles on [Whateverthing.com](http://whateverthing.com), created by Kevin Boyd.

To give this code a spin, use [Composer](http://getcomposer.org) to install the dependencies (and then make sure to place symbolic links for components/ and vendor/twbs/bootstrap in the web/ folder - this part isn't automated yet. Hopefully soon I will find a better solution), then either use the internal PHP web server or set up an apache/nginx virtual host to test it out.

[![Build Status](https://travis-ci.org/beryllium/UpThing.png)](https://travis-ci.org/beryllium/UpThing)


### &raquo; [Quick Web Apps with Composer and Silex, Part One](http://whateverthing.com/blog/2013/06/28/quick-web-apps-part-one/)

Part One of the series deals with what is essentially a Hello World reference implementation, albeit with a slightly entertaining twist.

The user is introduced to the "composer init" and "composer install" commands, as well as creating a Bootstrap file for Silex and a front controller for their web-enabled routes.

Part One source code is available in the 0.1 branch.

### &raquo; [Quick Web Apps with Composer and Silex, Part Two](http://whateverthing.com/blog/2013/06/30/quick-web-apps-part-two/)

Part Two of the series expands on the default route, by adding File Upload functionality. It also adds a route that returns a Binary File Response, so individual uploaded files can be retrieved by an HTTP request. Finally, a simple "Gallery" is added that shows all the images that have been uploaded.

The code in this example is not ideal - in fact, it would serve as an excellent jumping off point for a guide on refactoring web code that is difficult to maintain.

Part Two source code is available in the 0.2 branch.

### &raquo; [Quick Web Apps with Composer and Silex, Part Three](http://whateverthing.com/blog/2013/07/01/quick-web-apps-part-three/)

Part Three of the series addresses some of the most egregious shortcomings of Part Two. By replacing the inline HTML code with Twig templates, the HTML components of the Gallery and Upload Form are separated into their own layer - this makes it easier to maintain and expand on them in the future. The other major topic covered is Imagine, an image manipulation library that can work with both PHP-GD and Imagick to accomplish some pretty neat things (I think that I didn't bring enough attention to this part of the post, so some people may have glossed over it - I definitely recommend checking out the changes made in the thumbnail code). 

The code in this example is slightly better than the previous parts, but it's still not 100% awesome. On the plus side, users are introduced to the "composer require" command, which is handy during development for pulling in new packages for your projects. 

Part Three source code is available in the 0.3 branch.

### &raquo; [Bootstrap 3: Quick Observations and a Demonstration](http://whateverthing.com/blog/2013/08/21/bootstrap-3-demonstration/)

This is a de facto Part Four for the Quick Web Apps series, although I glossed over the particulars of the implementation. It's not so much a how-to as it is a review of Bootstrap.

This part also marks the addition of the code to GitHub so anyone can check it out and fork it if they want. At this stage of development, I'd recommend not using it in production, however :)

Part Four source code is available in the 0.4 branch.

---

Stay tuned for further updates to UpThing, as I plan to explore some useful front end tools for improving the user experience, as well as some back-end API functionality. Also, unit and functional testing. This will show how Composer and Silex can be easily used to deliver a professional-quality web application in a fairly short timeframe.

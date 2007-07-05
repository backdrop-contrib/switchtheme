Switchtheme allows you to create a block to allow users to switch themes on the fly. 
The module will present users with a list of all enabled themes and allow them to
choose between them. Anonymous users have their choices tracked in a session variable.
For logged in users, the user record is updated with their choice so that their
last selection will stay the same the next time they log in. 

******* TO USE THIS MODULE ********

1) Activate all themes that you want users to choose from.

2) Go to the admin/blocks page and make sure that the select switchtheme block has
been activated and is available in every enabled theme. 

3) Go to the admin/access page and identify which user roles are allowed to see the 
switchtheme block. You may only want authenticated users to see it, for instance.
No one but the admin will be able to see the blocks until this is done, so do
this only after you have made sure that the block is visible in all views.

4) The theme names may not be very meaningful to regular users, so the module
settings page has an option to allow the admin to create titles to use for each theme. 
If no titles are created the theme name is displayed instead.


********     NOTES    *************

The module has been designed to defer to themes created by the sections module 
(http://www.drupal.org/project/section). In other words, if you use the sections 
module to create a special theme for the admin section, the  switchtheme 
module will use that theme rather than the individual theme chosen by the user.

If you want a quick way to review many themes before deciding which ones to install and
enable, try the Drupal Theme Garden (http://themes.drupal.org).

If you are setting up a lot of themes, you may find the blockregion module 
(http://www.drupal.org/project/blockregion) to be a helpful way of setting up blocks 
to work the same way across many themes. That will save you the time of setting up
every block in every theme.


********  USAGE EXAMPLE  ***********

You can use this module to present users with a small, medium, and large text version of
your site. To do that:

1) Select the theme that you want to use for this purpose. Create a subfolder below the
theme folder for every subtheme that you want to create (i.e. medium, large, and extra-large).
The folder names will be used as the theme names, so make sure they don't duplicate any
existing themes. One way to do that is to use the regular theme name as a prefix, then
append something to the name (i.e. bluemarine_large).

2) Copy the style.css and any theme images from the main folder to each of these sub-
folders. 

3) Change style.css in each subfolder to display appropriately for the chosen font size.
Well-designed css may only need to be changed in a few places. For instance, the
Bluemarine theme sets a basic font size at the very top of the css to 76%. Make that 
percentage higher and almost everything in the theme will be displayed in larger text. 
(You may need to change a few other css settings to get it working completely.)

Any style.css files and images in the subfolders will override those in the main folder,
but all folders will use the template.php and tpl.php files in the main theme folder,
so you don't need to duplicate all the template files, only the css and image files.

4) Go to the settings page and give the themes user-friendly names like 'Regular', 
'Medium', and 'Large' and turn the blocks on as noted above.

Now your users will have a drop-down selection list they can use to increase the
font size of their pages.







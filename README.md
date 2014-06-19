This is a simple responsive singularity/sass grid with breakpoints at 350px, 720px, and 1080px.

Below 1080px this grid is 90% fluid width, above it is fixed at 960px.
(Why 1080px? Because 960px/.90 ~= 1080px+/-, so there is minimal jitter on resize)

It has the following proportions at these breakpoints:
Above 1080px: 3 6 3
Below 1080px: 4 8

Below 1080px, the right & left 3 width sidebar columns move to the left 4 width column, with left above the right sidebar.  This is source independent.

This sass file is intended for Drupal 7.x Omega4 themes using singularity grids.  This assumption is reflected in the class names (.l-page, header.l-header, etc).  Do not enable layout extensions in the Omega4 settings.

Border colors have been added to grid elements for debugging and should obviously be removed in production.

Usage: The best way to use this grid is to copy the contents of the omega-subtheme.styles.scss file into your Omega4 child theme, which should be:
sites/all/themes/omega4_child_theme/sass/omega4_child_theme.styles.scss

Remember to set grid variables in variables folder:

Set variables in variables/_grid.scss file
$grids: 12;
$gutters: 1/4;


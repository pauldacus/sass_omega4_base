This is a simple responsive singularity/sass grid with breakpoints at 350px, 720px, and 960px.

Below 960px this grid is 90% fluid width, above it is fixed at 960px.

It has the following proportions at these breakpoints:
Above 960px: 3 6 3
Below 960px: 4 8

Below 960px, the right & left 3 width sidebar columns move to the left 4 width column, with left above the right sidebar.

This sass file is intended for Drupal 7.x Omega4 themes using singularity grids.  This assumption is reflected in the class names (.l-page, header.l-header, etc).  Do not enable layout extensions in the Omega4 settings.

Border colors have been added to grid elements for debugging and should obviously be removed in production.

# LibGuide dropdown template

A hack of the side-nav LibGuide template to include a more responsive nav menu. Using the `@media` rule, the usual side-nav menu will display after the `lg` breakpoint, i.e. when the window is ≥992px wide, while the dropdown is set to `display:none`. Below that width, the display settings swap so that the dropdown is displayed and the side-nav menu is set to `display:none`.

Importantly, I had to suppress submenus when the dropdown menu is displayed. Clicking on the submenu dropdown carat causes the main dropdown menu to close, meaning it has to be reopened to view the expanded submenu. Users will have to navigate to the top-level page in order for subpages to appear in the dropdown menu.

If you aren't sure what I mean by all of that, just remove `.nav > li > a.s-lg-tab-drop` from the `@media all and (max-width: 992px)` rule and test it out.

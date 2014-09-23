# FenixEdu Ashes Theme

Ashes is a theme for Bennu Portal, initially developed for the FenixEdu Academic application family.

Note: This theme requires Bennu Portal 3.3.0 or higher.

## About the Theme

The Ashes theme is based on Bootstrap 3.1, with a few minor customizations and quirks.

Note that as `portal.js` has been deprecated in Bennu 3.2, this theme does NOT contain a client-side layout.

## Layouts

This theme provides two layouts:

- 'default' (or 2-col): This layout features a top navigation bar with the app logo, a main area with 2 colums (one for a secondary menu, and another for the content) and a footer, containing the FenixEdu logo, the application's copyright notice and a link to the support email.
- 'one-col': This layout greatly resembles the 'default' layout, but on the main area, it only has one column, where the body is shown.

## Menu Organisation

Due to its multi-menu layout, this theme imposes a requirement:

- Applications should not be installed directly on the top-level, as their functionalities will not be shown in the side menu (which only expects containers).

## Known Issues

## A note on 'general.css'

The `general.css` file is included in the theme, and added to every page. This file is kept for legacy reasons (as it originated in the pre-Bennu Portal FenixEdu Academic) and should not have any impact on the Bootstrap or FenixEdu styles, only adding its own classes. If you find a situation where something is broken due to the presence of it, please file an issue.

When developing your application using the Ashes Theme, you should NEVER depend on `general.css` being there. Not only it deviates from the FenixEdu design standards, but it is subject to major changes (hopefully only deletions), even between revisions.

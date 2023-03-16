# 7-1 Architecture

This project uses the 7-1 architecture pattern for organizing Sass (Scss) files. The structure consists of the following folders:

1. abstracts/
2. base/
3. components/
4. layout/
5. pages/
6. themes/
7. vendors/

The `main.scss` file imports all styles from the folders and compiles them into a single CSS file.

## Folder Descriptions

- `abstracts/`: Sass tools and helpers, such as variables, mixins, functions, and media queries.
- `base/`: Global styles such as CSS resets, animations, typography, and basic HTML elements styling.
- `components/`: Reusable components like buttons, forms, cards, and other UI elements.
- `layout/`: Overall structure of the site, including styles for the header, footer, and grid system.
- `pages/`: Page-specific styles that may not be shared across the entire site.
- `themes/`: Various theme or color scheme styles for different designs or branding.
- `vendors/`: Third-party CSS libraries and frameworks.

## Usage

To use the 7-1 architecture in your project, follow these steps:

1. Create the seven folders (`abstracts/`, `base/`, `components/`, `layout/`, `pages/`, `themes/`, and `vendors/`) in your project's Sass (Scss) directory.
2. Create the `main.scss` file in the same directory as the folders.
3. Import the individual files from the seven folders into the `main.scss` file using the `@import` directive. The order of imports should follow the folder structure as shown below:

```scss
// main.scss

// Abstracts
@import 'abstracts/_variables';
@import 'abstracts/_mixins';
@import 'abstracts/_functions';
@import 'abstracts/_media';

// Base
@import 'base/_animations';
@import 'base/_typography';
@import 'base/_base';

// Components
@import 'components/_buttons';
@import 'components/_forms';
@import 'components/_cards';

// Layout
@import 'layout/_header';
@import 'layout/_footer';
@import 'layout/_grid';

// Pages
@import 'pages/_home';
@import 'pages/_about';
@import 'pages/_contact';

// Themes
@import 'themes/_default';
@import 'themes/_alternate';

// Vendors
@import 'vendors/_normalize';
@import 'vendors/_bootstrap';
@import 'vendors/_mantine';
```

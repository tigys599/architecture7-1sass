# 7-1

The 7-1 architecture is a design pattern for structuring Sass (or Scss) projects. It is composed of 7 different folders and 1 file. The 7 folders are:

base: contains global styles, such as CSS reset and typography.
components: contains specific, reusable components, such as buttons, forms, and cards.
layout: contains styling for the overall layout of the site, such as the grid system and header/footer.
pages: contains page-specific styles, if necessary.
themes: contains styling for different themes or color schemes.
abstracts: contains Sass tools and helpers, such as variables and mixins.
vendors: contains third-party CSS libraries and frameworks.
The 1 file is the main.scss file, which imports all the different files from the folders and compiles them into a single CSS file.

The 7-1 architecture is a way to keep the code organized, modular, and easy to maintain. It allows for easy scalability, reusability, and flexibility of the styles.

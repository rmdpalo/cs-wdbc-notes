# Semantic Elements & HTML Extras
## What is HTML 5
- Living Standard 
  - The HTML standard is a document that describes how HTML should work
- Role of Browsers
  - The standard describes the rules of HTML, but browsers actually have to do the work and implement HTML according to those rules.
- HTML 5
  - the latest evolution of the standard that defines HTML. It includes new elements & features for browsers to implement.
  - [HTML Standard](https://html.spec.whatwg.org/#is-this-html5?)
  
## Entity Code
- Special sequences that we can use inside of our HTML that will result in different characters. 
  - These could be reserved characters, or things that are difficult to type (i.e. the copyright character)
- Start with an ampersand and end with a semicolon
- the browser interprets them and renders the correct character instead.
- [Entity Code](https://entitycode.com/) / [Character Entity Reference Chart](https://dev.w3.org/html5/html-author/charref)

## Semantic Markup
relating to meaning, semantic markup is __meaningful markup__
- header, nav, main, footer, section, etc. all act like divs but are more meaningful and give us an idea of what its purpose is.
- why?
  - SEO: Search engines will consider its contents as important keywords to influence the page's search rankings. (-MDN)
  - Screen readers can use it as a signpost to help visually impaired users navigate a page.
  - finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
  - suggests to the developer the type of data that will be populated
  - semantic naming mirrors proper custom element/component naming (like in React)
- semantic elements
  - __main__ - houses the main content of a page that doesn't repeat in other pages (i.e. navbars, footers, headers, logos)
  - __nav__ - represents anything on the page that provides navigation links both to other pages and the same page.
  - __section__ - represents a standalone section of a website, pretty generic but still better than just a div.
  - __article__ - represents a self-contained composition in a document. (not exclusive to literal articles, includes blogs, forum posts, etc.)
  - __aside__ -  represents a portion of a document whose content is tangential to the main content. (sidebars)
  - __header__ - represents introductory content, typically a group of introductory or navigational aids. It may contain some heading elements but also a logo, search form, author name, and etc.
  - __footer__ - represents a footer for its nearest sectioning content or root element, usually contains information about the author of the seciont, the copyright data or links to related content.


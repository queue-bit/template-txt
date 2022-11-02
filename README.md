# HTML Template

This is a modified version of: 

> [TXT by HTML5 UP](https://html5up.net/txt)  
> html5up.net | @ajlkn  
> Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)

See the [original readme](README.txt)  
See the [license](LICENSE.txt)

This repo/version is specifically designed to work with my personal website builder ([https://github.com/queue-bit/go-pubsite](https://github.com/queue-bit/go-pubsite)) in a github action.


## Notable Changes From The Original

1. Removed files:
   1. index.html
   2. left-sidebar.html
   3. no-sidebar.html
   4. right-sidebar.html
2. Added files :
   1. Go Templating (for `html/template`, together these make up a modified version of index.html):
      1. base/base.html
      2. base/body.html
      3. base/footer.html
      4. base/header.html
   2. CSS:
      1. assets/css/extend.css

## Go Template Expected Vars


Expects a struct with the following defined:

| Struct | Member | Description |
|-|-|-|
| CurrentPage | Title | Title of the current page |
| CurrentPage | Nav | Breadcrumb nav of the current page |
| CurrentPage | Excerpt | Excerpt of the current page |
| CurrentPage | Content | The page content (article body) |
| CurrentPage | SiteRoot | URL of the site's root |
| CurrentPage | Analytics | Analytics Code (HTML with script tag) |
| SiteMetaData | Twitter | URL to Twitter user |
| SiteMetaData | Github | URL to GitHub user |
| SiteMetaData | Linkedin | URL to LinkedIn user |
| SiteMetaData | Domain | The domain as defined in the config file |
| SiteMetaData | Title | The site's title as defined in the config file |
| - | Toc | Table of Contents (HTML) |
| - | TopNav | The top navigation (HTML) |
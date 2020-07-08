# staticSearch

### A codebase to support a pure JSON search engine requiring no backend for any XHTML5 document collection

This codebase, developed by Joey Takeda and Martin Holmes, provides a configurable, customizable tool which you can point at an XHTML5 document collection and have it generate a search page which requires no backend server-side component. It creates stemmed indexes of all document text, along with an HTML search page including faceted search features based on `<meta>` tags in the document collection. It also supports wildcards in search terms. The search page uses pure JavaScript to query the index, which is a large collection of small JSON files, to provide a rapid and sophisticated search for any small-to-medium website. The search does not require any server-side code at all.

The generation code uses XSLT3 and the search functionality is JavaScript. Implementations of the Porter2 stemmer in XSLT and JavaScript are part of the package. A live search page based on this code is already in use in the site _Mapping Keats's Progress_ https://johnkeats.uvic.ca/search.html.

The default branch of this repo is the dev branch; the master branch is used for releases. Formal releases started in early 2020, and the master branch will always reflect the latest release tag, so you can pin your own project either to master or to a specific release tag to avoid unexpected changes in behaviour due to codebase changes. For testing to prepare for upcoming changes, you can use the dev branch.

Full documentation can be found in the file docs/staticSearch.html.

Please report all issues you encounter as tickets on the repo.

The code is licensed under both MPL and BSD. 

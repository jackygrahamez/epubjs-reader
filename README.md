Epub.js Reader
================================

![Demo](http://blogs.ischool.berkeley.edu/i202f13/files/2013/10/Screen-Shot-2013-10-10-at-8.02.43-PM-1024x627.png)

[Try it while reading Moby Dick](http://epubjs-reader.appspot.com/)

About the Reader
-------------------------
This reader came out of the Berkeley Future of eBooks classes in Fall & Spring 2013.
It renders a ePub version of the TDO book using the [Epub.js](http://futurepress.github.com/epub.js/) library.

It is very much still a work in progress, so please bear with us. We would greatly appreciate reports on any bug or issues you come across

Getting Started
-------------------------

All the rendering is encapsulated within Angular directives.

```<epubreader>``` has only a src attribute and will render the complete reader.

```html
<epubreader src="/moby-dick/"></epubreader>
```

```<epubviewer>``` has several more attributes, requiring only only a src and will display just the basic epub, without the rest of the interface elements.

```html
<epubviewer src="{{src}}"></epubviewer>
```

Other available attributes are:

* on-ready
* on-chapter-displayed
* on-page-changed
* path
* cfi
* metadata
* toc

Deploying to App Engine
-------------------------

Update the app.yaml with you application id.

Then run:
```
appcfg.py update .
```

Additional Resources
-------------------------

[Epub.js Developer Mailing List](https://groups.google.com/forum/#!forum/epubjs)

IRC Server: freenode.net Channel: #epub.js

Follow us on twitter: @Epubjs

+ http://twitter.com/#!/Epubjs

Other
-------------------------

EPUB is a registered trademark of the [IDPF](http://idpf.org/). 

waldyrious.github.io
====================

Redesign of my webpage (http://waldirpimenta.com)

### Implementation notes

- **Fully [client-side](https://en.wikipedia.org/wiki/Client-side_scripting)**:
  no need for server logic, can be statically hosted
- **[DRY code](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)**:
  common elements (navigation menu and footer) are defined once and instantiated multiple times
    - Declarative (non-js) inclusion of common header and footer through seamless iframes
    - Declarative inclusion of resources (css/js) not yet possible, so header isn't fully DRY.
- **[Progressively enhanced](https://en.wikipedia.org/wiki/Progressive_enhancement)**:
  functional without js and even css
  (except iframes' seamlessness, which currently relies in css
  [while waiting for browsers to catch up](http://caniuse.com/#feat=iframe-seamless))
- **[Valid](http://validator.w3.org/check?uri=http://waldyrious.github.io),
  [polyglot xhtml5](http://www.w3.org/TR/html-polyglot/)**:
  well-formed, valid as both html5 and xml;
  machine readable with any xml parser; errors are fatal so they don't creep up.
- **[Mobile-friendly](https://www.google.com/webmasters/tools/mobile-friendly/?url=http://waldyrious.github.io)**


### Todo:

- [x] home
- [ ] works
- [ ] updates
    - Automatic feed -- need to think how to do it.
      Perhaps emulate friendfeed using Zapier, IFTTT or Yahoo Pipes.
      Or maybe build an app for it with Firebase.
      Sources: check out "from me" collection in feedly, my current friendfeed, github
    - Since this will provide dynamic content, have the link be added dynamically to the navbar
- [ ] blog
    - Need to think what platform to use.
      Something simple, with RSS/Atom and Discus comments
- [x] cv
- [x] timeline
- [x] contact


### License:

* [Creative Commons Attribution-ShareAlike 4.0 International](http://creativecommons.org/licenses/by-sa/4.0/)

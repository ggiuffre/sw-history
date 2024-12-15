# History of web apps


## World Wide Web

Represent information as a graph of static documents. Made for scientific
documents.

Problems that is solves:
* share information [...]

Open problems:
* documents are static, not customizable based on request parameters


## Dynamic rendering on the server

E.g. PHP, Perl, ASP, Django [...]


## Dynamic rendering on the client / Client-side scripting?

Users can interact with HTML pages via buttons and other things that trigger
events. Events are handled by a script that manipulates the DOM.


## AJAX

Client-side scripts can asynchronously query an API while manipulating the DOM.


## Reactive programming

The view is just a function of state. Views react to state changes.
Applications are a composition of multiple views, possibly nested. Views bring
together HTML, CSS and JS so that developers can now build applications with
actually good UX.

Problems that it solves:
* Developer experience doesn't suck anymore; we basically went from imperative to declarative


## Single-page applications

E.g. create-react-app, Parcel, Angular... basically a response to the insane
complexity that comes up if you try to use pure React for a production app [...]

Open problems:
* bundle size quickly gets too big -> bad for slow connections or small CPUs
* bad for search engines and for accessibility: you are greeted by an empty div with id="root"
* requires an API
* designed for small websites that have a single app shell


## Next.js / SSG?

Basically dynamically choose between SSG, SSR CSR, and "ISR" [...]

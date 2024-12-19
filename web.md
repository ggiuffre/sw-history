# History of web apps


## World Wide Web

Represent information as a graph of static documents. Made for scientific
documents.

Problems that is solves:
* share information [...]

Open problems:
* documents are static, not customizable based on request parameters

First appeared in 1989.


## Server-side scripting

Web servers don't just answer requests based on which page was asked, but on
every request run a script that produces a response customized to the request.
Example scripting languages and frameworks are PHP (1995), ASP.NET (2002) and
Django (2005). Note that this also allows web pages to act as the interface to
a database.

Problems that is solves:
* documents contain information that can depend on request parameters and/or on
  context (for example what time it is)
* interaction with a web application is slow (every interaction requires a
  network call)

Open problems:
* users cannot interact with a documemt in the way they would with a normal
  program (documents are not "interactive")


## Client-side scripting

Users can interact with HTML pages via buttons and other things that trigger
events. Events are handled by a script that manipulates the DOM.

Problems that it solves:
* documents are interactive
* interacting with a web site is faster — not all interactions require a
  network call

Open problems:
* data updates require a full page reload
* client-side scripts are limited to modifying the DOM


## AJAX

Client-side scripts can asynchronously query an API while manipulating the DOM.

Problems that it solves:
* data updates can be done in the background

Open problems:
* web page interactivity is a second thought — it has to be done imperatively
  and programs have to modify the DOM in an unstructured way


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

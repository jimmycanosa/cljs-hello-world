### ClojureScript: simple within parenthesis

Example code using:
* ClojureScript
* Shadow-cljs
* Reagent
* re-frame
* a third party React library (`react-tooltip`)
* a third party JavaScript library (`date-fns`)

Here is a clickable example [web page](https://jimmycanosa.github.io/cljs-hello-world/public/) based on the source code of this repo.

##### References
Have a look at this [Blog post](https://davidvujic.blogspot.com/2021/01/simple-within-parentheses.html) 
for an introduction to `Clojure`, `ClojureScript`, `Reagent` and `re-frame`.

[Slides](https://docs.google.com/presentation/d/1UoB09b2sT3RrZ8L6-ZN9sRGQ8WTnzvI32-M7IXJsEtE/edit?usp=sharing) 
in :sweden: used in the 2021-01-20 [FreeCode MeetUp Series](https://freecode-meetup-series.confetti.events)
and the presentation in :sweden: [on Youtube](https://youtu.be/o-NhnF-t-JE)

Looking for code and examples from __FuncProg Second MeetUp 2021__?
[It's in this feature branch](https://github.com/DavidVujic/cljs-hello-world/tree/func-prog-2021-second-meetup)

##### Development
Starting the app:

``` bash
npx shadow-cljs watch app tests
```

You can now browse:
* the example web page at http://localhost:8080
* the unit test page at http://localhost:8081

###### Emacs
Or, if you are using Emacs, run the command `cider-jack-in-cljs` from the editor. 
To make the app startup process even smoother, create a `.dir-locals.el` file in the root folder, add this to it:

``` emacs-lisp
((nil . ((cider-default-cljs-repl . shadow)
         (cider-shadow-default-options . ":app")
         (cider-shadow-watched-builds . (":app" ":tests")))))
```

##### The CSS
The theme switching `css` comes from this [blog post](https://alexandersandberg.com/theme-switcher/).

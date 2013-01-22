# Presentation: some language experiments

Online as slide show at http://solsort.com/2013/berlincompiler

# Personal Notes

## Content

- talk
    - intro
        - intro
            - this talk: interactive, interrupt, ask questions
            - my background
        - vision: the next billion
        - idea: canonical syntax
            - homoiconicity to the next level - source text as a serialisation format for the AST
            - designed for code transformations
            - practical experiments: Yolan and LightScript
            - have you seen this idea before? where?
    - concrete experiments
        - lightscript/yolan
            - JavaScript/lisp-like language on J2ME
        - yolan 2
            - self-hosted
            - visual code
            - hosted on the JS-vm
            - method-calls instead of function calls
            - `[code]`
            - experience: dogfood not good enough, lists not rich enough
        - lightscript 2/3
            - Combined TDOP-parser + prettyprinter for JS/C-like language
            - self-hosted
            - staged computation
            - towards common scripting language denominator
            - `[code]`
            - experience: dogfood currently just limited JS, want optional static typing, non-js-semantics, newline-comment-node
    - conclusion / discussion
        - next step: Yolan 3
        - discussion: critical feedback
        - discussion: language features



- This talk
    - interactive, interrupt, ask questions
- Background
- Canonical syntax
    - homoiconicity to the next level - source text as a serialisation format for the AST
    - designed for code transformations
    - practical experiments: Yolan and LightScript
    - have you seen this idea before? where?
- Vision
    - programming for the next billion
    - textual code representation will not suffice
    - platform is mobile
    - personal tool, eat-my-own-dogfood
- Experiment: LightScript/Yolan
    - 
- Experiment: Yolan 2
    - self-hosted
    - visual code
    - hosted on the JS-vm
    - method-calls instead of function calls
    - experience: dogfood not good enough, lists not rich enough
- Experiment: LightScript 2/3
    - Combined TDOP-parser + prettyprinter for JS/C-like language
    - self-hosted
    - staged computation
    - towards common scripting language denominator
    - experience: dogfood currently just limited JS, want optional static typing, non-js-semantics, newline-comment-node
- .. Top-down operator precedence
- Wanted dogfood: Yolan 3
    - hosted on common scripting language denominator
        - portable core + platform specific extensions
    - JS-to-Yolan
    - optional static typing
- discussion
    - your opinion? Critical feedback?
    - what are your favorite language features, why?
    - your opinion?
    - your opinion on language feature/design-must-have
    - what do you think
    - what are your critical 
- Extras
    - generational GC
    - theaded code / interpreter
        - direct threaded vs. indirect threaded
    - inline caching
    - partial evaluation

- intro
    - form: informal
    - background
        - personal language experiments
        - started out with master-thesis w/ languages for j2me
        - lightscript - a javascript dialect
        - yolan - a lisp dialect
        - following iterations + total rewrites
    - purpose:
        - present current experiments + try-out-ideas
    - interrupt with questions
    - plan for the presentation
        - two ideas: canonical syntax and language abstraction
        - ideas
            - canonical syntax
            - language abstraction
- what - personal language experiments
    - ls1/yl1 javascript-dialect and lisp-like language for j2me and thesis
    - yl2 lisp-like syntax for js; canonical syntax; self-hosted
    - ls2/ls3 - canonical syntax for a subset of js;
        - ls2 - self hosted, no var statement, staged execution
        - ls3 - stricter semantic subset for re-targetability
    - yl3 - to be implemented
- canonical syntax (implemented / proof of concept)
    - the idea
        - canonical syntax / reversible parsing
        - why:
            - design language for program transformations
            - textual representation is good for development with a keyboard...
                - the next billion
    - parsing
        - grammar vs. operator precedence
    - pretty-printing
    - general syntax of c-like languages
        - ... { .. }
        - elegance of implementation vs. corner-cases
    - diving into the source
- personal conclusions / experiences
    - yl bootstrap development
    - common patterns in c-like-syntax
    - method-invocation as basic building block when making lisp-syntax for js
    - want optional static typing
- vision / future direction
    - non-textual representation for editing
        - canonical syntax
        - optional static typing
    - hosted scripting language with portable core
        - common core for scripting languages (map+array+class+lambda)
- discussion
    - does it make sense
        - canonical syntax
        - hosted scripting language with portable core
    - what language features do you deem important and why
- Too much time?
    - anybody something?
    - some other stuff i could talk about
        - generational GC
        - theaded code / interpreter
            - direct threaded vs. indirect threaded
        - inline caching
        - partial evaluation

## Presentation style

- focus areas
    - vision
    - technical/language-stuff
    - personal conclusion / journey
- switch between 3 screens
    - vim scratchpad
    - reveal.js slide show
    - lightscript source code

Uses [reveal.js](https://github.com/hakimel/reveal.js/) as slideshow engine, which is most of the files in the repository (except index.html and readme)

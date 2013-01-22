# Presentation: some language experiments

Online as slide show at http://solsort.com/2013/berlincompiler

# Personal Notes

## Content

- intro
    - intro
        - this talk: interactive, interrupt, ask questions
        - purpose: present/share vision + get feedback / present current experiments + try-out-ideas
        - my background
    - vision: the next billion
        - programming for the next billion
        - platform is mobile
        - textual code representation will not suffice
    - idea: canonical syntax
        - homoiconicity to the next level - source text as a serialisation format for the AST
        - designed for code transformations
        - practical experiments: Yolan and LightScript
        - have you seen this idea before? where?
- concrete experiments
    - lightscript/yolan
        - JavaScript/lisp-like language on J2ME
        - master thesis at University of Copenhagen
    - yolan 2
        - self-hosted
        - visual code
        - hosted on the JS-vm
        - method invocation instead of function calls
        - `[code]`
        - experience: dogfood not good enough, lists not rich enough
    - lightscript 2/3
        - Combined TDOP-parser + prettyprinter for JS/C-like language - common patterns in syntax
        - self-hosted
        - staged computation
        - towards common scripting language denominator
        - `[code]`
        - experience: dogfood currently just limited JS, want optional static typing, non-js-semantics, newline-comment-node
    - next step: Yolan 3 dogfood
        - hosted on common scripting language denominator
            - portable core + platform specific extensions
        - JS-to-Yolan
        - optional static typing
- conclusion / discussion
    - discussion: critical feedback
    - discussion: favorite language features, why?
- Extras if excess time
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

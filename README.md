# BRS Reskin Notes
----------------

### Utilize Foundation for Components

Most components (tables, typography etc) can be styled through a front-end framework like Foundation. This cuts down time on having to redesign every separate component, especially if it's a pain to change markup.

I've included an **example** folder which quickly spins up a very basic Foundation project with icon fonts included.

You can find more about Foundation here:

http://foundation.zurb.com/docs/

### You Can Reference the Prototype

Feel free to also reference the BRS prototype if useful. *(click login button to enter)*


[Big Red Sky Protoype](http://bigredsky.uat.liquidvisual.net)
[Source Repo](https://github.com/liquidvisual/brs-0115)

This was an early proof-of-concept that had more design and UX involved. For the basic reskin, it's really about just getting the application frame to work, stripping back existing styles and overriding with clean defaults (like Foundation's).

The *Screen Note* images should help assist in the coding of the re-skinned application frame - it doesn't have to be perfect though, feel free to improvise or tweak values based on what you feel is right during development.

### Icon Fonts

Instead of using tiny images and sprites for everything - it's easier to utilise font icon libraries. This brings the weight down and makes scaling easier. We can also change the colours for active & hover states.

The two libraries I recommend:

1. [Foundation Icon Fonts 3](http://zurb.com/playground/foundation-icon-fonts-3) - best for main navigation icons for their size and consistency
2. [Font Awesome](http://fontawesome.io/cheatsheet/) - for everything else - incl. arrows and micro symbols

Place these in the master template:

    <link rel="stylesheet" href="src/css/foundation-icons.css">
    <link rel="stylesheet" href="src/css/font-awesome.css">

Include font icons in markup like this:

    <i class="fi-home"></i> // Foundation Icons
    <i class="fa fa-home"></i> // Font Awesome
    
---
    
### Open Sans Font
    
    <link rel="stylesheet" href="http://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,700italic,400,300,700">
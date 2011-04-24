# Arrangement for View Assets Pattern

- [Introduction to the AVA Pattern](#introduction)
  - [Why do we need the AVA Pattern](#)
  - [What do I get from the AVA Pattern, besides consistency?](#)
- [/images/ Directory Convention](#images)
  - [Grouping Rules](#images/grouping-rules)
  - [Naming Rules](#images/naming-rules)
  - [Examples](#images/examples)

<a name="introduction"></a>
## Introduction to the AVA Pattern

In the recent years, we’ve been seeing a lot of improvements on the organization procedures for web applications. More specifically, the MVC Pattern; which greatly improved development speeds by imposing a well structured architecture. This allowed developers to feel at home with any application that uses the pattern.

The Model-View-Controller (MVC) Pattern is oriented to the back-end. There’s a specification about where to store your interface related code, the View, but there’s no real specification regarding how and where you should store your assets. This is where the Arrangement for View Assets (AVA) Pattern shines.

The AVA Pattern works side by side with the MVC Pattern. Both are framework and language agnostic, and independent of each other, but together you can achieve a better organization which will improve productivity, especially during advanced stages of the application.

Take these with a grain of salt and remember that you should always use what your team is accustomed to; these conventions may be modified to fit your project, however, try to follow the general idea about the structure.

For instance, you may want use snake_case over the dash-case naming pattern; these types of modifications are a matter of preference. 

### Why do we need the AVA Pattern?

You may think that there's a steep learning curve involved with the AVA Pattern; however this is not true. The main objective of the AVA Pattern is to provide a written docuentation for you and your team to consult when in doubt about how to store your assets.

### What do I get from the AVA Pattern, besides consistency?

The main plus you'll get from the AVA Pattern is consitency. And that alone is something that is worth your time. Consistency is not something you should only want to achieve when you're working on a team with other Developers working on the Front-End but it's something you should aim for for your own sake.

Think of the following use cases:

- As a Freelancer
  - The odds are that you're going to work alone on the project. You complete the project and months later you need to give maintenance to the project; and you completely forgot about the file structure and file names of the project. You'll spend some time trying to figure out your own code.
- As a member of a Development Team
  - You're part of a team that has another front-end Engineer besides you; everything is fine and dandy till he begins naming files under a completely different directory than the one you set; after some time you can notice who made what just by how it's stored.
- As a Team Leader
- As an Outsourcer

## Overview of the Structure.

Need to write some stuff here..

    /css/                         # Documented? Soon.
      style.css
      handheld.css
    /img/                         # Documented? ✓
    /js/                          # Documented? Soon.
      tests/
        qunit/
        index.html
        tests.js
      libs/                      
        jquery-1.5.1.min.js
        jquery-1.5.1.js
        modernizr-1.7.min.js
        dd-belatedpng.js
      plugins.js
      script.js

<a name="images"></a>
## /img/ Directory Convention

Conventions save you from having to figure out how the project is structured. The following conventions are the result of testing and polishing rules on production environment over the years.

<a name="images/grouping-rules"></a>
### Grouping Rules

Grouping is important; especially when you're working with projects that have many assets. The following rule proposes a way to organize these files into an easy to navigate way.

    RULE
      IF images FROM same GROUP > 5
        store in new directory
        repeat RULE
      else
        store in root

This rule may loop a max of 3 times. Having too many levels is not advised since it may make everything more complex to mantain in the long run and will make your css file bigger.

<a name="images/naming-rules"></a>
### Naming Rules

Names for individual files should always be **singular**, even if they're sprites that contains several elements. This is, by convention, a good practice that is taken from other web related frameworks.

Sub-Directories a.k.a. Groups should be named in their **plural** form when possible. Remember, this only applies to directories. For files, use the singular variant.

This whole plural/singular paradigm is to follow web frameworks and database naming conventions; think of it as a general recomendation.


    background files:
      bg(-group)?(-name)
    sprites:
      sp(-group)?(-name)
    buttons:
      bt(-group)?(-name)
    icons:
      ic(-group)?(-name)
    other:
      (group-)?(name)

When the file is going to have several variants, it's a good practice to append the change in type or dimension using the following pattern.

    (name)((-HEIGHTx)(WIDTH)?)?

Please note 

    logo-300x.jpg
    logo-500x250.jpg
    logo-500x300.jpg
    logo-300x-grayscale.jpg

Notice that you're not forced to add the height when there's no variation to that file. The `x` is still left in place to denote that we're talking about width and not height:
    
    50x <- 50 width
    x50 <- 50 height

<a name="images/examples"></a>
### Examples

Need to document this further.
  
    /bg-content.jpg
    /bg-content-light.jpg
    /sp-main.jpg
    /ic-form-submit.jpg
    /placeholders/
      content-big.jpg
      content-small.jpg
      content-medium.jpg
      user-display-100x.jpg
      user-display-200x.jpg
      video-medium.jpg
      
      
      
#### Thanks to:

- [Armando Canals](http://twitter.com/armandocanals) for his feedback.
- [Cesar Salazar](http://twitter.com/cesarsalazar) for his feedback.
- [Chris Eppstein](http://twitter.com/chriseppstein) for his feedback.

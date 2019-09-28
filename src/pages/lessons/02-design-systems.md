---
title: "Design Systems"
number: 2
type: lessons
cover: "https://source.unsplash.com/rhNff6hB41s"
---
import { Subpage, Callout } from "../../course-components";

<Subpage slug="intro">

### Introduction

This lesson we'll talk about design to development handoff and introduce design systems. We'll also look at how you can build your own UI toolkit.

</Subpage>
<Subpage slug="design-systems">

### Design Systems

A big deal in contemporary interaction design today is the topic of Design Systems. I'm going to send you right to one of the best sources on this topic today: Invision's Design Better site. Run by the legendary Aarronn Walter (remember _Designing for Emotion_ from the UX class?), this is a fabulous resource for digital product designers and front end designers. In particular, lets dive into their book [_Design Systems Handbook_](https://www.designbetter.co/design-systems-handbook).

<Callout color="alternate" lead={true}>

Skim [_Design Systems Handbook_](https://www.designbetter.co/design-systems-handbook).

<small>Read as much as you're able in detail but at least be familiar with the main concepts, methods, and process discussed in this book.</small>

</Callout>

For more examples of this idea and inspiration for the possibilities consult the [Design Systems Repo](https://designsystemsrep) for a collection of official design systems for brands such as Salesforce, Audi and Apple.

</Subpage>
<Subpage slug="mockups">

### Mockups for Design Systems

Design Systems can be quite a big deal to put together and take a whole course in themselves. One subset of a design system that is practical to hone in on and gain experience working with in the context of this course is the component library portion. Also known as a UI toolkit, this portion of a design system prescribes actual code that should be used to create components of a particular design system. Some of the design systems you observed in the last section included component libraries.

Such a component library typically includes the following:

- A color scheme
- A set of fonts and basic type styles
- A grid system for laying out elements consistently
- A scalable library of specific components including everything from form fields and buttons to complex structures that occur in the system

In this course we'll demonstrate using the Fabricator system to build UI Toolkits.

<Callout color="alternate" lead={true}>

Read this [introduction to UI Toolkits](https://fbrctr.github.io/getting-started/what-is-a-toolkit.html)

</Callout>

Knowing that where we're going is to create this library of components and structures, it follows that we should first plan them and mock them up. Note that this comes after we've worked through wireframes and style tiles for the project and thus have a solid sense of the overall elements our project will need as well as some initial approval of the visual direction we'll be taking.

Watch this demonstration of mockup techniques using Sketch:

<iframe width="560" height="315" src="https://www.youtube.com/embed/tuDbVTt8q7c" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</Subpage>
<Subpage slug="ui-toolkit">

### Living System as UI Toolkit

Mocking up a design system is a lot of work, but worth it to ensure you have a solid plan. The next step is to ensure this plan can be easily used by developers consistently and without compromise. As discussed in the _Design Systems Handbook_ there are many approaches to this including whole teams managing the system and its implementation. In smaller companies this may be simply you, the hybrid designer/developer. In such cases a great tool to learn is an older but great tool called Fabricator.

<Callout color="alternate" lead={true}>

Skim the [Fabricator Website](https://fbrctr.github.io/)

</Callout>

Here's what makes this tool great:

- It allows you to create a library of UI components and their styles in an isolated way (separate from their use in a website). This includes, by default, individual components, combined/complex structures, and whole page prototypes.
- It creates a documentation website for you as you work so you can easily show the components and keep notes about their use.
- It creates a bundle you can easily distribute to where the styles are to be used.
- You don't have to learn a JavaScript framework to use it; basic knowledge of templating with [Handlebars](https://handlebarsjs.com/) is sufficient for the most part.

Here's how to get set up:

1. Create an empty repo for your system on Github, clone it to your computer and use Terminal or the integrated terminal in your code editor to navigate into your repo's root folder.
2. (Ensuring you're in your repo's root folder) Run this code from the Fabricator Startup guid:
  ```bash
  curl -L https://github.com/fbrctr/fabricator/archive/master.tar.gz | tar zx --strip 1
  ```
  This downloads the fabricator base code and unzips it into your project folder.
3. Run `npm start` to start up the Fabricator system. This includes an install step so you'll see a `node_modules` folder appear with all the dependencies for the system. It also generates the asset bundle and documentation site in a `dist` folder. The system should automatically open in your browser at `localhost:3000`.
4. Open and update the `package.json` and update the name, version, description, and author to reflect your project. Remove the `homepage` line altogether.
5. Open and update the `README.md` with information about your project. For appropriate ackowledgement, include this line somewhere:
  ```md
  Built using [Fabricator](http://fbrctr.github.io/) by [Luke Askew](http://twitter.com/lukeaskew).
  ```
5. Commit this initial file set in your project repo.
6. Move to your `develop` branch for work from here forward as you add new features.

<iframe width="560" height="315" src="https://www.youtube.com/embed/yXd15DsCo7Q" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Next you need to get busy adding the styles and "materials" that will make up your system. Here's an overview:

- Edit the landing page for the documentation site as you see fit by opening and editing `src/views/index.html`.
- Populate your system's color values in `data/tookit.yml` using the structure you see there by default.
- Add/modify the `.html` files in the `src/materials/components` folder to create the markup for your core set of simple components. Learn more [here](https://fbrctr.github.io/building-a-toolkit/materials.html).
- As needed, you can add an `images` folder in the `src/assets/tookit` folder and point to them using the path: `/assets/toolkit/images/` in your component.
- Add styles for your components as you see fit inside the `src/assets/tookit/styles` folder. There is a toolkit.scss Sass file there by default set up and ready for you to use imports and partials for your modular style sheets as you've learned about in previous projects.
- Add more complex structures as you did components but using the `src/materials/structures` folder.
- Prototype complete pages by adding `.html` files in the `src/views/pages` folder.
- As needed, override default Fabricator system styles using files in the `src/assets/fabricator/styles` folder.

Throughout the `html` files note the following helpful conventions:

- All `.html` files can begin with Frontmatter blocks that allow to provide notes describing your materials. [Read more](https://fbrctr.github.io/building-a-toolkit/materials.html#documenting-a-material)
- You can use standard markup as well as Handlebars to display variables from data sources. [Read more](https://fbrctr.github.io/building-a-toolkit/data.html)
- Include components in other components or structures using the partial syntax from Handlebars. So if we have a component called `button.html` we can include it elsewhere with `{{> button}}`.

<iframe width="560" height="315" src="https://www.youtube.com/embed/10YmN2VVOwc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</Subpage>

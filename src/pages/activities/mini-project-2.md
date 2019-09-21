---
title: "Mini-Project 2: UI Toolkits in Use"
type: activities
cover: "https://source.unsplash.com/k39RGHmLoV8"
---
import Subpage from "../../components/subpage.js"

<Subpage slug="overall">

### Overview

This project gives you the chance to practice building or working with a design system. You can choose between creating your own or implementing an existing one. Either way you must use best practices covered in course so far, use Github, and end up with a project worthy of including in your portfolio.

</Subpage>
<Subpage slug="build">

### Option 1: Build Your Own

Given what you've learned about design systems and the Fabricator framework, plan and build a small UI toolkit for a site.

- You may select any topic for your context; you may choose to base this on a previous project, design something new, or create one for an existing site. Either way you must still complete each of the steps below.
- You will create mockups in Sketch first in order to think through the colors, fonts, grid system, and a small set of components for the toolkit.
- You must build a toolkit in Fabricator that includes the following (based on your mockups of the same):
  * Grid system (columns and baseline grid)
  * Color system
  * Type styles (headings, paragraphs, lists, quotes, other site-specific needs)
  * Button and hyperlink styles including normal, hover, and focus states
  * At least four additional distinct components or structures based on the needs of the site, such as masthead and footer, page banners, navigation bars, lockups, side-by-sides, etc.
- You must show these components in use in two separate demonstration pages within the system as demonstrated in course content. These must feel complete and purposeful.

Use this schedule to complete this project:

#### Week 1

Choose a topic and wireframe two sample pages from the site or application. Use these to plan the requirements listed above. Complete at least your colors, grid, and typography in a Sketch mockup and sync to an InVision project for input from your professor. Be meticulous with details and consistent in your implementation of these elements.

#### Week 2

Finish the remaining components in your mockups and sync them to InVision. Then create a Github repo and set up Fabricator. Ensure that you have your colors and type set up in Fabricator by the end of the week. Substeps include:
  - Set up the repo with a `master` (default) and a `develop` branch.
  - Complete your work on the `develop` branch or on feature branches that you merge into `develop` on your own.
  - At the end of this week create a Pull Request to merge your work from `develop` into `master` so that your professor can use this to review your work for the week. This means you should create the PR, "assign" your professor as a reviewer, **and then wait for feedback before merging the code into `master`.** Your professor will provide feedback in the form of comments and may indicate "Approval" or "Request Changes" on the PR.

#### Week 3

Continue to build out your mocked up components in Fabricator and create your two demonstration pages.
  - After feedback from your professor, apply and changes requested and then merge last week's work into `master` and close the Week 2 PR.
  - Continue your work on `develop` or feature branches that you merge into `develop` on your won.
  - When finished, create a final PR to merge your final work from `develop` into `master`. As before, add your professor as a reviewer and wait for approval before merging.

</Subpage>
<Subpage slug="use">

### Option 2: Use Another

UI Toolkits have been around in a variety of shapes and forms for quite some time. [Bootstrap](https://getbootstrap.com/) is one such example; it is a library of CSS that aims to be generally unstyled (or at least easy for you to customize) but provides a robust set of common components, type styles, form styles, and grid structure to implement. Other examples include [Foundation](https://foundation.zurb.com/), Gumby, and the more opinionated [Materialize](https://materializecss.com/).

With this option you can choose one of these frameworks, or any other robust design system toolkit with which to build a small website or simulated web application. You must propose the topic and content of the site, create high fidelity wireframes of the intended site, and then build them using the system. As a set of minimum requirements this project must:

- Include at least four complete pages, with any other pages set up as a functional if limited "content coming soon" temporary page.
- Implement the chosen design system smoothly and coherently
- Be placed on Github and use best practices to track changes
- Be worthy of included in your portfolio for job interviews

Use this schedule to complete this project:

#### Week 1

Propose design system and submit complete, detailed wireframes for your site or application. These should not use color or final graphics but must include complete and detailed content. This way this acts as a blueprint upon which you will lay your selected design system.

#### Week 2

Begin to build your site out using HTML and the simple starter structure on Github (with or without Sass depending on your chosen design system). As a benchmark, aim to have all your site pages stubbed in (working navigation with at least a "content coming soon" message on each page of the site or application), configure your chosen design system, and complete at least one of the pages in full.
  - Set up the repo with a `master` (default) and a `develop` branch.
  - Complete your work on the `develop` branch or on feature branches that you merge into `develop` on your own.
  - At the end of this week create a Pull Request to merge your work from `develop` into `master` so that your professor can use this to review your work for the week. This means you should create the PR, "assign" your professor as a reviewer, **and then wait for feedback before merging the code into `master`.** Your professor will provide feedback in the form of comments and may indicate "Approval" or "Request Changes" on the PR.

#### Week 3

Continue your work implementing the content of your other three required minimum pages using the design system and minimal additional styling.
  - After feedback from your professor, apply and changes requested and then merge last week's work into `master` and close the Week 2 PR.
  - Continue your work on `develop` or feature branches that you merge into `develop` on your won.
  - When finished, create a final PR to merge your final work from `develop` into `master`. As before, add your professor as a reviewer and wait for approval before merging.

</Subpage>

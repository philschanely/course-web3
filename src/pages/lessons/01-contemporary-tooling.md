---
title: "Contemporary Tooling"
number: 1
type: lessons
cover: "https://source.unsplash.com/L94dWXNKwrY"
---
import { Subpage, Callout } from "../../course-components";

<Subpage slug="intro">

### Introduction

Its time. You've arrived. You're now in a class composed of folks who are serious about working on the web in some capacity. In this lesson we'll gear up with some contemporary tooling including:

- Atom for editing project code
- Terminal for running simple automated scripts
- Git and Github for tracking changes to our code.
- Sass for advanced CSS operations

</Subpage>
<Subpage slug="local-setup">

### Local Setup

This course may (or may not) be the first time you work directly on your own computer for your web projects. So first we'll get some folders set up and then install some tools to get rolling.

#### Working Directory

I highly recommend that you get in the habit of using the `Sites` folder as the main directory in which you store your various web projects. This is a folder that you can find (or create if one is not already there) in your user root folder on your Mac. Follow these steps:

1. Open Finder
2. Select View > Show Path Bar. This turns on a bar at the bottom of the Finder window that shows where you are in your computer's directory tree.
3. Double-click on the point in this path bar where your username appears. It is likely after the `Users` folder.
4. Look in this folder for a `Sites` folder. If one does not exist, right-click and choose New Folder, then name it "Sites" (case-sensitive).
5. Make this "Sites" folder easy to get to by dragging it to the Finder sidebar under the "Favorites" heading.

For any project you set up in this class, place the project's root folder in this "Sites" folder or somewhere organized inside it. I have main folders for my full time job, my freelance work, and a "Sandbox" folder for various experiment projects.

<Callout color="alternate">

Video demonstration coming soon!

</Callout>

#### Install Atom

Install [download Atom](https://atom.io/) to use for editing your project code.

<Callout color="alternate">

Video introduction coming soon!

</Callout>

Atom is an open source tool that has many developers contributing to it, including building neat plugins to enhance its core functionality. Consider installing the following plugins:

- `atom-beautify`
- `emmet`
- `editorconfig`
- `pigments`
- `minimap`
- `minimap-find-and-replace`
- `minimap-git-diff`
- `minimap-pigmenst`
- `platformio-ide-terminal`

</Subpage>
<Subpage slug="terminal">

### Basic Command Line

Now its time to talk about something that you might have heard of, seen, or even dabbled with---but not necessarily knowing why. What is this? The Terminal.

#### What is the Terminal?

Terminal, command line, shell---these are all vernacular names for this thing that looks like a really old computer. One where you type in commands, press return and hope you didn't just instruct your computer to blow up.

But don't worry; it doesn't have to be quite so scary or elusive. As hinted above, Terminal is a tool for executing commands in your computer system. These can be very simple commands that allow you to simply browse folders like you do in Finder, or alias commands that call up much more complex operations on your computer.

For the purposes you might use as a designer or front end developer the most common use for the Terminal is to run commands that help us develop locally. We'll dive into this later in the lesson, but as we get started it will be important to learn how to navigate around with the the Terminal...

#### Basic Terminal Commands

One thing to always be aware of in terminal is _where_ you are in directory tree so that you are executing commands in the right place. The basic idea here is that when you are in terminal you are always situated in a particular folder. You can tell where you are by looking at the terminal prompt line. Generally it should follow this format:

```
Computer-name:Folder username$ _
```

* `Computer-name` -- This is the name of the machine you're working on
* `Folder` -- this is the name of the folder you're currently in
* `username$` -- the username of the current user---you!

You can also "see" where you are by using the following commands:

* `pwd` -- prints the full path to the current working directory.
* `ls` -- shows the list of contents in the current folder.

You can move around between folders using the following command:

```
cd path
```

This is short for "change directory" and you just replace `path` with a relative path. So if you are in the `Sites` folder and want to move into a folder called `my-first-project` just type:

```
cd my-first-project
```

Or to move out of a folder just type:

```
cd ../
```

You can also enter long paths to move deeper at once:

```
cd my-first-project/src/images
```

Finally, navigate from the root folder for your user by starting the path with `~/`.

<Callout color="secondary">

**Pro tip:** You can bypass many of these commands on a Mac by Right-clicking on a folder from within Finder and choosing `New Terminal at Folder`.

</Callout>

<Callout color="alternate">

Video demonstration coming soon!

</Callout>

So, add to your list of possible research topics during this project the idea of learning some basic command line operations. One such set of operations is know as Git and its up next!

</Subpage>
<Subpage slug="git">

### Version Control and Source tracking

So by now you've probably heard of Github and might even have poked around there. Maybe you were even tickled by the [Octocat maskot](https://octodex.github.com/)!

_Git_ is a command line **technology** that allows us to keep track of changes we make to our code. _Github_ is a **platform powered by Git** that allows you to have a central location for your project.

Watch this video for a visual demonstration of the ideas behind these technologies:

<iframe width="560" height="315" src="https://www.youtube.com/embed/w3jLJU7DT5E" frameborder="0" allowfullscreen></iframe>

Here are some additional overall points:

- Project containers are called "repositories" or **"repos"** for short. We will create a repo for each of our projects and use this to house all the code and supporting assets for the project. You can create repos directly on Github and then clone them onto your computer, or you can create them locally first and later push them up to Github. We'll talk about this more later with Github Desktop.
- When you make a substantive change or set of changes to your code base you make a **"commit"** that captures the changes along with your username, the date, and a universal reference that allows you to look at the files and lines within each file that you changed. This allows us to both see the changes easily as well as to navigate between the changes, such as if we wanted to revert to an earlier state or recover some previous code.
- We make our commits on onto threads or **"branches."** This allows us to work on a series of changes in isolation so that we don't change things for others before they're ready.
- When we are ready to bring our changes over for others, we **"merge"** our branch into another branch in some fashion. This allows us to compare all the changes we committed on our branch with the code on the other branch and reconcile any differences.
- When we want to merge work from one branch into another we do this formally through Github using a feature called **"Pull requests" or a "PR"** for short. This is a courteous way of announcing to your team that you have changes you'd like to bring into a branch, and invites their review. Its also a formal way to capture the complete set of changes you've made on a branch to compare them against the original work before you merge the two.

Here is a visual illustration of these terms: [Github Flow](https://guides.github.com/introduction/flow/)

#### Getting Started with Git and Github

Complete the following steps to get your feet wet with Github:

1. Create a free account with Github and customize your profile.
2. Create a `sandbox` repo to test out how Github works. Use [this guide](https://guides.github.com/activities/hello-world/) to see how you can do a lot online directly in Github including code editing.

But thanks to Git itself we can also clone a Github repo and work on it on our own computer. Even better, we can use a graphical tool such as Github Desktop to handle the git stuff.

4. Download [Github Desktop](https://desktop.github.com/) to use as a graphical interface for committing.
5. Clone your `sandbox` repo using Github Desktop being sure to note where you place the repo on your computer (ideally wihin your "Site" folder).

Now you can work on your own computer, commit your changes, and push them to Github to share with others or even to set up deployment.

<Callout color="alternate">

Video demonstration coming soon!

</Callout>

#### Gitflow: A Process and Branching Convention

Not to be confused with the name of the link above, Gitflow is a common convention for working with branches and it goes like this:

- `master` is the primary branch where the tested, stable code is placed that is ready for the world to see. A typical repo on Github starts with this branch as the default branch, and many folks just do all their work right there on the master branch. But making another branch essential creates an isolated copy of the code based on all the commits up to that point on the initial branch, so it can be nice to "fork" off onto a separate branch when you're building new features.
- A convention that has arisen for this is to create a `develop` branch distinct from `master` that is where active development is happening. When work here is stable and ready to release to the world, we bring those changes over to `master` using a merge that represents a "release" of new versions of the code base. But we keep `develop` going and continue to make improvements, new features, and bug fixes there until they're ready to release again to master, and so on and so forth.. However, we usually don't work _directly_ on `master` or `develop`. Instead...
- Feature branches are small branches off of `develop` where one or more users works on an isolated set of features, improvements, or bug fixes. So we branch from `develop` and name the branch after whatever we're working on. We add commits to that branch until we're finished. Then we look to merge our feature branch into `develop`. This way our new features can be tested in `develop` to ensure everything works well before finally merging into `master` for the world to see. Branches are typically named using `kabob-casing` and it is a good practice to make them specific even if long.

For your research, consider diving into this more with this article on [Git flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow). Note that this article covers the actual terminal commands used for Git, but you won't generally need to know these as we'll use a graphical user interface (GUI) later called Github Desktop.

Later we'll talk about the topic of deployment, but, in short now as a preview, Deployment is when we publish the work from a given branch to an actual web server where it can be seen by the world. We often tie the master branch to a full public deployment: through a technique called "continuous integration" or CI, changes made to a branch can automatically deploy to the live webserver. Its a little scary, and a little magical, but its super helpful and clean. Separating our work onto `master` and `develop` braches helps take some of the scariness out of this, so that we have the chance to test the integrated work on `develop` before we take it "live" on `master`. Sometimes we also tie a "staging" deployment to `develop` so that we can test the work there in a very similar web server environment.

So when you set up a new repo, you are given a `master` branch by default. But don't work on it! Instead, create a `develop` branch. On solo projects you can work right there on `develop` until you're ready to merge your work into `master` as a release. But on large or collaborative projects, add new work by first creating a feature branch off of `develop`. We'll gain some experience with merging through PRs in the first mini-project.

<Callout color="alternate">

Video demonstration coming soon!

</Callout>

#### Learn Git

So all this talk of repos, commits and branches goes back to the version control technology called Git. While there are other similar technologies, this is by far the most commonly used one. So for your research component on this upcoming project you could consider using one or more of the following resources to dig deeper with Git:

* the quick and easy [try Git by CodeSchool](https://try.github.io/)
* the more in depth [free Udacity course on Version Control with Git](https://classroom.udacity.com/courses/ud123). And don't worry... the timeblocks shown on each module there is only an estimate, and by my experience a gross overestimate.
* [Git for Humans](https://learning.oreilly.com/library/view/git-for-humans/9781492017875/) from A Book Apart, available on Safari Tech Books.

Bottom line here for Git is threefold:

1. You need to be familiar with the concepts of version control: using a repo to manage commits for any given project.
2. You need to be able to set up a repo and make your own commits, and Github is a fine place to do this.
3. You should be able to clone an existing repo for the times when such a repo provides a nice starting point for a project you're working on.

</Subpage>
<Subpage slug="local-development">

### Local Development

As we now start to develop locally this can be rather simple:

1. Ensure your project files are all contained inside a single root folder on your hard drive.
2. Open a browser such as Chrome and then use the browser to open a file in your site such as your home page.
3. Make changes to the site files in Atom and save the file.
4. Switch back to your browser and refresh to see the changes.

This is the process I used for years. Its simple and it works.

But today we have some better options. With just a little configuration we can both improve our project's share-ability to other developers and improve our development experience.

#### Install NodeJS

First, install [NodeJS](https://nodejs.org/en/) (LTS Options is fine), a development helpful JavaScript-based development tool. We could spend a whole course just on NodeJS as it has become a key tool to be used by developers today.

A key feature that comes with NodeJS is called Node Package Manager or NPM. This tool makes it easy for us to add other libraries to our projects such as jQuery or Bootstrap from the worldwide library of "packages."

#### Simple Starter for Local Development

Among this huge library of tools I've selected a few to help us organize our projects and run development commands.

Read the first portion of this [Simple Starter](https://gist.github.com/philschanely/cd70aac7d6a4a16d09fcfdc3b7e53916) for setting up local development using some helpful NPM tools.

<Callout color="alternate">

Video demonstrations coming soon!

</Callout>

</Subpage>
<Subpage slug="sass">

### CSS Preprocessing with Sass

Now its time to take your CSS skills to a new level. However, I don't mean that we're going to talk about new CSS properties or techniques per se. What we're going to discuss next is how we can become more efficient and organized thanks to a technology known as CSS Preprocessing.

Take a look at the [Sass](http://sass-lang.com/) main webpage. Without diving into any subpages, what would you guess this technology does?

Hopefully you caught the key idea that SASS is a "CSS extension". Sass is just one of several other options for this same idea ([LESS](http://lesscss.org/) is another of the prominent ones). But what does that mean?

Read more from the [Sass Basics tutorial](http://sass-lang.com/guide).

For your own sites, review the Sass-related sections of the [Simple Starter instructions](https://gist.github.com/philschanely/cd70aac7d6a4a16d09fcfdc3b7e53916) for setting up local development using some helpful NPM tools.

<Callout color="alternate">

Video demonstrations coming soon!

</Callout>

</Subpage>

---
layout: lesson
title:  "1: Github and CSS Preprocessing"
---

### Basic Command Line

Its time. You've arrived. You're now in a class composed of folks who are serious about working on the web in some capacity. And now its time to talk about something that you might have heard of, seen, or even dabbled with---but not necessarily knowing why. What is this? The Terminal.

What is the Terminal?

Terminal, command line, shell---these are all vernacular names for this thing that looks like a really old computer. One where you type in commands, press return and hope you didn't just instruct your computer to blow up.

But don't worry; it doesn't have to be quite so scary or elusive. As hinted above, Terminal is a tool for executing commands in your computer system. These can be very simple commands that allow you to simply browser folders like you do in Finder, or alias commands that call up much more complex operations on your computer.

For the purposes you might use as a designer or front end developer, the terminal is used for several semi-regular abilities:

1. To manage version control or source code tracking. We'll look at this soon, but this is basically working with Git and Github to keep track of changes you and your team members are making to files on a project. Its really amazing and very useful. Learn about 8 statement. It benefits you to know about these abilities, but there are also some nice graphical tools we can use for this as well.
2. To quickly add common frameworks or libraries to your projects, such as adding jQuery, Bootstrap, Materialize, or any number of other such tools. These are hosted and serviced through a number of platforms such as Bower, NPM, and Yarn as well as simply cloning a repository from Github. I know that was a lot of terms you don't know, but Terminal commands basically give us quick access to things we might otherwise browse the web to find, then manually download, move into our site folder, etc. We'll look specifically at Bower and NPM in this course.
3. To execute shortcut commands as a part of some of the libraries you added thanks to the previous step. One such example is to use a library called `browser-sync` to automagically refresh your web browser as you work on a project. You might have used Brackets before and its feature called Live Preview. This is similar, but somewhat limited in comparison to tools that become available if we learn a little command line.

So, add to your list of potential research topics during this project the idea of learning some basic command line operations. Thankfully, as we start with Git in the next section, most resources that teach Git also go over or link to some good basic command line resources.

### Git and Github

So now you've probably heard of Github and might even have poked around there. Maybe you were even tickled by the [Octocat maskot](https://octodex.github.com/) while you were there!

Regardless, Github is a crucial tool to add to your arsenal of tools and working with Git is a skill you should possess. Indeed, Git is something separate from Github. They both have to do with Version Control, or tracking different versions of code and files in a project.

So add learning Git and Github to your list of research topics. Consider completing the quick and easy [try Git by CodeSchool](https://try.github.io/) or the more in depth [free Udacity course on Version Control with Git](https://classroom.udacity.com/courses/ud123). And don't worry... the timeblocks shown on each module there is only an estimate, and by my experience a gross overestimate.

Bottom line here for Git is threefold:

1. You need to be familiar with the concepts of version control: using a repo to manage commits for any given project.
2. You need to be able to set up a repo and make your own commits.
3. You should be able to clone an existing repo for the times when such a repo provides a nice starting point for a project you're working on.

So what about Github? As was mentioned in the Udacity course above, Github is an online service that allows us to host Git repositories so we can share them with colleagues and the world.

Check out this nice big picture look at Github:

<iframe width="560" height="315" src="https://www.youtube.com/embed/w3jLJU7DT5E" frameborder="0" allowfullscreen></iframe>

Thanks to Github we can show our code to potential employers, and host projects we're working on so that other team members can access our work, and so we can reconcile our changes safely.

I've learned a lot about how this looks and works in my first few months on the job and will post a video soon to show you more.

But for now, complete the following steps:

1. Create a free account with Github and customize your profile.
2. Create a sandbox repo to test out how Github works. Use [this guide](https://guides.github.com/activities/hello-world/) to see how you can do a lot online directly in Github including code editing.
3. Read this overview of the [Github Flow](https://guides.github.com/introduction/flow/) for a visual illustration of branching, committing on a branch, opening a pull request, discussing, and merging.

But thanks to Git itself we can also clone a Github repo and work on it on our own computer. Even better, we can use a graphical tool such as Github Desktop to handle the git stuff.

4. Download Github Desktop to use as a graphical interface for committing.
5. Clone your sandbox repo using Github Desktop being sure to note where you place the repo. I like to use the Sites folder directly under my user folder on my Mac (peer to Documents and Downloads).

Before we do any work locally its wise to create a branch for that work.

6. In Github Desktop choose Branches > New Branch and create a new branch called `Develop` to use as a catch-all for work in progress commits.
7. Switch to this branch using the middle dropdown.
8. Make some changes to the local files and commit them on this branch using Github Desktop.

The commits we make locally don't automatically sync up to Github, so once we've made changes we can use `git push` to publish our commits to the repo on Github.

9. When ready, push the branch to the repo on Github using the rightmost "Push" option on the tool panel in Github Desktop.

If you look at your repo online in Github you should see your new branch and new commits.

10. Open a Pull request to look into merging it. This might feel silly without other people to discuss it with you. We'll use this moving forward for you to signal to me that you want feedback on your work in progress.
11. Merge the pull request after resolving any conflicts (if applicable).

OK. Now you're ready for a serious project!

### CSS Preprocessing with SASS

Details coming soon!

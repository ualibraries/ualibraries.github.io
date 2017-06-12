---
title: Reviving Our Continous Integration Environment 
---

We're committed to delivering the most reliable websites, software, and services 
possible.  That's why we've chosen to make continuous integration a priority 
for our technical infrastructure.  Continuous integration is a software development 
practice that helps developers catch problems early by requiring them to 
merge their code into a shared environment, called a CI (continuous integration) 
server, that runs automated tests.  The server will report any problems back 
to the developer so they can fix the problem before deploying the code to 
production.

We've used CI for many years, but lately we noticed that there were a lot of 
issues with our system.  It was prone to breaking and time consuming to fix.
We needed to revive our continuous integration environment to make it more useful
to our developers and in turn make our products better. 

The first step was to upgrade our installation of [Jenkins](https://jenkins.io/), the open source
software that we use to automate building and testing our code.  After that, we
worked on integrating Jenkins with other services.  We really wanted to be able 
to use [UA NetID](https://netid.arizona.edu/) to log in to the Jenkins admin interface, so we set up the
[Jenkins CAS Plugin](https://plugins.jenkins.io/cas-plugin) to talk to WebAuth to make authentication a breeze.  Next, we
focused on improving the integration between Jenkins and [Slack](https://slack.com/), a
handy chat app we use for a lot of our communication.  We were able to set up
Slack so that it would notify developers when the tests failed and were even
able to tag specific users so that they would get phone alerts when there was
a problem.  The result is that we're faster than even when responding to bugs
or service outages.

The most fragile part of our CI environment was our use of [Selenium]( http://www.seleniumhq.org/).
Selenium is a browser automation tool that simulates how a user interacts with
a website.  Although it can be very useful, it's also very picky about which
browser version you're using.  We often had problems where our Selenium-based
tests wouldn't work because they required specific versions of Firefox that
were no longer installed due to automatic updates.

Thankfully, [Docker](https://www.docker.com/) provided an excellent solution to this problem.  Docker
is a containerization tool that allows us to run system processes in an isolated
environment.  This means that we're able to run Selenium with the correct version
of Firefox without having to worry about automated updates breaking things.

These improvements to our CI environment have already paid off by saving us time
and catching bugs before they can affect our users.  We hope to continuously 
improve our continuous integration environment to give our users the best experience
possible!


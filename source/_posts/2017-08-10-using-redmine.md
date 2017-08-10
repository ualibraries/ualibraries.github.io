---
title: Using Redmine
---

Having shared documentation to record decisions, work happening, and research notes is essential for everyone involved in the work to collaborate effectively. No matter what tool you use, this kind of documentation can improve communication, inform coordination of efforts, and keep everyone on the same page.

During a project, we can

- Track the status of a project
- Remember all the tasks and to-dos related to that project
- Categorize wishlist features
- Access any code written for the project (and see which ticket it was written for)
- Send new contributors to see rationale behind previous decisions

After a project, this kind of documentation

- Provides access to all the conversation related to an issue or decision
- Gives future code or product maintainers one source for relevant documentation
- Exposes the changes that happened in the code during the project
- Shows when work happened, when work tasks became part of the project, and when they moved from one stage to the next to completion

One tool we use for this kind of communication and documentation, especially for work happening close to the code, is Redmine, an open-source project management tool. While Redmine is oriented toward software development, it's flexible, and since we have our own internal installation, we can modify it to fit our needs. After developers started using it a few years ago, others in our organization started using it too, so now we use it to track all kinds of things - from support requests and bugs to big dreams and rough ideas.

Here are a few of the things we appreciate about Redmine:

- You can get to it from everywhere. (even your phone!)
- The information lives in the web browser - there's nothing to install.
- It supports reference and conversation directly aroun the code for a project.
- We can work on it. It's our install and it's open-source.
- In our organization, we're used to communicating by email. Redmine's email integration lets you stay up to date in your inbox without visiting the application.
- Conversations can continue in email without fragmenting the communication. This is because cc-ing Redmine lets all the conversation be documented on the issue. 

Everyone involved with the work can get up-to-speed on what has happened so far, future contributors have access to work and decisions affecting the product, and the answer to an important question about the work won't end up trapped in one person's inbox.

## Access and permissions

If you're a library employee (or a guest who has been granted access), visit redmine.library.arizona.edu and sign in with your NetID to see all the projects, issues, and documentation.

Redmine differentiates between members who are working on a project and non-members who may be providing feedback or contributing to the project as part of a different workflow. If you'd like to be added as a member on a project, ask one of the people listed as a Project Manager or Contributor on the project overview page.

Without being a member of a project, you'll be able to:

- View issues, code, and documentation in the wiki
- Comment on and watch any issues you're interested in
- Besides being able to do what non-members can do, members can also:

If you are a member on a project, you can also:

- Create, move, categorize, reassign, and otherwise modify issues
- Commit code
- Make and edit wiki pages

Redmine admins can also:

- Create and modify trackers and workflows
- Manage user accounts
- Delete stuff

## Keeping up to date

### In the web interface

Redmine's interface is a place to find work that has already happened, that has been planned, and that's in progress, as well as a place to explore technical documentation and code associated with the project. We tend to use Redmine's 'project' structure to group issues by product, but it can also be used to organize work that's taking place on many products.

Everything we do on a project - from a new feature to an old bug to a pie-in-the-sky daydream is an issue in Redmine. We add information to these issues to make sure our stuff is done and documented.

To find out what's been going on in a project, try the activity log. It shows every change that has been made in a project, including updates and comments on issues, wiki page changes, and code commits.

Redmine comes with a wiki at the project level. These can contain just about any kind of information. If you see a *wiki* tab in your navigation bar, it's the wiki for that project.

One of the things that makes Redmine different from other project management systems is its communication around the code related to a project. Specific commits can reference tickets to appear right next to the comments about an issue, and in this way all the changes that were made to resolve an issue are in one place. If there are code repositories associated with the project, they'll be visible under the "Repository" link.

When you're looking at an issue you're interested in, use the star to "watch" the ticket and get notified when there are changes.

## Email notifications

If you've authored, watched or been assigned an issue, you'll get an email anytime something changes. Don't worry, though, you're not obligated to get a ton of email - visit My Account and change the impact on your inbox anytime.  

Messages from Redmine come with a subject that will tell you the ticket number and the summary. The body of the message shows the original issue description along with any metadata that has changed on the issue. You can stay up to date on a ticket you're interested in without ever leaving your email client.

To see the issue in context, with the complete timeline of comments, metadata changes, and associated code since the ticket was created, use the linked issue number and title displayed in the body of the email. Once you're signed in, you'll go straight to the issue.

If you want to add your own comment without leaving your email, hit reply and type your response as the first part of the message. Make sure you don’t change the email subject! This will automatically update the ticket to include your message as a comment and email the people involved in the issue.

## Issue metadata
Some fields we use:

Tracker describes the type of ticket. Tasks are things to do, features are new things to build, and bugs are problems with the existing website or application. We've also used a decision tracker to identify discussions that result in decisions rather than code.
Summary is like the title of the ticket. We try to use as much descriptive information in this field as possible because it makes tickets easier to find later.
Status - new tickets are new/approved, proposed means that it's an idea and not necessarily a requirement to complete, if a ticket is declined it is either no longer valid or we've decided not to do it for some reason. Tickets can also be in feedback status, which usually means they need more discussion or a sign-off.
Assignee - the person who is responsible for making sure the ticket gets done. We don't assign tickets to groups or teams - one point person needs to make sure that the issue is addressed.
Category and Target version are two ways to group issues. Categories allow for grouping by type of activity or area of a website or application. Target versions are groupings by project milestone (or software release.) For the Redux project we use target versions for project milestones that have definite deliverables while activities that are ongoing are grouped with categories.
Start and Due dates allow for planning and scheduling work.
% done helps those working on the ticket to communicate with others how close the ticket is to being completed. Redmine's task-subtask structure can also use this information to show progress on complex issues.

Browse issue lists and save custom queries
All the metadata that is included on issues makes them easier to list and sort. Redmine's filter panel on the issues list can limit by almost any of the metadata on issues or even on projects.

Use the filters to build a list of tickets and choose Save to keep your query. You're the only one who can see your custom queries which will display in a list at the right of the issue list and also the calendar. To make changes later, view your query and choose Edit.

If the tickets in a project have start or due dates, Redmine will display them in a calendar view. Custom queries work in the calendar display, so you can look at the subset of issues you're interested in.

The roadmap shows all open versions.

We tend to use versions more like project milestones that describe our progress, but these are not set in stone at the start of a project. Redmine supports our workflow as things versions grow, issues change, and the work we need to do becomes more clear. 


We heart Redmine.
Redmine was a pilot that stuck. It has helped us keep track of quite a few websites and applications over the years, and we’re working on making it even more useful. Please let us know if you have questions about how Redux is using Redmine. We're here if you need help!


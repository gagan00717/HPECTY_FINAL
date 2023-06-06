
## Blockly




Google's Blockly is a library that adds a visual code editor to web and mobile apps. The Blockly editor uses interlocking, graphical blocks to represent code concepts like variables, logical expressions, loops, and more. It allows users to apply programming principles without having to worry about syntax or the intimidation of a blinking cursor on the command line. All code is free and open source.



# Getting Started with Blockly


Blockly has many resources for learning how to use the library. Start at our Google Developers Site to read the documentation on how to get started, configure Blockly, and integrate it into your application. The developers site also contains links to:

# Installing Blockly



Blockly is available on npm.

'npm install blockly'



We now have a beta release on npm. If you'd like to test the upcoming release, or try out a not-yet-released new API, you can use the beta channel with:

'npm install blockly@beta'



# Branches
There are two main branches for Blockly.

master - This is the (mostly) stable current release of Blockly.

develop - This is where most of our work happens. Pull requests should always be made against develop. This branch will generally be usable, but may be less stable than the master branch. Once something is in develop we expect it to merge to master in the next release.

other branches: - Larger changes may have their own branches until they are good enough for people to try out. These will be developed separately until we think they are almost ready for release. These branches typically get merged into develop immediately after a release to allow extra time for testing.

#New APIs
Once a new API is merged into master it is considered beta until the following release. We generally try to avoid changing an API after it has been merged to master, but sometimes we need to make changes after seeing how an API is used. If an API has been around for at least two releases we'll do our best to avoid breaking it.

Unreleased APIs may change radically. Anything that is in develop but not master is subject to change without warning.

Issues and Milestones
We typically triage all bugs within 2 working days, which includes adding any appropriate labels and assigning it to a milestone. Please keep in mind, we are a small team so even feature requests that everyone agrees on may not be prioritized.

# Milestones

Upcoming release - The upcoming release milestone is for all bugs we plan on fixing before the next release. This typically has the form of year_quarter_release (such as 2019_q2_release). Some bugs will be added to this release when they are triaged, others may be added closer to a release.

Bug Bash Backlog - These are bugs that we're still prioritizing. They haven't been added to a specific release yet, but we'll consider them for each release depending on relative priority and available time.

Icebox - These are bugs that we do not intend to spend time on. They are either too much work or minor enough that we don't expect them to ever take priority. We are still happy to accept pull requests for these bugs.

Good to Know
Cross-browser Testing Platform and Open Source <3 Provided by Sauce Labs
We test browsers using BrowserStack












# JSON Forms React seed App

This seed demonstrates how to use [JSON Forms](https://jsonforms.io) with React in order to render a simple form for displaying a task entity.

It is based on `create-react-app` and only contains minor modifications.

- Execute `npm ci` to install the prerequisites. If you want to have the latest released versions use `npm install`.
- Execute `npm start` to start the application.

Browse to http://localhost:3000 to see the application in action.

## File Structure

Let's briefly have a look at the most important files:

- `src/schema.json` contains the JSON schema (also referred to as 'data schema')
- `src/uischema.json` contains the UI schema
- `src/index.tsx` is the entry point of the application. We also customize the Material UI theme to give each control more space.
- `src/App.tsx` is the main app component and makes use of the `JsonForms` component in order to render a form.

The [data schema](src/schema.json) defines the structure of a Task: it contains attributes such as title, description, due date and so on.

The [corresponding UI schema](src/uischema.json) specifies controls for each property and puts them into a vertical layout that in turn contains two horizontal layouts.

## Rendering JSON Forms

JSON Forms is rendered by importing and using the `JsonForms` component and directly handing over the `schema`, `uischema`, `data`, `renderer` and `cell` props. We listen to changes in the form via the `onChange` callback.

## Custom renderers

Please see [our corresponding tutorial](https://jsonforms.io/docs/tutorial) on how to add custom renderers.

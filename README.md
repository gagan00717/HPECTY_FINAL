#  Project: 
Purpose: Log Message Knowledge Base Builder on ProLiant Servers

# Getting Started

Aim of this project is to create an interface where users can create forms and    include the fields they want from a collection which can be used to take input about various log messages, their characteristics, error resolving techniques, etc. The forms have to be user-friendly and should be easy to generate by users who may not have technical skills to write the code from scratch.
Technologies such as Google Blockly, JSON Forms, React.js are to be used. Tools are to be developed to enable the automation of file generation and deployment of the package.



This seed demonstrates how to use  the app 


- Execute `npm ci` to install the prerequisites. If you want to have the latest released versions use `npm install`.
- Execute `npm start` to start the application.

Browse to http://localhost:3000 to see the application in action.


you can find the deployment here : https://hpecty-final.vercel.app/



## Technicality used 

## Blockly




Google's Blockly is a library that adds a visual code editor to web and mobile apps. The Blockly editor uses interlocking, graphical blocks to represent code concepts like variables, logical expressions, loops, and more. It allows users to apply programming principles without having to worry about syntax or the intimidation of a blinking cursor on the command line. All code is free and open source.



# Getting Started with Blockly


Blockly has many resources for learning how to use the library. Start at our Google Developers Site to read the documentation on how to get started, configure Blockly, and integrate it into your application. The developers site also contains links to:

# Installing Blockly



Blockly is available on npm.

`npm install blockly`



We now have a beta release on npm. If you'd like to test the upcoming release, or try out a not-yet-released new API, you can use the beta channel with:

`npm install blockly@beta`









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


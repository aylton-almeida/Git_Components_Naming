# Git Components Naming

Git Components Naming is a guide on how to structure and name the components of your git repositories

## Features

  * [Folders](#folders)
  * [Branchs](#branchs)
  * [Commits](#commits)

## <span id="folders">Folders</span>

Each project has its specific folders structure, but there are some most commonly found, and here is a quick description with their function.

  src - The source folder contains the main code of your application

  assets - The assets folder contains all files that have some kind of value for your app

  lib - The libraries folder contains third party-code that will be used in our application

  vendors - The vendors folder contains third party files, like images and fonts or something bigger than a library, like a framework

  test - The test folder contains unit test for functions inside your code
  
  utils - The utils folder contains files with code used in several different files
  
  components - The components folder contains parts of your app, usually used with tools such as ReactJs and Angular 

All these folders are just sugestions and should be used as needed in each project, there is no exact rule on how they should be implemented

## <span id="branchs">Branchs</span>

For now use GitFlow, those guys know what they are doing. Here is a quick summary:

Master: branch with production level code

Develop: branch with preparatory code for the next deploy

feature/*: branchs containing a new feature for the project. Ex: feature/login

hotfix/*: branches focused on correcting bugs that were found at the production level. They are named based on the next version where they'll be released. Ex: hotfix/2.3.1

release/*: branches containing code with higher reliability than the develop branch. Named based on the version where they'll be released. Ex:release/1.5.3

## <span id="commits">Commits</span>

Each commit should use at least two of the following strucutre components, and as many strctures as needed: object[mode]{Description}

The **object** should be a file, folder or version, being significative for the development team.

The **mode** tag represents which action was taken with the object in question and should be surrounded with **brackets**, you should use as many tags as necessary, below are some tag examples:

* [+] - Added object
* [~] - Modified object
* [^] - Ugraded object
* [.] - Finished object 

The **description** should be a quick text with important information not mentioned above, it should be surrounded with **braces**.

Below are some examples:

project[+]  - Project has been created

assets[+]index[~]{modified page title} - Folder "assets" was created and the index page was modified

## Authors

* [Aylton Almeida](https://github.com/stevreeper)



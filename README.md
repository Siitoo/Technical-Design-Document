﻿# Technical Design Document (TDD)

I am [Alfonso Sanchez-Cortes](https://github.com/Siitoo), student of the [Bachelor’s Degree in
Video Games by UPC at CITM](https://www.citm.upc.edu/ing/estudis/graus-videojocs/). This content is generated for the second year’s
subject Project 2, under supervision of lecturer [Ricard Pillosu](<https://es.linkedin.com/in/ricardpillosu>).

## ¿What's a TDD?

The technical design document, usually written by the technical director or the programming leader in the pre-production phase,contains a technical description of the production of a game.
It includes details of all the software, hardware and game engine components that will be used during production, and what those particular tools will provide to the development team,
and includes a brief description of how the code will be written. The document is updated in different stages of the production of the game. It often comes and goes between the editor
and the developer as the technical details are better defined. For that reason, there is a box on the first page of the document that describes the changes made to the file and who made the changes.

In summary, TDD is a statement of the solution to a specific game concept outlined in a “Game Design Document” (GDD) and discusses things such as the following:  

*Coding standards  

*Technical design  

*Tool instructions  

### Coding standards

Documentation on the coding standards includes specifics on coding conventions, hardwares and software specifications, naming conventions, technologies used(including middleware), file types, data layout, and any other technical information that is necessary for developing the game. 
The documentation should also provide an overview of what all the functions and data do, and how they interact with each other.

#### Coding conventions

Set of guidelines for a specific programming language, in the TDD we will establish what conventions we use and what we do not, these rules will be respected throughout the development.  

See [coding conventions c++](http://geosoft.no/development/cppstyle.html).  

#### Programming Style

With the objective that all the programmers of the project use the same style to facilitate the reading of the code, rules will be defined to create a style for all. For example:

![conventions](/docs/conventions.jpg)

#### Hardware and software specifications

At this point we need to know all the technical specifications of the hardware and software with which we will work, example:  
  
*Numbers of CPUs  

*Total memory of each computer  

*Processor  

*All characteristics of GPU  

*Ram

#### Technologies used  

Of the technology that we are going to use in our project, for example the STL libraries, that we are going to use? Not? Will we use it through a .dll? Static or dynamic compilation?

#### File types

What types of files are we going to use?  

For images jpg, png, etc?  

For the UML?  

For the music and the sounds effects?  

For the documents? 

In this section we detail all the types of files that will be included in the development process, their extensions, their maximum capacity and their characteristics.

#### Data layout

In the previous section we have defined what types of files we are going to use and their characteristics, in this we will explain how the information is distributed in the data. How to save a game or how and where we keep our player's statistics.  
For example:  
![examplePlayerData](/docs/examplePdata.jpg)

#### UML structure

Defined all the above only remains to know how we are going to organize the code, its modules and its different factories (create entities, or GUI).
For this we will use UML structures, but there are different types:  

*[Class diagram](https://en.wikipedia.org/wiki/Class_diagram) 

*[Package diagram](https://en.wikipedia.org/wiki/Package_diagram)  

*[Object diagram](https://en.wikipedia.org/wiki/Object_diagram)  

*[Component diagram](https://en.wikipedia.org/wiki/Component_diagram)  

*[Composite structure diagram](https://en.wikipedia.org/wiki/Composite_structure_diagram) 

*[Deployment diagram](https://en.wikipedia.org/wiki/Deployment_diagram)

We normally use class diagram, object diagram and composite structure diagram.
A package diagram is a good idea to make an outline of how we will organize all the files(Resouce Management).

![classdiagram](/docs/classdiagram.jpg)
![objectdiagram](/docs/objectdiagram.jpg)

### Technical design

Technical design documentation is the counterpart to design documentation. The engineers will read through the design documents and provide technical information on how  the features will be coded for the game. This documentation is disseminated to the appropriate engineers on the team for implementation.
Tool instructions provide information on how to use the tools. 

![exampleTechDesign](/docs/exampleTechDesign.jpg)


### Tools Instructions

Tool instructions provide information on how to use the tools. For example, an engineer and designer will work together to document how the scripting tools work. 
These tool instructions must be updated when any changes are made to the tool functionality; otherwise, the documentation will quickly become unhelpful and even obsolete.
Taking an example of UI system:
(insert image and explication)

**Well, this is the basis, but we will discuss other important issues to be able to create a TDD.**

### Builds creation  

This point is quite important because if we do not know when we should get a version or like, the development will never end since you can always improve all the elements of the game.  
We must define when we release a version of our game and all the elements that must be in order to have a valid version.  
  
![releaseExample](/docs/releaseexample.jpg)

### Branches policy

We must define how we will work with the code throughout the development time, for this we will use the branch policies. You have to define specific branches in order to develop versions or change the current one without interrupting the rest of the team. The main branches are:  
  
*Master: release production.  

*Develop : work to next release.  

Supporting Branches:  

*Feature : feature for a distant future release.  

*Release: all features for next release are finished.  

*Hotfix: to solve critical error in master version.  
 
![branchesPolicy](/docs/branches.jpg)  

### Resource management

In the past we define what types of files we will use in the project and its characteristics, we also specify in which other types we keep the data and what they contain, so we just need to know where we keep these files, distributed in folders? With some specific order? If we keep it in folders, will these be compressed?
A very visual way to define this section would be the use of UML package diagram and deployment model

![branchesPolicy](/docs/packageModel.jpg)

### Analysis platform and performance budgets

To finish we will deal with the topics of platform analysis and performance budget in a simple way. On the part of the performance budgets we define the objective of FPS(frames per second) to which our game should go when we launch it to the market and how much time we spend as a maximum to the execution of different parts of the code (in ms) such as: logic, audio, graphics, etc.

![fpsTarget](/docs/fpsTarget.jpg) 

On the part of analysis platforms we will explain what tools we will use to achieve this objective and an explanation of how they work, as well as how and when these analyzes will be done.  

The image below shows the [Brofiler tool](http://www.brofiler.com/)  

![brofilerImage](/docs/brofilerImage.jpg)

**The purpose of this research is to know the elements that make up a TDD and how to create it, then we will explain step by step how to create a TDD and at the end we will show an example of an index of a TDD.**

## Creating a Technical Design Document  

1.Create a **document** with:  
  
	*Name of your game  

	*Name of your team(or company)  

	*Members of the group 

	*Current date(it will change every time you update it)  

	*TDD version number(he number of the version varies depending on how many times the document has been modified)  

2.Add a **table of contents** whit:

	*Introduction  

	*Technical Overview  

	*Game Mechanics  

	*Build Creation  
 
	*Resource Management and File Formats  

	*Tool Instructions  
  
3.We want to explain the game in a general way in **introduction** write:  

	*Purpose of your game  

	*Technical Goals  

	*Target Platform (hardware and software specifications)  

	*External Tools to develop  

	*Development Team  

	*Development Time  

	*Branches Policy  

 


 
 



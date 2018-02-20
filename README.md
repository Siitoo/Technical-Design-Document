# Technical Design Document (TDD)

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

### Technical design

Technical design documentation is the counterpart to design documentation. The engineers will read through the design documents and provide technical information on how  the features will be coded for the game. This documentation is disseminated to the appropriate engineers on the team for implementation.
Tool instructions provide information on how to use the tools. 

### Tools Instructions

Tool instructions provide information on how to use the tools. For example, an engineer and designer will work together to document how the scripting tools work. 
These tool instructions must be updated when any changes are made to the tool functionality; otherwise, the documentation will quickly become unhelpful and even obsolete.
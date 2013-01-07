#CustomBotConsole
* Authors: Kenshin Himura *(Sudarsan Balaji)*, Balakumar S, Yaswanth Kodavali
* License: *GNU GPL v3 and CC-BY-NC-SA Licenses* (see gpl.txt and ccbyncsa.txt)
* ReadMe Version: 1.2

##Description
This repository holds various project and project-related directories pertaining to our final year project. The main project directories are explained as below.

##customBotConsole
holds our coding and creation of a custom Console Application for Windows, using Microsoft Visual Studio 2012 Ultimate for Windows 8 (hereafter referred to as VS2012), built in C++, meant to handle a Pioneer-3AT mobile robot equipped with Sick LMS100, with a FOV of -135 to +135 degrees, providing a total of 541 readings per scan. ARIA library used with GNU GPL 2.0, with no modification of the source (as of now). ARIA's License, which becomes a mandatory license for this program also, can be found in LICENSE.txt.
###xInputTest
holds our console application built in C++ used for testing the xInput library and its usage for use in the customBotConsole application. This project is part of the customBotConsole's VS2012 solution. Implemented in the customBotConsole application.
###testParse2D
holds our console application built in C++ used for parsing the .2d files generated by the Laser Range Finder (LRF). Simply translates the .2d file into a more interpretable .2dparse file WITHOUT changing any of the values held by its parent file. Its (.2d file) format and other details were obtained from the ARIA documentation which truly deserves credit for clarity and user-friendliness. Also part of the customBotConsole solution in VS2012.
###changeToGlobal
is our initial attempt in C++ programming to convert the laser readings to global co-ordinates. We later formed the opinion that MATLAB R2012a/R2012b (hereafter referred to as MATLAB) is more suitable to handle the task, and thus started MATLAB coding for reading and processing the generated .2dparse file.
##2dParseReader
is the MATLAB project directory of the parser and processor of the .2dparse files generated by the testParse2d application. This is the currently active project and all new/modified code will be pushed here (as of now). A separate [ReadMe](https://github.com/kenshinthebattosai/customBotConsole/blob/master/2dParseReader/ReadMe.md) exists for this project to keep works on it updated, considering the scope of this MATLAB project.

##Updates and Stuff
* Created debug branches to push to master later, and to allow collaboration.
* Branch [debugKen](http://www.github.com/kenshinthebattosai/customBotConsole/tree/debugKen) branched from master for use by [kenshinthebattosai](http://www.github.com/kenshinthebattosai).
* Branch [debugBala](http://www.github.com/kenshinthebattosai/customBotConsole/tree/debugBala) branched from master for use by [balakumar-s](http://www.github.com/balakumar-s).
* Branch [debugYash](http://www.github.com/kenshinthebattosai/customBotConsole/tree/debugYash) branched from master for use by Yaswanth Kodavali.
* Visit [network branch page of this project](http://www.github.com/kenshinthebattosai/customBotConsole/network) for network/branch information.

##Ongoing Branches of Work
(to be updated every once branches of work are finished)
* [kenshinthebattosai](http://www.github.com/kenshinthebattosai) currently working on an improved implementation of least squares scan-matching.
* [balakumar-s](http://www.github.com/balakumar-s) currently working on segmentation of laser readings for line fitting and line fitting.
* yash.kodavali currently working on understanding the working of the bot.
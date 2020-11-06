# Brushwood Golf Club Scoring

This application provides a C#-based command line application that is a prototype of the scoring system for
the Brushwood Golf Club.

## Getting Started

To get started, check out the project from GitHub, get the software installed to build and run the application,
and then attempt to run it.

### Getting the Project

The project uses Git and is hosted on GitHub. Therefore, you will need a GitHub account and the Git utilities. Once
those requirements are met, you can clone the repository using the following commands:

    git clone git@github.com:toddWallentine/brushwoord-score.git

This will checkout the .NET Solution onto your local machine so that you can build, run, and develop the application.

### Installing the Build Tools

This application is built using .NET Core so you will need to install:

* .NET Core 3.1

### Running the Application using the Build Tools

To run the application, you can use the .NET command line (dotnet). Switch into the Brushwood project (`Brushwood` directory)
and run:
    dotnet run courseName rounds.csv golfers.csv

where you specify the name of the course (so that the application can find the CSV that defines the holes on the course),
the CSV that has the scores for all the golfers, and finally the list of golfers and their associated quota/handicap.

The result of this will be the scoring summary that can be used to calculate the winners and how much of the pot each person
won.

## Projects

There are several projects that make up the Brushwood Golf solution including:

* Brushwood: The main project that has the runnable console application (command line interface - CLI).
* Brushwood.Domain: The project that holds the domain classes including Golfer, Course, and Hole.
* Brushwood.Tests: The main set of automated tests.
* Brushwood.Domain.Tests: The automated tests for the domain classes.
# Basic Twitter Viewer & Editor

This repository contains a Basic Twitter Viewer and Editor developed in Python. This project was created for the "Software Development Tools & Systems Programming" course at the Technical University of Crete.

## 📖 Project Overview
The main goal of this project is to apply standard software development practices and tools in Python. The application is built by iteratively applying Logging, Profiling, Refactoring, and Unit Testing to a foundational codebase. 

## 📊 Dataset
* The application uses a dataset of tweets related to the 2012 US Presidential Election.
* The dataset file is approximately 1GB in size.
* It contains roughly 300,000 tweets stored in JSON format.
* The system filters the data to read only the "text" and "created at" fields for each tweet.
* In-file IDs are ignored; a tweet's ID is strictly defined by the line number it occupies.

## ⚙️ Supported Commands
The viewer operates via a command-line interface, running a continuous loop that accepts the following user inputs:

* **`C`**: Creates a new tweet using provided text and the current system date/time.
* **`r <number>`**: Reads the tweet located at the provided line/ID number.
* **`u <number>`**: Updates the text of the tweet at the provided line/ID number.
* **`d`**: Deletes the current tweet.
* **`$`**: Navigates to and reads the last tweet in the dataset.
* **`-`**: Navigates to the tweet exactly one position above the current one.
* **`+`**: Navigates to the tweet exactly one position below the current one.
* **`=`**: Prints the ID of the currently selected tweet.
* **`q`**: Exits the program without saving any modifications.
* **`w`**: Overwrites the file on disk to save current changes.
* **`x`**: Saves all changes to the disk and exits the program.

## 🏗️ Development Lifecycle
The source code was developed in distinct phases to simulate a professional software engineering lifecycle:

* **Development Phase**: The initial working implementation of the application.
* **Logging Phase**: Implementation of an event tracker that records user commands into a `logme.txt` file.
* **Profiling Phase**: Performance analysis to identify bottlenecks in memory usage and execution speed.
* **Refactoring Phase**: Code optimization based on profiling results to improve data loading and handling.
* **Unit Testing Phase**: Creation of test suites to verify the final code implementation.

---
*Developed for Academic Year 2022-2023*

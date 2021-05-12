# Steve's OpenRefine Notes

Initial notes:

Use the overview of each lesson to provide an overview of the activities.

## Setup

Please do this is the pre-session because we won’t have time in the main sessions
Download the files
Install the software
For both of these see the link: https://datacarpentry.org/OpenRefine-ecology-lesson/setup.html
I recommend that you tidy up your desktop (perhaps put everything into a folder so that only the file you need for this workshop are on the desktop). OR MAYBE A SECOND FOLDER CALLED DC-DESKTOP. Put the data file onto your desktop (or your second desktop folder). The key thing is that you should know where it’s stored.)

## Introduction

What do we want from a good analysis?

Good results = Good data + Good analysis

What is good data? Perhaps ask the class for what good data is. Possible answers are: lots of data, no gaps or unknowns, variables are the same data catagory (integers are integers, dates are dates) and no typos.

Computers can make allowances for data which is in the wrong column, or row or typos. Correcting these sorts of issues is called 'data cleaning' or 'data wrangling'.

We'll look at OpenRefine as a way of cleaning data. OpenRefine was called Google Refine, but transisioned to an open source project.
Open refine will help us - to quote the DC pages: "Get an overview of a data set; Resolve inconsistencies in a data set; Help you split data up into more granular parts; Match local data up to other data sets; Enhance a data set with data from other sources; Save a set of data cleaning steps to replay on multiple files"

## Working with OpenRefine

Datefile types (open wee_data files in a text editor or bash) as examples of what data files look like.

Go through the creating project in the OpenRefine lesson.

Facetting is the process of examining different aspects of the dataset: asking what happens if I collect the data in one of these columns in one place. There are different types of facet available, but we'll start with a Text Facet.

(Discuss the similar names listed under the text facetting process)

Clustering is where we try to combine data that we think is similar: for example New York, new york and newyork are (probably) all the same city. We could correct these by hand, but it's time consuming, we may miss data out by accident, our 'estimates' of similarity may be subjective (and so someone else may do it differently) and we need to do every dataset by hand. Clustering automates that process.

Splitting - follow the DC instructions.

## Extra - writing your own tranformations

You can write your own transformation. (Select the arrow on the species column, cell 
and tranform). In this example we want to convert the species name from the fullname,
given as genus and species to the abbreviated (single letter) genus. After splitting the columns
value.substring(0,1)+"."

Undo-Redo/Trim - follow the DC instructions.

## Filter and Sort with OpenRefine

Follow the DC instructions


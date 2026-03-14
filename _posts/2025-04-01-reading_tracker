---
layout: default
title: Reading Tracker Application
---
# My Personal Project : **Reading Tracker**

## Proposal

My **Reading Tracker** project is an application to track one's journey in reading books. 
It can be used by everyone who loves book, 
especially those who want to stay on track on reading challenges 
or simply want to record their reading progress. 
This project is of interest to me because I have always loved reading books. I am also hoping that it will boost my motivation to read more books.

## User Stories
- As a user, I want to be able to add a book to my reading list an arbitrary number of times.
- As a user, I want to be able to view my reading list in my reading tracker.
- As a user, I want to be able to edit my reading progress of a book(based on the number of pages read).
- As a user, I want to be able to view how many pages I have read in total out of all books in my reading tracker.
- As a user, I want to be able to view how many books in my reading list that I have finished.
- As a user, I want to be able to add a chapter summary of a book.
- As a user, I want to be able to view list of chapter titles of a book.
- As a user, I want to be able to view a chapter summary of a book.
- As a user, I want to be able to save my reading list to file (if so I choose).
- As a user, I want to be able to load my reading list from file (if so I choose).

## Instructions for End User
- You can add multiple books to the reading list by clicking "Add new book" button on the left pane.
- You can edit the book title, current and total page by selecting the book then editing its information on the right pane. Then, click "Edit book" button to save the change.
- You can remove a book from the list by selecting the book then click "Remove book" button on the right pane.
- You can view the current progress of your reading by clicking "Progress" panel on the right pane.
- You can view a chapter summary of a book by selecting the book, then select the chapter title on the right pane.
- You can locate my visual component when opening the application as a splash screen.
- You can save the current state of reading list to a file by clicking "Save to file" button on the left pane.
- You can load reading list from a file by clicking "Load from file" button on the left pane.

## Phase 4: Task 2
```
Thu Mar 27 15:54:58 PDT 2025
The book "Book title" is added to the reading list.
Thu Mar 27 15:55:03 PDT 2025
The book "The Miracles of the Namiya General Store" is added to the reading list.
Thu Mar 27 15:55:03 PDT 2025
The book "The Hunger Games" is added to the reading list.
Thu Mar 27 15:55:03 PDT 2025
Loaded reading list from a file.
Thu Mar 27 15:55:10 PDT 2025
The book "Book title" is added to the reading list.
Thu Mar 27 15:55:25 PDT 2025
The book "Book title" is changed to "My New Book".
Thu Mar 27 15:55:33 PDT 2025
The book "The Hunger Games" is removed from the reading list.
Thu Mar 27 15:55:37 PDT 2025
Saved reading list to a file
```

## Phase 4: Task 3
There are associations between `ReadingTrackerApp`, 
`Book`, and `ChapterSummary` that increases coupling unnecessarily. I would 
remove those associations, leaving `ReadingTrackerApp` only has `JsonWriter`,
`JsonReader`, and `ReadingList` in its field. The app would still be able
to run smoothly since `ReadingList` has associations with `Book` and `ChapterSummary`.

## Credit
splash screen was made by using Canva

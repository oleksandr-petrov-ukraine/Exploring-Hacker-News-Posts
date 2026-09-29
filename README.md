# Exploring Hacker News Posts

This project analyzes Hacker News posts to compare `Ask HN` and `Show HN` posts and investigate how the time of day is associated with the average number of comments.

The analysis was completed using Python and Jupyter Notebook.

## Project Goals

The main goals of this project were to answer two questions:

* Do `Ask HN` or `Show HN` posts receive more comments on average?
* Do `Ask HN` posts created at certain times of the day receive more comments on average?

## Dataset

The project uses a dataset of Hacker News posts containing information such as:

* post ID
* title
* URL
* number of points
* number of comments
* author
* creation date and time

The original dataset was reduced by removing posts that received no comments and then randomly selecting from the remaining posts.

## Analysis

The project includes the following steps:

1. Read the CSV dataset into Python.
2. Separate `Ask HN` and `Show HN` posts.
3. Calculate the average number of comments for each post type.
4. Extract the hour from each `Ask HN` post's creation time.
5. Group posts and comments by hour.
6. Calculate the average number of comments for each hour.
7. Sort the results and identify the hours with the highest average number of comments.
8. Draw conclusions while considering the limitations of the dataset.

## Key Findings

* `Ask HN` posts received approximately **14 comments per post** on average.
* `Show HN` posts received approximately **10 comments per post** on average.
* Among `Ask HN` posts, posts created at **15:00 Eastern Time** had the highest average number of comments: **38.59 comments per post**.

## Limitation

The dataset excludes posts that received no comments.

Because of this, the analysis describes the average number of comments among posts that received at least one comment. The results should not be interpreted as proof that creating a post at a particular time will necessarily result in more comments.

## Technologies and Tools

* Python
* Jupyter Notebook
* CSV
* `csv` module
* `datetime` module
* Git & GitHub

## Project Structure

```text
Exploring-Hacker-News-Posts/
│
├── Basics.ipynb
├── hacker_news.csv
├── README.md
└── .gitignore
```

## Purpose

This is a portfolio project created as part of my transition into a career as a **Python Data Engineer**.

The project helped me practice working with raw data, data processing, grouping and aggregation, working with dates and times, and drawing conclusions from data while considering its limitations.

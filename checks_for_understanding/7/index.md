# Check for Understanding 7

## Question 1 - Storing Data

Recall that, in lecture, we introduced SQL databases as a way to organize and manage data. We've previously seen that we can also use CSV (comma-separated values) files to store data as well. Why might we prefer to use a SQL database instead of a CSV file to store data?

|____|

## Question 2 - Indexing

Recall that, by creating an index to a column of a SQL table, we can speed up `SELECT` queries on that column. Why, then, should we not just always create indexes on every column in a SQL table?

|____|

## Question 3 - shows.db

Recall shows.db from lecture, a database of TV shows from IMDB, which had the following schema:

```sql
CREATE TABLE genres (
    show_id INTEGER NOT NULL,
    genre TEXT NOT NULL,
    FOREIGN KEY(show_id) REFERENCES shows(id)
);

CREATE TABLE people (
    id INTEGER,
    name TEXT NOT NULL,
    birth NUMERIC,
    PRIMARY KEY(id)
);

CREATE TABLE ratings (
    show_id INTEGER NOT NULL,
    rating REAL NOT NULL,
    votes INTEGER NOT NULL,
    FOREIGN KEY(show_id) REFERENCES shows(id)
);

CREATE TABLE shows (
    id INTEGER,
    title TEXT NOT NULL,
    year NUMERIC,
    episodes INTEGER,
    PRIMARY KEY(id)
);

CREATE TABLE stars (
    show_id INTEGER NOT NULL,
    person_id INTEGER NOT NULL,
    FOREIGN KEY(show_id) REFERENCES shows(id),
    FOREIGN KEY(person_id) REFERENCES people(id)
);

CREATE TABLE writers (
    show_id INTEGER NOT NULL,
    person_id INTEGER NOT NULL,
    FOREIGN KEY(show_id) REFERENCES shows(id),
    FOREIGN KEY(person_id) REFERENCES people(id)
);
```

Suppose you expect drama shows to have been most popular (that is, the highest rated) in 2020. Via which table(s) in shows.db could you best answer the question of which genre was most popular in 2020?

|____|

## Question 4 - Race Conditions

In your own words, what is a race condition and why are they a problem? What can be done to prevent race conditions when working with databases?

|____|
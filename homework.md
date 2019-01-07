## Questions

1.  Return ALL the data in the 'movies' table.

A. SELECT * FROM movies

2.  Return ONLY the name column from the 'people' table

A. SELECT NAME FROM people

3.  Oops! Someone at CodeClan spelled Stephen's name wrong! Change it to reflect the proper spelling ('Steven Raferty' should be 'Stephen Rafferty').

A. UPDATE people
   SET
   name = 'Stephen Rafferty'
   WHERE name = 'Steven Raferty';

4.  Return ONLY your name from the 'people' table.

A. SELECT name FROM people
   WHERE name = 'Conor Wilson'

5.  The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.

A. DELETE FROM movies
   WHERE title = 'Batman Begins'

6.  Create a new entry in the 'people' table with the name of one of the instructors.

A. INSERT INTO people (name) VALUES ('Keith Douglas')

7.  Antonio Horta Osario has decided to hijack our movie evening! Remove him from the table of people.

A. DELETE FROM people
   WHERE name = 'Antonio Horta Osario'

8.  The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'! Create a new entry in the 'movies' table to reflect this.

A. INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00')

9.  The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.

A. SELECT show_time FROM movies
   WHERE title = 'Guardians of the Galaxy'

   INSERT INTO movies (title, year, show_time) VALUES ('Guardians of the Galaxy 2', 2017, '20:55')

## Extension

1.  Research how to delete multiple entries from your table in a single command.

A. DELETE FROM movies
   WHERE id in (1, 2, 3, 4, 5)

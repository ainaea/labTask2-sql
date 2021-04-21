# labTask2-sql

-- CREATE TABLE movies(
-- 	movie_id INTEGER PRIMARY KEY AUTO_INCREMENT,
--     title VARCHAR(255),
--     year_released INTEGER,
--     director_id integer,
--     Foreign key(director_id) references directors(director_id)
-- );

-- Question 1
-- SELECT title
-- FROM moviesmovies

-- Question 2
-- SELECT title, year_released
-- FROM movies
-- ORDER BY year_released DESC

-- Question 3
-- SELECT *
-- FROM directors
-- ORDER BY country ASC

-- Question 4
-- SELECT *
-- FROM directors
-- ORDER BY country, last_name ASC

-- Question 5
-- INSERT INTO directors (first_name, last_name, country)
-- VALUES ("Rob", "Reiner", "USA"); 

-- Question 6
-- SELECT last_name, director_id
-- FROM directors
-- WHERE first_name = "Rob" AND last_name = "Reiner"

-- Question 7
-- INSERT INTO movies (title, year_released, director_id)
-- VALUES ("The Princess Bride", 1987, 11);

-- Question 8
-- SELECT movies.title, movies.year_released, directors.last_name
-- FROM movies
-- INNER JOIN
-- directors ON movies.director_id = directors.director_id

-- Question 9
-- SELECT movies.title, directors.first_name, directors.last_name
-- FROM movies
-- INNER JOIN
-- directors ON movies.director_id = directors.director_id
-- ORDER BY directors.last_name

-- Question 10
-- SELECT first_name, last_name
-- FROM directors
-- WHERE director_id = 2

-- Question 11
-- SELECT directors.last_name, directors.country
-- FROM movies
-- INNER JOIN
-- directors ON movies.director_id = directors.director_id
-- WHERE movies.title = "Roma"

-- Question 12
-- DELETE FROM movies 
-- WHERE movie_id = 15;
-- Deleting a movie row has no adverse effect on movies and directors

-- Question 13
-- DELETE FROM directors 
-- WHERE director_id = 7;
-- Cannot delete or update a parent row: a foreign key constraint fails

-- Question 14
-- SELECT first_name AS fname, last_Name AS lname, director_id AS id
-- FROM directors;

-- Question 15
-- SELECT movies.title
-- FROM movies
-- INNER JOIN
-- directors ON movies.director_id = directors.director_id
-- WHERE first_name = "Peter" AND last_name = "Jackson"

-- Question 16
-- ALTER TABLE movies
-- ADD earnings DECIMAL;
-- UPDATE movies
-- SET earnings = movie_id * 2.3 + director_id * 5.3
-- WHERE movie_id BETWEEN 1 AND 17; 
-- SELECT title
-- FROM movies
-- WHERE earnings >= 50
-- ORDER BY earnings;


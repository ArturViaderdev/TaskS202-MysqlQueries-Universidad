# 📌 Sprint 2.2: SQL Evaluator (Universidad)

## How to Use the SQL Query Evaluator

1. **Create a repository on GitHub**
    - Use this repository as a _template_ and copy it to your account using the "Use this template" button.
2. **Edit your queries directly on GitHub**
    - In your repository, navigate to `queries/queries.sql`.
    - Click **“Edit this file”** (the pencil icon) and paste each query below its corresponding statement.
    - When you’re done, save the changes using “Commit changes” with a clear message.
3. **Check the execution**
    - The changes will be automatically applied to the main branch.
    - GitHub Actions will detect the new commit and launch the workflow.
4. **Review the results**
    - Once the workflow has finished, a file named `RESULTADOS.md` will be generated in the main branch.
    - Open it to see which queries passed or failed the tests.
5. **Fix the issues**
    - If any query is incorrect, edit `queries/queries.sql` again via GitHub’s web interface.
    - Commit again and wait for `RESULTADOS.md` to regenerate.
6. **Submit the link**
    - Once all queries have been validated, copy and share your repository’s URL on Moodle.

***
Data alone doesn't explain anything. With SQL, you learn to ask the questions that reveal what really matters.

## Task Overview

This task invites you to practice the art of formulating precise and useful questions to a database, an essential skill in backend development and data analysis. You'll work with two databases, **Tienda** and **Universidad**, allowing you to tackle everything from basic queries to more advanced operations with multiple tables, filtering, sorting, and aggregations. The goal isn't just to get the correct result, but to understand what you're asking, how you're doing it, and why.

Think of each query as a small logical thinking challenge: how to access relevant information, how to relate tables, and how to structure the query to get exactly what you need in the clearest and most optimized way possible.

## How to Complete the Task

- Import the two provided database schemas (**Tienda** and **Universidad**) into your MySQL environment.
- Each query is numbered. Write it, execute it, and verify it works correctly.
- Once you think a query is correct, reflect on whether it can be improved: Is there a clearer way? Can it be optimized? Research SQL best practices and optimization techniques.
- For submission, copy all queries to the corresponding automatic correction repository, following the instructions in the **README.md**.
- Review your results files to ensure everything is well-written and returns the expected output.
- When ready, add the links to your automatic correction repositories to Moodle and submit the task to your mentor.

## Universidad Database

**Auto-evaluation:** [Link to auto-evaluation repository](https://github.com/IT-Academy-Back/university-sql-queries-evaluator/tree/main)

Download the database from the **schema_universidad.sql** file, view the E-R diagram in an editor, and perform the following queries:

```sql
-- 1. Return a list with the first surname, second surname, and name of all students. The list must be sorted alphabetically from lowest to highest by first surname, second surname, and name.
-- 2. Find the name and both surnames of students who haven't registered their phone number in the database. (nombre, apellido1, apellido2)
-- 3. Return the list of students born in 1999. (id, nombre, apellido1, apellido2, fecha_nacimiento)
-- 4. Return the list of professors who haven't registered their phone number in the database and whose NIF ends with K. (nombre, apellido1, apellido2, nif)
-- 5. Return the list of subjects taught in the first semester, in the third year of the degree with identifier 7. (id, nombre, cuatrimestre, curso, id_grado)
-- 6. Return a list of professors along with the name of the department they are linked to. The list must return four columns: first surname, second surname, name, and department name. The result will be sorted alphabetically from lowest to highest by surnames and name. (apellido1, apellido2, nombre, departamento)
-- 7. Return a list with the subject names, start year, and end year of the school year for the student with NIF 26902806M. (nombre, anyo_inicio, anyo_fin)
-- 8. Return a list with the names of all departments that have professors teaching some subject in the Computer Engineering Degree (Plan 2015). (nombre)
-- 9. Return a list with all students who enrolled in some subject during the 2018/2019 school year. (nombre, apellido1, apellido2)
```

**Solve the next 6 queries using LEFT JOIN and RIGHT JOIN clauses.**

```sql
-- 10. Return a list with the names of all professors and the departments they are linked to. The list must also show those professors who have no department associated. The list must return four columns: department name, first surname, second surname, and professor name. The result will be sorted alphabetically from lowest to highest by department name, surnames, and name. (departamento, apellido1, apellido2, nombre)
-- 11. Return a list with professors who are not associated with a department. (apellido1, apellido2, nombre)
-- 12. Return a list with departments that have no professors associated. (nombre)
-- 13. Return a list with professors who don't teach any subject. (apellido1, apellido2, nombre)
-- 14. Return a list with subjects that have no professor assigned. (id, nombre)
-- 15. Return a list with all departments that haven't taught subjects in any school year. (nombre)
```


## Summary Queries

```sql
-- 16. Return the total number of students. (total)
-- 17. Calculate how many students were born in 1999. (total)
-- 18. Calculate how many professors there are in each department. The result should only show two columns: one with the department name and another with the number of professors in that department. The result should only include departments with associated professors and must be sorted from highest to lowest by number of professors. (departamento, total)
-- 19. Return a list with all departments and the number of professors in each. Note that there may be departments with no associated professors. These departments must also appear in the list. (departamento, total)
-- 20. Return a list with the name of all existing degrees in the database and the number of subjects each has. Note that there may be degrees with no associated subjects. These degrees must also appear in the list. The result must be sorted from highest to lowest by number of subjects. (grau, total)
-- 21. Return a list with the name of all existing degrees in the database and the number of subjects each has, for degrees with more than 40 associated subjects. (grau, total)
-- 22. Return a list showing the names of degrees and the sum of total credits for each subject type. The result must have three columns: degree name, subject type, and sum of credits from all subjects of that type. (grau, tipus, total_creditos)
-- 23. Return a list showing how many students enrolled in some subject in each school year. The result must show two columns: one with the start year of the school year and another with the number of enrolled students. (anyo_inicio, total)
-- 24. Return a list with the number of subjects each professor teaches. The list must include professors who don't teach any subject. The result will show five columns: id, name, first surname, second surname, and number of subjects. The result will be sorted from highest to lowest by number of subjects. (id, nombre, apellido1, apellido2, total)
-- 25. Return all data of the youngest student.
-- 26. Return a list with professors who have an associated department and don't teach any subject. (apellido1, apellido2, nombre)
```


## Levels

- **Level 1**: Achieve if you build 37 correct queries, 20 of which must be from the Universidad diagram.
- **Level 2**: Achieve if you build between 37 and 56 correct queries, 20 of which must be from the Universidad diagram.
- **Level 3**: Achieve if you successfully build more than 56 correct queries (20 of them from the Universidad diagram)!!!


## Resources

You can download the databases from the files shema_tienda.sql and schema_universidad.sql.

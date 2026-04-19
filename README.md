# Exercise: university data analysis with LINQ
The academic coordination office needs a small console tool that can quickly answer questions about students, courses, lecturers, and enrollments. The technical team has already prepared the data model and a class with sample collections. Your job is to complete the methods that execute LINQ queries on in-memory objects and present the results in the console.

## Business context
The application is meant to support everyday work of a program coordinator. In practice, this means quickly finding students by chosen criteria, checking enrollment activity, preparing small summaries, and building more advanced cross-sectional reports. The goal is to write clear code that reflects SQL-style thinking while using LINQ capabilities in C#.

## What you receive
* a ready-to-run console application with a menu,
* domain classes: `Student`, `Course`, `Lecturer`, `Enrollment`,
* a `UniversityData` class that loads data into static collections,
* a `LinqExercises` class with methods to complete,
* comments above every method with a task description and an SQL equivalent.

## Implementation scope
Complete the methods in `Exercises/LinqExercises.cs`. Each method should return a collection of strings, and the application will print those strings in the console after the matching menu option is selected.

1. Filtering with Where.
2. Projection with Select.
3. Sorting with OrderBy and ThenBy.
4. Reading a single element with FirstOrDefault.
5. Condition checks with Any and All.
6. Counting with Count.
7. Removing duplicates with Distinct.
8. Simple paging with Skip and Take.
9. Combining data with Join.
10. Flattening nested results with SelectMany.
11. Grouping with GroupBy.
12. Basic aggregations such as Average and Max.

## Advanced challenge section
At the end of the project you will also find four extra questions that combine several LINQ operators in one query. This part best reflects how larger business reports are usually built.

1. Students with more than one active enrollment.
2. Courses starting in April 2026 without final grades.
3. Lecturers and the average grade across all of their courses.
4. Student cities and the number of active enrollments.

## Suggested workflow
1. Run the application and choose option 0 to see the input data overview.
2. Read the comment above the selected method in LinqExercises.
3. Try to sketch the SQL version first and only then rewrite it as a LINQ expression.
4. Keep the output readable so that correctness can be checked quickly.
5. After each change, run the program again and validate the result from the menu.

## Example menu fragment
```
Console.WriteLine("1. Students from Warsaw");
Console.WriteLine("2. Student email addresses");
Console.WriteLine("3. Students sorted alphabetically");
```

## Assessment criteria
* correct use of LINQ operators,
* result consistent with the task description,
* readability and simplicity of the query,
* ability to combine several operators in more advanced cases.
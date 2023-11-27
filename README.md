# Create
<div>Create Table Mother(Id int NULL)</div>
<div>Create Database Lesson</div>

# Drop
<div>Drop Database Lesson</div>
<div>Drop Table Mother</div>

# Alter
<div>Alter Table Student ADD Age int NULL</div>
<div>Alter Table Student Drop Column Age</div>
<div>Alter Table Student Alter Column Age smallint</div>

# Select
<div>Select * From Student</div>
<div>Select Name from Student</div>
<div>Select * from Student Where Name = 'Ali'</div>
<div>Select * from Student Where Name = 'Ali' order by Id DESC</div>
<div>Select Sum(Id) as ToplamId from Student</div>
<div>Select Min(Id) as MinId from Student</div>
<div>Select Max(Id) as MaxId from Student</div>
<div>Select Count(Id) as MinId from Student</div>
<div>Select Avg(Id) as MaxId from Student</div>
<div>Select Top 5 Id from Student</div>
<div>Select Top 50 percent Id from Student</div>
<div>Select DISTINCT name from Student</div>
<div>Select * from Student Where Name='Ali' AND ClassId = 2</div>
<div>Select * from Student Where Name='Ali' OR ClassId = 2</div>
<div>Select * from Student Where Name='Ali' OR ClassId = 2 AND Id=3</div>
<div>Select * from Student Where Name Like '%a%'</div>
<div>Select * from Student Where Name Like 'a%'</div>
<div>Select * from Student Where Name Like '%a'</div>
<div>Select * from Student Where Name IN('Haydar')</div>
<div>Select * from Student Where Id Between 0 AND 5</div>
<div>Select * from Student Where Date Between '1948-11-11' AND '1948-11-12'</div>
<div>Select Name,Count(Name) as NameCount from Student Group By Name Order By Name DESC</div>
<div>Select Name,Count(Name) as [NameCount] from Student Group By Name Having Count(Name) > 1</div>

# Insert
<div>Insert into Student(Name) Values('Haydar')</div>

# Update
<div>Update Student Set Name='Ali' Where Name='Ayla'</div>

# Delete
<div>Delete from Student Where Id=2</div>

# Truncate
<div>Truncate Table Student</div>

# Join
<div>SELECT S.Id,S.Name,S.LessonId,L.Name AS LessonName ,S.ClassId , C.Name as ClassName FROM STUDENT AS S</div>
<div>FULL JOIN LESSON AS L ON L.Id = S.LessonId</div>
<div>FULL JOIN CLASS AS C ON C.Id = S.ClassId</div>

# Union
<div>Select Name from Student</div>
<div>Union Select Name from Lesson</div>
<div>Union Select Name from Class</div>

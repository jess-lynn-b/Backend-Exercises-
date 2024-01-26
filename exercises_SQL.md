-- -- Exercise 1
CREATE TABLE Customers(
    CustomerID INT PRIMARY KEY,
    Name TEXT,
    Email TEXT
);
INSERT INTO Customers ( CustomerID, Name, Email)
    Values ( 1, 'Alice Johnson', 'alice.johnson@email.com');
INSERT INTO Customers ( CustomerID, Name, Email)
    Values ( 2, 'Bob Smith', 'bob.smith@email.com');
INSERT INTO Customers ( CustomerID, Name, Email)
    Values ( 3, 'Charlie Brown', 'charlie.brown@email.com');
-- SELECT * FROM Customers;

-- -- Exercise 2 Part
-- UPDATE Customers
-- SET Email = 'bob.smith@newdomain.com'
-- WHERE CustomerId = 3;
-- SELECT * FROM Customers;

-- -- Exercise 3 
-- DELETE FROM Customers
-- WHERE CustomerID = 3;
-- SELECT * FROM Customers;

-- -- Exercise 4

-- CREATE TABLE Orders ( 
--     OrderQty INT PRIMARY KEY
-- );
-- INSERT INTO Orders (OrderQty)
--     VALUES (1);

-- CREATE TABLE Books(
--     Title Text PRIMARY KEY
   
-- );
-- INSERT INTO Books (Title)
--     VALUES ('If you give a mouse a cookie');
-- SELECT * FROM Customers, Books, Orders;

-- Exercise 5

CREATE TABLE Students(
    StudentID INT PRIMARY KEY,
    Name TEXT
);

CREATE TABLE Grades (
    StudentID INT PRIMARY KEY,
    Subject TEXT,
    Grade INT
);
INSERT INTO Students( StudentID, Name)
    VALUES (1, 'Wessley Green');
INSERT INTO Students( StudentID, Name)
    VALUES (2, 'Jelly Roll');
    
INSERT INTO Grades ( StudentID, Subject, Grade)
    Values (1, 'Math', 92);
INSERT INTO Grades ( StudentID, Subject, Grade)
    Values (1, 'Science', 98);
INSERT INTO Grades ( StudentID, Subject, Grade)
    Values (2, 'English', 82);
SELECT * FROM Students, Grades;

  
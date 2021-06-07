## Description

A group of N students take a Physics exam. Design an algorithm that reads for each student the grade obtained and calculates and prints:

A.- The number of students who obtained a grade lower than 50.

B.- The number of students who obtained a grade of 50 or more but less than 70.

C.- The number of students who obtained a grade of 70 or more but less than 80.

D. The number of students who earned a grade of 80 or higher.

## Usage

```Javascript

 let Student=require("./Student").Student;
 let Group=require("./Group").Group;
let arraystudents=[];

arraystudents.push(new Student(50));
arraystudents.push(new Student(80));
arraystudents.push(new Student(70));
arraystudents.push(new Student(55));
arraystudents.push(new Student(54));
arraystudents.push(new Student(65));
arraystudents.push(new Student(45));
arraystudents.push(new Student(90));
arraystudents.push(new Student(30));
arraystudents.push(new Student(80));
arraystudents.push(new Student(60));
arraystudents.push(new Student(20));
arraystudents.push(new Student(10));
arraystudents.push(new Student(62));
arraystudents.push(new Student(71));
arraystudents.push(new Student(62));
 let group=new Group(arraystudents);
let calc=group.calculate_grades();
console.log(calc.a+" Students scoring less than 50");
console.log(calc.b+" Students with a grade of 50 or more but less than 70");
console.log(calc.c+" Students with a grade of 70 or more but less than 80");
console.log(calc.d+" Students with a grade of 80 or more");


```
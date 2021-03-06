
This README describes the instructions for a Java programming exercise. 

Scenario:

An online course booking system is being built for a college. Students log in and
register for available courses on a first-come, first-serve basis.

A Student in the system is associated with a collection of all the courses they have 
already taken. 

A Course, such as "Java Data Structures" is run periodically. Each
time a course is scheduled, it has associated attributes such as which students are registered to take it. It also has a pre-set capacity for the number of students that can 
register. If a student tries to register and the course is full, they will be automatically wait-listed. If a registered student withdraws, the system
should register a wait-listed student (if there is one) to fill their place.

Some courses have pre-requisites: these are other courses that students must have taken before
they are allowed to register for a course. When trying to register for a course, the system must check that
they have completed any pre-requisites. 

When a Student registers for a course, it does not change their 'courses taken' attribute. Eventually when they have passed assessment their record will change, but that is beyond the scope of this exercise.

To help get started, Course, Student and CourseSchedule classes have been created. The aim of the exercise is just to implement the two
public methods on CourseSchedule - so effectively just the parts of the system that allow students to register and de-register from courses. In the finished system you can assume these are ultimately triggered from the web interface, but there is no need to implement any of that. Preserve the three given classes and the signatures of the public methods
on CourseSchedule, but change anything else you like, including the fields of the classes. 

This pretend system has no durable persistence, all state changes are
'in memory' only. Given that context, consider that in the running system there
will be a single instance of CourseSchedule per course being
scheduled - meaning all requests to register/de-register for a
particular course are called on just one Java object.

All the functional requirements given are equally important. From a non-functional standpoint, your solution
must scale well - for example you might imagine this is an online college containing hundreds of thousands of students. 



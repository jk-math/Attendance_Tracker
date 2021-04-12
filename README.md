# Attendance_Tracker

With many of my classes moving to remote instruction, taking attendance has morphed into combing through meeting attendance csv files produced by Microsoft Teams. I decided to write some code so that I could upload all the attendance csv files and have an attendance tracker generated for me.

Many students arrive late to class and this has been incredibly frustrating. Many students log in to meetings a few minutes late, which is something they would not do if the classes were in person. Imagine having to creak open the door when the instructor is already 5 minutes into the class. This is not something students do in person, but it has quickly become something students do online. As a result, I wanted some way to track when students arrived late. Luckily, the datetime objects in Python make this incredibly easy. I also wanted a way to introduce a time buffer. For example, if class starts at 9am and a student logs in at 9:00:37am, I may not want to mark this student as late. 

The attendance tracker will also mark students as absent. I have noticed an uptick in the number of absences for remote courses. My guess is that students think that instructors just don't notice that they are not attending. There are some potential problems with this. If students log in with an account other than their college issued email account, they will be marked as absent. I haven't fully built out what to do in the case that a student logs in with a different account or attends the meeting as a "guest".

As any instructor knows, many students log in to meetings and do not actually attend class. This attendance tracker does not take that into account. I typically stick around for a couple of minutes after class and just mark down the students who do not respond to me. 

I should also note that I do not require students to have their cameras on during class meetings. Perhaps this requirement would result in better student attendance, but at this point I don't feel comfortable requiring students to be on camera. There are students who create looping videos of themselves to make it seem like they are really attending class, so requiring cameras to be on is not a fix for everything. 

I have included some test files including an example of an initial roster used to create the attendance tracker and an example of a Teams attendance report.

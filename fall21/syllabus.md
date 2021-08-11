# CS 625, Fall 2021 Syllabus

[Jump to Summary Schedule](#summary-schedule) | [Download printable PDF version](https://github.com/odu-cs625-datavis/public/raw/main/fall21/syllabus.pdf)

## Course Overview

*"The purpose of visualization is insight, not pictures." -Ben Shneiderman*

**Catalog Description:** This course covers the theory and application of data visualization. This includes issues in data cleaning to prepare data for visualization, theory behind mapping data to appropriate visual representations, introduction to visual analytics, and tools used for data analysis and visualization. Modern visualization software and tools will be used to analyze and visualize real-world datasets to reinforce the concepts covered in the course.

**Comparison to CS 725/825:** If you have already taken CS 725/825, then CS 625 is not appropriate for you. Future offerings of CS 725/825 require CS 625 as a prerequisite.

## Instructor Contact and Office Hours

Dr. Michele Weigle: mweigle at cs.odu.edu, <https://www.cs.odu.edu/~mweigle/>

My office hours will be Tue 11a-12:30p (in-person and/or Zoom) and Thu 5-6:30p (Zoom only), or by appointment. See Blackboard for the link to the Zoom office hours meeting room. For Zoom office hours, students will be placed into the waiting room if I am already meeting with another student. If you cannot attend during regular office hours, please contact me to set up an alternate appointment time.

## Course Objectives

After completing this course, you should be able to do the following:

* Use OpenRefine to explore and clean real-world data.
* Explain the difference between exploratory (discover task) and explanatory (present task) visualizations.
* Describe the channels of visual encoding and order them from most effective to least effective.
* Identify a visualization where an inappropriate arrange design choice was made and explain why the choice was inappropriate.
* Explain how different data types map most effectively to various visualization idioms (i.e., charts).
* Explain the importance choosing an appropriate colormap.
* Given a dataset, develop questions about the data that can effectively be answered with a visualization.
* Critique and redesign an existing visualization.
* Use Tableau, R, Vega-Lite, or other API or software to create effective standard charts, such as line charts, scatterplots, bar charts.
* Use Tableau, R, Vega-Lite, or other API or software to create an effective visualization of real-world data.
* Explain and defend the design choices that you made in creating your visualization.

## Meeting Times and Course Delivery Method

This course will be organized based on the "flipped classroom" model. Students will be assigned readings and homework that will be due before the class meeting time. There will be few, if any, lectures by the instructor. Class time will be spent on discussions of the readings and assignments, demonstrations, and in-class work. *It is essential that each student be fully prepared to participate in class discussions each week.*

This course will be delivered in a hybrid method, with one face-to-face section in a traditional classroom and several online sections available:

* CRN 18816 - in-person (TR 9:30-10:45am, ECSB 2120)
* CRN 18819 - WC2 (in Hampton Roads)
* CRN 18820 - WC5 (in Virginia, but outside of Hampton Roads)
* CRN 18821 - WC7 (in the US, but outside of Virginia)
* CRN 18990 - WC8 (outside of the US)

All course materials, including the link to the Zoom class session, will be made available in Blackboard. The audio of in-person class meetings and all materials projected in class will be live streamed via Zoom and recorded for later viewing. *Online students are strongly encouraged to actively participate in the Zoom session during the regular class meeting time.* Online students must meet the same deadlines as face-to-face students. All deadlines are based on the local timezone in Norfolk, VA.

### Fall 2021 COVID-19 Policies

As announced on [August 11](https://www.odu.edu/news/2021/8/message_from_preside), all students, faculty, and staff who participate in on-campus activites must be fully vaccinated or have received an exemption (and be tested weekly). In addition, face masks are required for all individuals in indoor public spaces, including classrooms.  I have been fully vaccinated.

Students who are uncomfortable with participating in the classroom are encouraged to switch to the WC2 section to enable other students who might prefer the face-to-face environment to have a seat.

*You are strongly encouraged to stay home if you are not feeling well.*

The provision of face-to-face lectures and live Zoom streams are contingent on the setup of the classroom and supporting equipment, and the general level of COVID-19 activity in the Hampton Roads area. If I become uncomfortable with the safety precautions being taken, or feel that the classroom environment and equipment detract from the quality of the course, then I reserve the right to change to a pure web conferencing delivery mode. *Additional notes related to ODU's Fall 2021 semester and COVID-19 may be added to this syllabus nearer to the beginning of the semester.*

## Requirements

### Prerequisites

There are no specific course prerequisites for this course, but I expect you to be comfortable with basic statistics. Extensive programming experience is not required, but you should be familiar with basic programming concepts (variables, arrays, functions, conditionals, etc.).

Additionally, if you choose to use certain APIs (not required), you should be familiar with Unix, HTML, CSS, JavaScript, and jQuery. If you need a refresher on Unix, see the [CS 252](https://www.cs.odu.edu/~zeil/cs252/latest/Directory/outline/index.html) webpage. There are many excellent resources available online for common web languages. 

### Course Materials

The required textbook for this course is [*Visualization Analysis and Design*](http://www.cs.ubc.ca/~tmm/vadbook/) by Tamara Munzner

* [online version accesssible for free via ODU](https://go.oreilly.com/old-dominion-university//library/view/visualization-analysis-and/9781466508910/)
* includes author's slides from half-day and full-day tutorials, PDF versions of all figures
* [textbook errata](http://www.cs.ubc.ca/~tmm/vadbook/errata.html)
* [author's keynote at d3.unconf](https://www.youtube.com/watch?v=jVC6SQS23ak) (55 min), overview of material from book

You will be required to write clearly about your visualization designs and design process. For writing help, I always suggest two inexpensive books:

* Writing for Computer Science by Justin Zobel
* The Elements of Style by Strunk and White

In addition, see the online writing resources collected on the ODU-CS [New Student Resources page](https://graduate.cs.odu.edu/resources/new-students/#Writing).

## Grading

### Assignment Types

Your grade in this class will be based on the following components:

**Participation** - 10%

* in addition to being present, students are expected to be prepared to talk about examples and figures in the required readings, explain learning checks, discuss their homework submissions, and participate in online discussions
* will receive points (0-2) for each week of class
* in-class rubric:
  * 0 - no participation during the week
  * 1 - late to class or not prepared to participate
  * 2 - on time to class and actively participating in discussions and in-class work
* online rubric:
  * 0 - no access of the class recording before the next class meeting or participation in online discussions
  * 2 - watched the class recording before the next class meeting and actively participating in online discussions

**Learning Checks** - 10%

* preparation for the next class meeting, submitted via Blackboard before the class meeting time
* I will not correct your answers, but correct answers with references to the textbook will be provided after the due date
* rubric:
  * 0 - not submitted
  * 1 - did not answer all questions or late submission (within 48 hours of due date)
  * 2 - answered all questions and submitted on time

**Homework** - 50%

* implement concepts from a previous class meeting, submitted via GitHub
* grading scale: 0-10, where 10 is the absolute best (don't expect to get 10s on a regular basis)
  * 2 points are reserved for the required writeup about the assignment
  * late assignments have a maximum score of 8

**Midterm Exam** - 30%

* demonstrate comprehension and application of concepts discussed during the first half of the semester
* open book, open notes

### Grading Scale

The grading scale is as follows:

| percentage | letter | 
| --- | --- | 
| 100-94 | A | |
| 93-90 | A- | 
| 89-88	| B+ | 
| 87-84	| B	| 
| 83-80	| B- | 
| 79-78 | C+ |
 | 77-74 | C |
| 73-70 | C- |
| 69-0 | F|

### Late Assignments

Any assignment submitted after its deadline is considered late. Submissions over 48 hours late are not accepted. This time limit includes weekends -- they are counted just like weekdays.

I reserve the right to specify that late submissions will not be accepted for particular assignments.

## Summary Schedule

*Note: This is a tentative schedule and may change during the semester. The complete schedule with assignments and due dates is posted on Blackboard.*

[ODU Fall 2021 academic schedule](https://www.odu.edu/academics/calendar/fall)

|Week |Date|Topic| Textbook Reading|
|---|---|---|---|
|1|	Aug 31, Sep 2|	Introduction, What's Vis and Why Do It? | Ch 1|
|2|	Sep 7, 9|	Data and Data Cleaning | Ch 2|
|3|	Sep 14, 16|	Marks and Channels | Ch 5|
|4|	Sep 21, 23	|Arrange Tables | Ch 7|
|5|	Sep 28, 30|	Arrange Tables (continued) | Ch 7|
|6|	Oct 5, 7|	Map Color and Other Channels | Ch 10|
|7|	Tue, Oct 12<br/>Thu, Oct 14|	**NO CLASS - Fall Break**<br/>Review for Mid-Term Exam| |
|8|	Tue, Oct 19<br/>Thu, Oct 21|	**MID-TERM EXAM**<br/>**NO CLASS**| |
|9|	Oct 26, 28|	Reduce Items | Ch 13 (through 13.4.1)
|10|	Nov 2, 4|	Exploratory Data Analysis (EDA)
|11|	Nov 9, 11|	Storytelling Vis
|12|	Nov 16, 18|	Rules of Thumb, Maps|Ch 6, Ch 8.1-8.3
| | Nov 23, 25|**NO CLASS - Thanksgiving Break** | |
|13|	Nov 30, Dec 2|	Multiple Views | Ch 12 (skip 12.4.4)
|14|	Dec 7, 9|	Manipulate View | Ch 11 (through 11.5)|
|| Fri, Dec 10|	*last day of classes*

## Course Policies

### Email/Blackboard

Each student must check the class Blackboard site and email daily. You should use our class Blackboard Discussion Board to ask and answer general course-related questions. I will use Blackboard Announcements to notify you about important updates (assignment deadline changes, office hours cancellations, etc.).

### Attendance (in-person students)

Since much of the course is based on discussion and in-class work, I expect you to arrive on time for class. Your grade will be affected if you are consistently tardy. If you have to miss a class, you are responsible checking the course Blackboard site to find any assignments or notes you may have missed. Students may leave after 15 minutes if the instructor or a guest lecturer does not arrive in that time.

If there are days on which the scheduled class meeting time is cancelled due to weather, there may still be assignments made and due. A post will be made to Blackboard Announcements whenever the class meeting is cancelled.

### Classroom Conduct

Please be respectful of your classmates and instructor by minimizing distractions during class. Cell phones must be turned to silent during class.

### Make-up Work

Make-ups for graded activities are possible only with a valid written medical or university excuse. It is the student's responsibility to give the instructor the written excuse and to arrange for any makeup work to be done.  A makeup exam may be different (and possibly more difficult) than the regularly scheduled exam.

### Disability Services

In compliance with PL94-142 and more recent federal legislation affirming the rights of disabled individuals, provisions will be made for students with special needs on an individual basis. The student must have been identified as special needs by the university and an appropriate letter must be provided to the course instructor. Provision will be made based upon written guidelines from the University's [Office of Educational Accessibility](http://www.odu.edu/educationalaccessibility). All students are expected to fulfill all course requirements.

Students are encouraged to self-disclose disabilities that have been verified by the Office of Educational Accessibility by providing Accommodation Letters to their instructors early in the semester in order to start receiving accommodations. Accommodations will not be made until the Accommodation Letters are provided to instructors each semester.

### Seeking Help

The course Blackboard site should be your first reference for questions about the class. If you have questions about course requirements or materials, post questions using the class Blackboard Discussion Board. For extra help, attend office hours.

## Academic Integrity

Old Dominion University is committed to students' personal and academic success. In order to achieve this vision, students, faculty, and staff work together to create an environment that provides the best opportunity for academic inquiry and learning. All students must be honest and forthright in their academic studies. Your work in this course and classroom behavior must align with the expectations outlined in the Code of Student Conduct, which can be found at https://www.odu.edu/oscai.

The following behaviors along with classroom disruptions violate this policy, corrupt the educational process, and will not be tolerated.

* Cheating: Using unauthorized assistance, materials, study aids, or other information in any academic exercise.
* Plagiarism: Using someone else's language, ideas, or other original material without acknowledging its source in any academic exercise.
* Fabrication: Inventing, altering or falsifying any data, citation or information in any academic exercise.
* Facilitation: Helping another student commit, or attempt to commit, any Academic Integrity violation, or failure to report suspected Academic Integrity violations to a faculty member.

*In particular, submitting anything that is not your own work without proper attribution (giving credit to the original author) is plagiarism and is considered to be an academic integrity violation. It is not acceptable to copy source code or written work from any other source (including other students, online resources), unless explicitly allowed in the assignment statement. In cases where using resources such as the Internet is allowed, proper attribution must be given.*

Any evidence of an academic integrity violation (cheating) will result in a 0 grade for the assignment/exam, and the incident will be submitted to the Department of Computer Science for further review. Note that academic integrity violations can result in a permanent notation being placed on the student's transcript or even expulsion from the University. Evidence of cheating may include a student being unable to satisfactorily answer questions asked by the instructor about a submitted solution. Cheating includes not only receiving unauthorized assistance, but also giving unauthorized assistance. For class files kept in Unix space, students are expected to use Unix file permission protections (chmod) to keep other students from accessing the files. Failure to adequately protect files may result in a student being held responsible for giving unauthorized assistance, even if not directly aware of it.

Students may still provide legitimate assistance to one another. You are encouraged to form study groups to discuss course topics. Students should avoid discussions of solutions to ongoing assignments and should not, under any circumstances, show or share code solutions for an ongoing assignment.

All students are responsible for knowing the rules. If you are unclear about whether a certain activity is allowed or not, please contact the instructor.

More information on academic integrity is available on the ODU-CS [academic integrity page](https://graduate.cs.odu.edu/resources/academic-integrity).

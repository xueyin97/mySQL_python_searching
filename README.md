# System for Recommendation for Applying Future Study 
Introduction
Students in UIC are always concerning about their future study nowadays. However, many students don’t have dream schools or are confused about which school they can be admitted to. After solving the problem, every student who wants to apply for their future study will benefit from our database. By creating this searching engine, students can access information about the universities, including world university rankings, teaching evaluation, research evaluation, and income evaluation. Moreover, they can refer to the application results from the previous applicants who have similar grades with themselves. 
Functions
The functions we are going to achieve are in the followings:
1.	Keywords search
i.	Searching for application results
Users can find the relevant application results by entering university name, country, application year, major, degree, and scholarship.  
ii.	Searching for university information
Users can find the detailed university information by entering university name, and country. University name, country, times rankings, teaching evaluation, research evaluation, and income evaluation are contained in university information.
2.	Filter function
i.	Searching for application results
We provide the following attributes for users to filter the application results: country, application year, major, degree, whether the applicants obtain the scholarship, and hot universities.
ii.	Searching for university information
       We provide the two attributes, country and hot university, for users to filter the universities information.
3.	University recommendation
   Users can give their preference score (0-10) to each attribute, including times ranking, major ranking, country, teaching evaluation, research evaluation, and income evaluation. Meanwhile, users can choose whether take GPA into consideration. System will evaluate the university performance by weighted mean equation in accordance to users’ preference. 
4.	 Orientation of users’ application
   Users can enter their GPA, IELTS or TOEFL, GRE grades, future majors to find the applicants whose grades are similar with theirs and the applying major is the same as theirs. The query results will contain applicant ID, university name, country, times rankings, major rankings, GPA, IELTS, TOEFL, GRE, scholarship, degree, and application year. Through the result, students are aware of the universities which they can get in.
5.	Update
   We can update the application dataset and the university dataset in order to provide the current information.
6.	Deletion
       If some universities won’t enroll new students for some reasons, we will delete the data related to the certain university or major and also the applications to the university.

We will use MySQL to create our database which includes all the useful information and convenient commands to implement the above functions. Besides, we will connect MySQL with Python to build a web page as a searching engine that faces to users.

Assumption
There might be some mistakes when inserting data. We will add some constrains to the insertion to avoid mistakes. For instance, the grades can not exceed the full mark or be negative. Each application ID can only link to one student ID, university ID, major, and etc. 

Test
We need to make sure that our data are consistent. Firstly, we will check whether the records linked to primary keys are unique. Then, we will check whether all the records related to the deleted data are removed

Summary
     We expect to create a searching engine by MySQL and Python for undergraduates who plan to apply for their future study. The searching engine can offer users with university information and pervious application results, which will help them to find their dream schools and position themselves.

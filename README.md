# Python Project -- TA Grading System

Suppose you are a TA for a class. You would like to automatically grade students assignment and send back the feedbacks through e-mails.

# Grading
The student assignments are included in the [submissions](submissions) folder named as
```
submission_student_123,
submission_student_234,
submission_student_456,
.....
```
The last 3 digits are student's ID number.

The grading rubic is listed [here](grading_rubic.md).

# Report
1. create a report_student_i.html (replacing i with the student ID number) file for each student, which contains (in reasonably formatted, valid HTML):
   - the name of the student's submission(linked to the file itself)
   - the different integers,decimals,prices,phone numbers and emails in the student's submission (list each category  separately)
   - the total scores of the submission
2. create a valid HTML web page called index.html with links to each of the summary files;
3. create a tar.gz file containing the directory [submissions](submissions) and the directory that contains all the HTML files you created above. Be sure the links in the webpages work after extraction.
   
# email the reports

1. Read the students' email addresses from the CSV file [Roster](Roster.csv). Send student_i.html to the correct student.
2. prompt the user for the email address (professor's email) and send the tar.gz file.
 

# Important Note
Don't hard code students' email addresses in the script. The student email should be read from the roster.

You must run your project on altair and send mail from your @cs.oswego.edu account. You can send mail from the terminal using the mutt command. A little Googling and looking at the man pages should tell you how to use it. The mutt command should not prompt the user for any input. Sender's email password should not be appeared in your script.

A successful demo will involve sending the emails.
As a student in the class, I can receiving the HTML file contains my summary and grade.
As a professor in the class, I can receive the zipped file, extract it, and am able to view students submissions and reports following the links on your page.


# Dev Environment / Useful Resources
- [PyCharm](https://www.jetbrains.com/pycharm/)
- [Regular Expressions in Python 3.6](https://docs.python.org/3/howto/regex.html)
- [Regular Expression Debugger / Tester](https://regex101.com/)






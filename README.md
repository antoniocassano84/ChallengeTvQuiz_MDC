# ChallengeTvQuiz_MDC
MDC - Technical Assessment

REQUIREMENTS (AC comments start with @)
A popular TV show has asked us to build a website that will allow them to publish quizzes.
• Each quiz will consist of a variable number of multiple-choice questions.
  @ At the moment the application consists of only one single quiz. 
  @ The quiz model should be added to allow the use to select a quiz.
  @ This piece of work requires 1 day full time work.
• Each question will consist of 4 possible answers.
• Every person taking part in a quiz have their results stored (and made retrievable) by email address.
  @ At the moment everyone is free to answer the questions without registering. A registration mechanism is needed
• Once a person has completed a quiz, they may not do that one again
  @ Investigate how to restrict quiz access by a user 
• At the end of the quiz it needs to display the users score out of the total number of questions
  @ A score field should be added to the User. A score is associated with a single quiz,user key
• At the end of the quiz it must also display the mean average of users that achieved the same score (to within
the same 10% increment) ( i.e. If I scored 57%, I would expect to see something like “36% of people
completing this quiz also scored between 50 and 60 percent”)
The quiz engine also needs an administration area.
• The admin area only needs simple authentication as only one person will ever use it.
• The admin area must allow the creation, editing and deletion of Quizzes and Questions.
• Once a quiz has been published it cannot be edited only deleted.
• There must also be a facility to view all quizzes completed by a user as well as the answers submitted
A script needs to be implemented that will send an email to a specified email address with details of all the quizzes
completed and how many people scored within each 10% increment of the quiz. The script will be triggered as a
scheduled task using a container orchestration service.

PLAN:
(1) Modify the DB underlying the project to include a new Quiz model with each Question model belonging to one single Quiz (same relationship as Question-Choice). With Django this change is straigthforward - 1 day 
(2) Need a registration mechanism to allow the tracking of the user activity. With Django this can be done (https://www.youtube.com/watch?v=2yoWf-kDXIk) - 5 days
(3) 




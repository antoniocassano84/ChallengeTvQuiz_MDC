# ChallengeTvQuiz_MDC
MDC - Technical Assessment

REQUIREMENTS
A popular TV show has asked us to build a website that will allow them to publish quizzes.
• Each quiz will consist of a variable number of multiple-choice questions.
• Each question will consist of 4 possible answers.
• Every person taking part in a quiz have their results stored (and made retrievable) by email address.
• Once a person has completed a quiz, they may not do that one again
• At the end of the quiz it needs to display the users score out of the total number of questions
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

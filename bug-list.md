# Bug List

> Make a list of the things that don't work as expected. Keep a list of things that you have fixed and try to document how you solved them.

1. Problem: *I had a problem finding out how to loop through the "questions" and "correctAnswers" arrays. I was trying to do it with == but in the end I found out that using just one = solved it for the moment. And it makes sense assigning the questions to correct answers, instead of comparing them since they are not equal to each other. I'm still thinking if this is the correct approach, but I will continue and make changes along the way. Also, my score counter starts at zero from the first question in the console.log so I will try to solve that as well.*
2. I have some current problems with my program, so I might take a step back and re-do some of the code to understand it better.

- 2025-03-26 around 22:40
3. I made a function for outputting one question at a time as a test, but when I wanted to clear the previous question using an empty string, it was continuously spamming the same message. It was because I used "+=" for all the lines including in the "else" statement and after using "=" and "+=" only for the questions it fixed it. - A minute later I tested again and I realized I didn't need the empty string for the "else" statement, at least for now

2025-04-02 14:00
1. Might not be a bug but when I press the button, the score doesn't increase from 1 to 2. It stays 1 but in the console it shows 2.
2. Same day around 19:00 - I changed the name of an ID above the script tags from question to questions and forgot to change the variable,
so some kind of error occurred.

- 2025-04-08 13:50. *My buttons appear stacked on top of each other after clicking on the start quiz button.*

- 2025-04-12 17:00-18:00. *I changed name of the function "quizQuestions" to "startQuiz" because I want that to be the function to start it. However, now nothing happens when I click on it. I am trying to fix it and checking that the IDs are correct etc.*
- 2025-04-12 18:15-18:30. *I fixed the problem and now it does start again when I click on start but the 4 other buttons for answers are not connected yet to questions/correctAnswers*

- 2025-04-23 15:30-15:40 *Trying to make my quiz function properly. If I put the function 'quizQuestions() at the bottom of the other function 'startQuiz' the score in the end stays at 1 no matter what buttons were clicked. Trying to fix it. Also still have no clue yet on how to make the buttons appear horizontally instead of vertically but that still looks fine to me.*

- 2025-04-28 10:15-10:50
1. Fixed the "problem" where the buttons aligned vertically by using "inline-block instead of just block"

- 2025-04-28 10:15-11:00
1. I have a problem with the quizQuestions function and using console.log it shows undefined
- 2025-04-28 11:00-11:40 
1. I fixed a problem for the 'this' where it was showing which button was pressed, but due to using index++ in the showQuestions
function as well as in 'startQuiz' it was showing the wrong number, two as six for example. Now it shows what button was pressed correctly.

- 2025-05-04
1. Still working on the issue where my 'userClick' parameter/variable is undefined and it can't track which button was pressed. With this.innerText in the startQuiz function it's showing me in the console log that for any button that was clicked it's adding one point which should be incorrect and for the final button that I click, it doesn't show me undefined?

- 2025-05-08 23:00-00:30
1. I experimented many different ways and after getting some help with the parameter problem, the index seems to be following better. It can only go to the next question now if I click on the correct answer but I think I can fix this with an else statement. Line 71 console.log(this.innerText) is showing as undefined

- 2025-05-08 12:30-14:10 (workshop) + 30 minutes at home so far
1. I have a bug where the "score" or correct answers rather, shows as 0 in the end no matter what. Working on it. 

- 2025-05-09 23:00-01:30
1. I fixed the bug above by using the event.target property and I also changed the addEventListener buttons to my 'answerClicked' function instead to make it work as well. I also did some small changes to other things and I had to move the index++ to increment both if the correct/incorrect answer was clicked and called for the startQuiz function after it. Happy with this progress finally!
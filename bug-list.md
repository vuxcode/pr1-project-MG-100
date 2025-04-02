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
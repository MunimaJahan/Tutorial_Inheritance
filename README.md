# Inheritance_n_Polymorphism

In this exercise we are going to practice a few code related to inheritance and polymorphism. We are going to design a **Quizz** where a set of different types of questions like short question, MCQ, true/false will be displayed to the user and will collect response from the user. Also the program will check whether the response is rigth or wrong.  

# What you have in the starter code
- We have a generic class called **Question** that has two member variables **text**, **answer** and a method
called **checkAnswer** as described bellow:
- **text**: stores the description of the question
- **answer**: stores the correct answer for the question
- **checkAnswer(String ans)**: That takes the answer as an argument/parameter and checks whether it is correct or not. It returns *true* if the answer matched with the correct answer stored in the variable **answer**, otherwise returns *false*.

You also have a **Main** class that demonstrate the use of the **Qustion**.

# What you have to do

## Task 1
- Import the project in *eclipse* from the repository.
- Run the program and see how it works.
- Try to understand the code and what it is doing.

## Task 2
- Create a new class called **MCQQuestion** that extends the class **Question**.
- Your **MCQQuestion** class should have the following members:
- An ArrayList **choices** to store the list of choices for a question.
- A constructor that creates the ArrayList
- A method **addChoice(String choice, boolean correct)** that adds choices for a question and stores as the answer for the question if the correct is *true*.
- A method **display()** that overrides the display method of the super class to display the MCQ question properly with choices.
- Rewrite the **Main** class to display a MCQ question and take a response from keyboard for the answer as the choice (1,2 ..)
- Display if the answer is correct or not.
- The screen may look like:
```
In which country was the inventor of Java born?
1: Canada
2: United States
3: Denmark
4: United State
Your answer: 1
true

```
## Task 3
- Create a new class called **Quiz** that will store a list of questions.
- Add a method called **addQuestion(Question Q)** that can add any type of question in the list.
- Add a method called **allQuestions()** that returns the list of questions added to a Quiz.
- Rewrite the **Main** class that creates a **Quiz** object and adds at least three different questions with answers in order: first one is a regular question, second one is an MCQ, third one is a regular question and so on (Try to make your questions as difficult as possible).

- Now display the questions from the Quiz one at a time and take a respose from the user. 
- Display whether the result is correct or not.
- You may declare any helper method, or getter and setter or constructor if necessary.

## Task 4
- Now change the **Question** class as an Abstract class and change display as an abstract method.
- Try to run the program and see what errors you get.
- Try to fix those errors.
- Now we don't have an inherited method display.
- Create a new extended class from **Question** as **ShortQuestion**.
- Use this **ShortQuestion** as we used the generic **Question** and rewrite your program.
- Try to compile the **ShortQuestion** without overriding the **display()** method.
- Write necessary code to fix the errors.

```mermaid
flowchart TD
    Start([Start]) --> |Initialize Game| InitGame[Generate Random Number]
    InitGame --> UserInput[Get User Input]
    UserInput --> CheckInput{Is Input Valid?}
    CheckInput -- No --> InvalidInput[Prompt Invalid Input]
    InvalidInput --> UserInput
    CheckInput -- Yes --> CheckGuess{Is Guess Correct?}
    CheckGuess -- Yes --> Correct[Prompt Correct Guess]
    Correct --> End([End])
    CheckGuess -- No --> HighOrLow{Is Guess Too High?}
    HighOrLow -- Yes --> TooHigh[Prompt Too High]
    HighOrLow -- No --> TooLow[Prompt Too Low]
    TooHigh --> UserInput
    TooLow --> UserInput



Flowchart Description

1. Start: The game begins.
2. Initialize Game: A random number is generated within the predefined range.
3. Get User Input: The user is prompted to guess the number.
4. Is Input Valid?: The program checks if the user's input is valid.
   - If the input is not valid, the user is prompted to enter a valid number.
   - If the input is valid, the program checks the user's guess.
5. Is Guess Correct?: The program compares the user's guess to the random number.
   - If the guess is correct, the user is notified, and the game ends.
   - If the guess is incorrect, the program checks whether the guess is too high or too low.
6. Is Guess Too High?: The program determines if the guess is too high.
   - If the guess is too high, the user is prompted to guess a lower number.
   - If the guess is too low, the user is prompted to guess a higher number.
7. End: The game ends when the user guesses the correct number.

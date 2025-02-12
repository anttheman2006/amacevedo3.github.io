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

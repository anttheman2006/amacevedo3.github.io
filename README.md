# amacevedo3.github.io
Anthony Acevedo
amacevedo3@my.waketech.edu
This is my school account.
This is the repo for the first lab.
<h1>About Me</h1>

<h2>My Interests</h2>
<p>I love to take photography, I love gaming as well, and parkour is an enjoyable hobby as well!</p>

<h2>Websites I recommend</h2>
<ul>
[FreedomInMotionGym](https://www.freedominmotiongym.com/parkouronline)</a> - This website offers you free online videos and tutorials and live interactive sessions with a dedicated Freedom in Motion coach over video call!</li>

[GameSpot](https://www.gamespot.com/)</a> - Game Spot is a website that provides news, reviews, and other information about video games. Users can also write reviews, post on forums, and participate in tournaments.</li>
</ul>
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

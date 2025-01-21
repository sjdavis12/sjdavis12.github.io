```mermaid
flowchart TD
    A[Start Game] --> B[Generate a Random Number]
    B --> C[Ask User for a Guess]
    C --> D{Is the Input Valid?}
    D -- No --> E[Display 'Invalid Input. Try Again.']
    E --> C
    D -- Yes --> F{Is the Guess Correct?}
    F -- Too High --> G[Display 'Too High. Guess Again.']
    F -- Too Low --> H[Display 'Too Low. Guess Again.']
    F -- Correct --> I[Display 'Correct! You Win!']
    G --> C
    H --> C
    I --> J[End Game]

# Description of the Flowchart

The flowchart represents a random guessing game. Here's how it works:

1. The program starts.
2. A random number is generated.
3. The user is prompted to guess the number.
4. The program validates the input:
   - If invalid, the user gets an error message and must try again.
   - If valid, the program checks if the guess is too high, too low, or correct.
5. Feedback is provided based on the guess.
6. The game ends when the correct number is guessed.

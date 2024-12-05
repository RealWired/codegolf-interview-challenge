# RealWired Code Golf

**Author:** Alex C, lead @ RealWired

Code golf is a programming challenge where developers compete to solve a specific coding problem **using the least number of characters or bytes possible while still creating working code**. 

It's like regular golf where the lowest score wins - in this case, the score is the length of your code. While code golf solutions often sacrifice readability and best practices for brevity, they can help programmers discover creative language features and alternative approaches to problem-solving. It's common to see code golfers use obscure language features, clever variable naming, and unconventional techniques to shave off every possible character. 

The challenge isn't just about making code shorter - it's about finding ingenious ways to achieve the same output with minimal syntax, often leading to surprising and educational discoveries about the programming language being used.

## ChatGPT, etc.

These questions are designed to be resistant to LLMs because they:

1.  Require creative interpretation of unconventional input formats
2.  Combine multiple domains (music, dance, geography, etc.)
3.  Include visual or pattern-based elements
4.  Require understanding of context-dependent transformations
5.  Include elements that need human creativity to interpret

Feel free to paste them into any LLM you like, but it's going to be obvious on your second week if you did, isn't it? The idea here is fun. There aren't any "right" answers. Only the answer *you* come up with as an *individual*.

## Guidelines

-   All solutions must be valid PHP 8.x code
-   Shorter solutions (measured in bytes) score better
-   Whitespace between statements is optional
-   Input/output methods should be specified in your answer.

## Scoring System

-   Base score: Number of bytes in the answer
-   Bonus deductions:
    -   -10% for not using any built-in functions
    -   -15% for creative variable naming that still maintains readability
    -   -20% for solutions that work with multiple input formats

## Questions

### 1. Emoji Encoder
Write a function that converts a string of emotions ("happy", "sad", "angry") into corresponding emojis, but the twist is the input will be in pig latin ("appyhay", "adsay", "angryyay"). 

*Score bonus for handling multiple emotion words in a single string.*

### 2. Time Zone Tangle
Create a function that takes two city names and returns the current time difference, but the cities will be provided with their letters in reverse order ("kognaB" for "Bangkok"). 

*The challenge: Use minimal PHP date functions.*

### 3. RGB Riddle
Write a program that takes a color name in l33tspeak (e.g., "r3d", "blu3", "gr33n") and outputs its RGB values. 

*The catch: You can't use any color-related built-in functions or predefined arrays.*

### 4. Palindrome Plus

Create a function that checks if a string is a palindrome, but only after applying these rules:

-   Replace all vowels with their ASCII codes
-   Reverse every third character
-   Ignore special characters Example: "A man a plan" → "65 m97n 97 pl97n"

### 5. Binary Beats
Write a function that converts a string of musical notes (A-G) into binary, but each note must be shifted based on its position in the musical scale. 

*The twist: Input notes will be provided in NATO phonetic alphabet ("Alpha" for A, "Bravo" for B).*

### 6. Pattern Predicament
Create a function that generates a specific pattern, but the input will be provided as mathematical operations written in words ("add five multiply three"). The pattern should emerge from applying these operations sequentially.

### 7. String Scramble
Write a function that unscrambles a string, but the unscrambling key is hidden within the string itself as prime number positions. *Don't use built-in prime number functions.*

### 8. Array Acrobatics
Create a function that performs array rotation, but the rotation amount is encoded in the array values themselves as Roman numerals. Example: [I, IV, "hello", III] → rotate by 4 positions.

### 8. Function Fusion
Write a program that combines two functions into one, but the operation to combine them is specified using emoji sequences. Example: 🔄 means compose, ⚡ means parallel execution.

### 10. Recursive Riddle
Create a recursive function that solves a specific pattern, but the recursion depth is determined by converting ASCII art numbers into actual numbers. Example:

 `░░░ ░░ ░
 ░░░  = 3 levels deep`

### 11. Data Structure Dance
Implement a simple data structure, but the operations must be inferred from dance move descriptions ("twist", "slide", "jump"). Each dance move corresponds to a different data operation.

### 12. Regex Remix
Write a regex pattern that matches specific strings, but the pattern must be built using musical notes that correspond to regex special characters (♪ for ., ♫ for *, etc.).

### 13. Bitwise Ballet
Create a function that performs bitwise operations, but the operations are specified using ballet positions ("first position" = AND, "second position" = OR, etc.).

### 14. Math Morphing
Write a program that solves mathematical expressions, but numbers are represented as words from different languages randomly mixed together ("uno", "deux", "tres").

### 15. Cache Conundrum
Implement a simple caching mechanism, but the cache keys must be derived from solving riddles embedded in the input strings.

### 16. Sort Saga
Create a sorting function that works with elements that change their values based on their position in the array and the current timestamp's digits.

### 17. Hash Harmony
Write a hashing function that creates a hash based on both the input string and a melody represented as musical notes. The melody affects how characters are processed.

### 18. Queue Quest
Implement a queue where the operations are determined by solving mini word puzzles in the input. Example: "first in, ???? out" (fill in the blanks to determine operation).

### 19. Tree Traverse

Create a binary tree traversal function, but the traversal order is specified by a series of compass directions ("N" = parent, "SE" = right child, etc.).

### 20. Stack Story
Implement a stack where each operation must be inferred from a short story snippet. The challenge is parsing the story to determine the operation.

### 21. Graph Geometry
Create a function that builds a graph, but the connections are specified using geometric shapes and their properties (triangle = 3 connections, square = 4 connections).

### 22. Linked List Labyrinth
Implement a linked list where the operations are encoded in a maze pattern. The path through the maze determines the sequence of operations.

### 23. Variable Verse
Write a program where variable names must be derived from solving poetry riddles, and the operations are determined by the poem's meter.

### 24. Memory Map
Create a memory management function where the allocation requests are specified using geographical coordinates, and the memory blocks must be organized based on their relative positions.

### 25. Algorithm Alchemy
Write a function that combines multiple sorting algorithms, but the choice of algorithm at each step must be determined by solving chemical compound formulas provided as input.

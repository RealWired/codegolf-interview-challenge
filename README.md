# RealWired Code Golf

**Author:** Alex C, lead @ RealWired

Code golf is a programming challenge where developers compete to solve a specific coding problem **using the least number of characters or bytes possible while still creating working code**. 

It's like regular golf where the lowest score wins - in this case, the score is the length of your code. While code golf solutions often sacrifice readability and best practices for brevity, they can help programmers discover creative language features and alternative approaches to problem-solving. It's common to see code golfers use obscure language features, clever variable naming, and unconventional techniques to shave off every possible character. 

The challenge isn't just about making code shorter - it's about finding ingenious ways to achieve the same output with minimal syntax, often leading to surprising and educational discoveries about the programming language being used.

**Yes, this is a serious technical test.** 

## ChatGPT, etc.

These questions are designed to be resistant to LLMs because they:

1.  Require creative interpretation of unconventional input formats
2.  Combine multiple domains (music, dance, geography, etc.)
3.  Include visual or pattern-based elements
4.  Require understanding of context-dependent transformations
5.  Include elements that need human creativity to interpret

Feel free to paste them into any LLM you like, but it's going to be obvious on your second week if you did, isn't it? The idea here is *fun*. There aren't any "right" answers. Only the answer *you* come up with as an *individual*.

**You will be asked to explain what your code does in person**, so copying and pasting a guess from OpenAI's ingest of StackOverflow answers may not be the best idea.

## Guidelines

-   Must run on PHP 8.x (not on a server that's been running since the dot-com bubble)
-   Shorter code = better score (like your will to live during a production outage)
-   Whitespace is optional (like your sanity after debugging WordPress plugins)
-   Submit answers while questioning every life choice that led you here

No need, nor any extra points for putting it into a unit test or running it on the CLI. Just human review. For fun.

## Scoring System

-   Base score: Number of bytes in the answer
-   Bonus deductions:
	-   -15% for variable names that would get you fired anywhere else
	-   -20% if it works but nobody knows why
	-   -50% if you can explain it without having an existential crisis
	-   -100% if it's actually maintainable (automatic disqualification)
   
Scoring is obviously subject to arbitrary dictatorship, as normal.

## Questions

### 1. Emoji Grief Counselor

The entire dev team is having an existential crisis in pig latin. Convert their emotional breakdown ("appyhay", "adsay", "angryyay") into emojis before Tom (DevOps) starts rewriting everything in Rust. *Bonus points if you handle the Sunda's complete mental collapse in one line.*

```
Input: "appyhay adsay angryyay"
Output: "😊 😢 😠"
Pseudocode:
function convertEmotions(text):
    remove 'ay' from each word
    replace 'happy' with 😊
    replace 'sad' with 😢
    replace 'angry' with 😠
    return result
```

### 2. Time Zone Russian Roulette

Your team is distributed across time zones because management hates synchronized lunch breaks. Every city name is backwards because the last dev who touched this code was later found rocking in a corner muttering about datetime parsing. Convert "kognaB" and "kroY weN" into a time difference that explains why you're in meetings at 3AM.

```
Input: "kognaB", "kroY weN" (Bangkok, New York)
Output: 11 (hours)
Pseudocode:
function timezoneDiff(city1, city2):
    reverse both city names
    get timezone of city1
    get timezone of city2
    return absolute hour difference
```

### 3. Colour Codes of Doom

The new intern is communicating exclusively in l33tspeak (*"r3d", "blu3", "gr33n"*). Convert their cries for help into RGB values before they discover JavaScript frameworks. *No, Stack Overflow cannot save you now.*

```
Input: "r3d"
Output: "255,0,0"
Pseudocode:
function convertL33t(color):
    if color is "r3d" return "255,0,0"
    if color is "blu3" return "0,0,255"
    if color is "gr33n" return "0,255,0"
```

### 4. Palindromes From The Void

Check if a string is a palindrome after:

-   Converting vowels to ASCII because Unicode hurt you once
-   Reversing every third character because chaos is the only constant
-   Ignoring special characters (they're not special, they're just misunderstood) *Example: "A man a plan" → "Your code review has been declined"*

```
Input: "A man a plan"
Pseudocode:
function cursedPalindrome(text):
    remove special characters
    convert vowels to ASCII (a->97, e->101, etc)
    reverse every third char
    check if result equals its reverse
```

### 5. Binary Symphony of the Damned

Transform musical notes into binary, but in NATO phonetic because the senior architect (Nathan) spent too long in military middleware. Convert "Alpha" (A) through "Golf" (G) into binary. *Warning: May summon elder debugging gods.*

```
Input: "Alpha Bravo Charlie"
Output: "01000001 01000010 01000011"
Pseudocode:
function natoToBinary(notes):
    replace each NATO word with corresponding letter
    convert each letter to ASCII number
    convert each number to 8-bit binary
    join results
```

### 6. The Pattern That Stared Back

Parse mathematical operations written in words by someone who learned programming from cursed GitHub repos ("add five multiply three"). *Previous maintainer went insane trying to understand their own regex.*

```
Input: "add five multiply three"
Output: 24
Pseudocode:
function parseOperation(text):
    replace 'add' with '+'
    replace 'multiply' with '*'
    replace number words with digits
    evaluate expression
```

### 7. String Theory Gone Wrong

Unscramble a string using prime number positions determined by an algorithm that was found scribbled on the bathroom wall. *Previous maintainer left to become a goat farmer.*

```
Input: "hello world"
Output: "hlowrdell o" (characters at prime positions 2,3,5,7,11 get priority)
Pseudocode:
function unscramblePrimes(text):
    find all prime numbers up to text length
    create new string using chars at prime positions first
    append remaining characters
```

### 8. Arrays: The PTSD Chronicles

Rotate an array based on Roman numerals because the last dev who worked here really liked gladiator movies. *Warning: May cause flashbacks to algorithm classes.*

```
Input: array=[1,2,3,4], rotation="IV"
Output: [3,4,1,2]
Pseudocode:
function rotateRoman(array, numeral):
    convert Roman numeral to number (IV -> 4)
    rotate array by that many positions
```

### 8. Function Fusion: A Love Story

Combine functions using emoji as operators. 🔄 means compose, ⚡ means parallel execution, 💀 means "here be dragons". *The original documentation was found in a fortune cookie.*

```
Input: f(x)=x+1, g(x)=x*2, operator=🔄
Output: f(g(x)) -> (x*2)+1
Pseudocode:
function combineFunctions(f, g, operator):
    if operator is 🔄:
        return composition(f, g)
    if operator is ⚡:
        return parallel(f, g)
```

### 10. Recursion: The Call Stack Strikes Back

Implement recursion where depth is determined by ASCII art numbers that look like they were drawn by a caffeinated raccoon:

```
 ░░░
 ░░ ░  = The number of times your function will call itself before
 ░░░    questioning its life choices
```
```
Input:  ░░░
       ░░ ░
        ░░░
Output: function calls itself 7 times (binary 111)
Pseudocode:
function recursiveNightmare(art, depth=0):
    convert ASCII art to binary (spaces=0, ░=1)
    if depth < binary_value:
        return recursiveNightmare(art, depth+1)
    return depth
```


### 11. Data Structure Dance Party

Implement a data structure where operations are determined by dance moves ("twist", "slide", "jump"). Previous developer was a failed choreographer. *Documentation is interpretive dance only.*

```
Input: array=[1,2,3], move="twist"
Output: [3,2,1]
Pseudocode:
function danceOperation(array, move):
    if move is "twist": reverse array
    if move is "slide": remove first element
    if move is "jump": duplicate first element
```

### 12. Regex: A Horror Story

Create a regex pattern using musical notes because Jason, fixing the backend, has finally lost it. ♪ means ".", ♫ means "*", and ♬ means "oh god why". Matching groups may contain traces of developer tears.

```
Input: "♪♫♬"
Output: ".*+"
Pseudocode:
function notesToRegex(pattern):
    replace ♪ with .
    replace ♫ with *
    replace ♬ with +
    return regex_pattern
```

### 13. Bitwise Ballet of Broken Dreams

Perform bitwise operations based on ballet positions because the senior dev minored in dance. First position = AND, second position = OR, fifth position = contemplating career change.

```
Input: a=5, b=3, position="first"
Output: 1 (5 AND 3)
Pseudocode:
function bitwiseDance(a, b, position):
    if position is "first": return a AND b
    if position is "second": return a OR b
    if position is "third": return a XOR b
```

### 14. Math: The Universal Language of Pain

Solve mathematical expressions where numbers are written in different languages ("uno", "deux", "tres") because the intern tried to make the codebase more "internationally friendly". *The code review lasted six days.*

```
Input: "uno plus deux"
Output: 3
Pseudocode:
function multilingualMath(expression):
    replace each number word with digit
    replace operation words with symbols
    evaluate resulting expression
```

### 15. Cache Me Outside

Build a caching system where keys are derived from solving riddles. Previous implementation used knock-knock jokes but was deprecated due to *dad joke overflow*.

```
Input: riddle="What has four legs but can't walk?", value="table"
Output: cached with hash of riddle solution
Pseudocode:
function riddleCache(riddle, value):
    solve riddle to get key
    hash the key
    store value with hashed key
```

### 16. The Sorting Hat's Revenge

Create a sorting function where elements change value based on their position and timestamp because someone took "dynamic programming" too literally. Must work during Mercury retrograde.

```
Input: array=[1,2,3,4]
Output: sorted array with values modified by current timestamp
Pseudocode:
function timeSensitiveSort(array):
    for each element:
        modify by (element + timestamp % 10)
    sort modified values
```

### 17. Hash Browns and Other Fatal Errors

Generate a hash based on both input strings and musical notes. The last person who modified this was found humming binary code in the server room.

```
Input: text="hello", notes="CDEF"
Output: hash modified by musical notes
Pseudocode:
function musicalHash(text, notes):
    for each character in text:
        modify char value by corresponding note
    return md5 hash of result
```

### 18. Queue: The Human Centipede of Data Structures

Implement a queue where operations are determined by solving word puzzles. Example: "first in, ???? out" (fill in the blanks or fill out your resignation letter).

```
Input: "first in, last out"
Output: determines if push or pop operation
Pseudocode:
function puzzleQueue(puzzle):
    if puzzle matches "first in, * out":
        extract operation from *
        perform corresponding queue operation
```

### 19. Binary Trees: A Family Tragedy

Create a tree traversal function using compass directions because GPS was too mainstream. "N" means parent, "SE" means right child, "SW" means left child, "NW" means time to update resume.

```
Input: tree=binaryTree, direction="SE"
Output: right child of current node
Pseudocode:
function compassTraversal(node, direction):
    if direction is "N": return parent
    if direction is "SE": return rightChild
    if direction is "SW": return leftChild
```

### 20. Stack Overflow: A Biography

Build a stack where operations are inferred from story snippets. Must handle nested callbacks and crushing existential dread.

```
Input: "The tired developer pushed another callback..."
Output: push operation detected
Pseudocode:
function storyStack(story):
    if story contains "push": perform push
    if story contains "pop": perform pop
```

### 21. Graph Theory: A Cosmic Nightmare

Construct a graph using geometric shapes because apparently, circles and squares weren't confusing enough. Triangle = 3 connections of pure regret.

```
Input: "▲▲■"
Output: graph with 10 connections (2 triangles * 3 + 1 square * 4)
Pseudocode:
function shapeGraph(shapes):
    count triangles and multiply by 3
    count squares and multiply by 4
    create graph with calculated connections
```

### 22. The Linked List That Took a Wrong Turn

Parse a maze of arrows (←→↑↓) to determine node connections. Created by a developer who played too much Dungeons & Dragons. There is no exit.

```
Input: "→→↓←↑"
Output: linked list with connections based on arrows
Pseudocode:
function mazeList(arrows):
    for each arrow:
        if →: connect to next
        if ←: connect to previous
        if ↑↓: connect to parallel list
```

### 23. The Variable Names Written By A Drunk Poet

Generate variable names by solving poetry riddles written by Edgar Allan Poe's ghost after discovering *Stack Overflow*. *Points deducted if your solution makes sense.*

```
Input: "Shall I compare thee to a summer's day?"
Output: variable name based on vowel count
Pseudocode:
function poeticVariable(poem):
    count vowels in poem
    generate variable name using count
    return "r" + vowel_count
```

### 24. Memory Management: Lost in Space

Allocate memory blocks using geographical coordinates because the senior dev believes RAM is a parallel dimension. *Points deducted if your solution acknowledges reality.*

```
Input: "{lat: 45.523064, lng: -122.676483}"
Output: memory address calculated from coordinates
Pseudocode:
function geoMemory(coordinates):
    calculate hash from latitude/longitude
    map hash to valid memory address range
    allocate block at calculated address
```

### 25. The Chemical Sorting Algorithm of Madness

Sort arrays using chemical compounds as instructions. NaCl means sort ascending, C₂H₅OH means sort by blood alcohol content, and C8H10N4O2 means sort by proximity to nearest coffee machine.

```
Input: array=[3,1,4,1,5], compound="NaCl"
Output: [1,1,3,4,5] (ascending because Na=sodium)
Pseudocode:
function chemicalSort(array, compound):
    if compound contains "Na": sort ascending
    if compound contains "Cl": sort descending
    if compound is "C8H10N4O2": sort by proximity to coffee machine
```


# BONUS ROUND: TypeScript Terror

Write a sorting algorithm in **ARNOLD-C** because someone lost a bet. Must convert the following TypeScript into valid ARNOLD-C syntax while maintaining functionality. The person who approved this challenge has been fired.

TypeScript version:

```
function bubbleSort(arr: number[]): number[] {
    let swapped: boolean;
    do {
        swapped = false;
        for(let i = 0; i < arr.length - 1; i++) {
            if(arr[i] > arr[i + 1]) {
                let temp = arr[i];
                arr[i] = arr[i + 1];
                arr[i + 1] = temp;
                swapped = true;
            }
        }
    } while(swapped);
    return arr;
}
```


Bonus points if you:

-   Include "GET TO THE CHOPPER" at least 5 times
-   Make every variable name a Schwarzenegger movie reference
-   Cause the code reviewer to question their career choices
-   Successfully explain this in a job interview without crying

**Yes, this is serious.**

*Note: We are not responsible for any existential crises caused by attempting this challenge. Your therapist has been notified.*

## Judging Criteria for ARNOLD-C Challenge:

-   Must actually compile in ARNOLD-C
-   Must make senior developers question reality
-   Must include at least 3 gratuitous movie references
-   Solution should be accompanied by a letter of resignation

## Support Group Information

We maintain a 24/7 hotline for developers traumatised by this challenge. Please have your health insurance information ready.

## Final Note

Remember: In code golf, like in therapy, it's not about the destination - it's about the friends we traumatised along the way.

*Note: All solutions must come with a written apology to the next maintainer.*

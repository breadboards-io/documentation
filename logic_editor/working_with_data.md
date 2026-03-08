# Working with Data

### The "Result" Concept: Using it
In Breadboard, instructions often work like a relay race. When one instruction finishes, it "hands off" its result to the next one. This result is stored in a special keyword called it.

In the logic editor, you will often see this referred to as **"Result of..."**. You can use it in any following instruction to access the information gathered or created in the step immediately before it.


#### Example:

- **Calculate** 10 + 5
- **Log** *it (This will print 15)*


### Date Instructions
These instructions allow you to create, modify, and display time and dates.


| **Commands**                                       | **Descriptions**                                                                                                                                                                                                                                                                                                                |
|----------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Format Date** [Date] to [Format String]              | Converts a date into a readable text format. When formatting a date, use these letters to define how it looks:<br><br>- **Year**: YYYY (2024), YY (24)<br>- **Month**: MMMM (October), MMM (Oct), MM (10), M (10)<br>- **Day**: Dddd (Friday), Ddd (Fri), DD (05), D (5)<br>- **Time**: HH (24hr), hh (12hr), mm (minutes), ss (seconds), a (am/pm) |
| **Adjust Date** [Add/Remove] [number] [unit] to [date] | Shifts a date forward or backward in time (e.g., "Add 2 days to the current date").                                                                                                                                                                                                                                             |
| **Set Date** [date]'s [unit] to [number]               | Directly changes one part of a date, such as setting the day to the "1st" of the month.                                                                                                                                                                                                                                         |


### Math Instructions
Use these for calculations and managing numeric data.

| **Commands**                              | **Descriptions**                                                                                                  |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| **Calculate** [Value A] [Operation] [Value B] | Performs math operations. Supports basics like +, -, *, / and advanced functions like power, sin, or square root. |
| **Format Number** [number] to [n] decimals    | Rounds a number to a specific number of decimal places (e.g., turning 3.14159 into 3.14).                         |

### Text Instructions
These instructions help you clean, cut, and combine pieces of text.

| **Commands**                                               | **Descriptions**                                                                                                                      |
|------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| **Combine Text** [Text A] and [Text B] with [Separator]        | Joins two pieces of text together. If you provide a separator (like a space or a comma), it will be placed between them.              |
| **Split Text** [Text] by [Separator]                           | Breaks a long string into a list of items wherever it finds the separator (e.g., splitting a sentence by " " to get a list of words). |
| **Slice Text** [Text] from [Start] to [End]                    | Cuts out a specific portion of text. **Pro-Tip**: Use negative numbers to count backward from the end of the text.                        |
| **Change Case** [Text] to [lowercase / UPPERCASE / Title Case] | Automatically changes the capitalization of your text.                                                                                |
| **Replace Text** In [Text], replace [Find] with [Replace]      | Swaps out specific words or characters for something else.                                                                            |
| **Match Text** In [Text], match [Pattern]                      | Searches for a specific pattern (Regex) within the text and returns the matches.                                                      |
| **Trim Whitespace** in [Text]                                  | Removes any accidental empty spaces from the very beginning and very end of your text.                                                |



### Pro-Tip: Chaining Operations
Because of the it keyword, you can chain these together for powerful results:

1. **Get Query Param** user_name
2. **Change** Case it to uppercase
3. **Combine Text** "WELCOME " and it with ""
4. **Change** #welcome-label's **Text** to it

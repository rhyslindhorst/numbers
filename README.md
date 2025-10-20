# README for Numbers Script

## Author Information
- **Name:** Rhys Lindhorst 
- **Course:** CPSC 298 Computer Science Colloquium
- **Assignment:** Numbers Script (Odd/Even Classification)  
- **Date:** 10/16/2025 

## Program Description
This program asks the user to input a positive integer and then prints all integers from one up until and including that number. Each number is printed as odd or even thereafter. 

## Example Output
If the user enters **5**, the program should display:
```
1 Odd
2 Even
3 Odd
4 Even
5 Odd
```

## Usage
To run the script interactively:
```bash
./numbers.sh
```

To test with an input file (for example, `numbers-input`):
```bash
./numbers.sh < numbers-input
```

## How the Script Works
To achieve this task, I prompted the user to input a positive integer using 'read'. I then used a for loop to iterate number starting from one. I then used the modulo operator to determine if the number in the iteration is odd or even. I then printed the outcome.

## Core Logic Example
```bash
for (( i=1; i<=num; i++ ))
do
  if (( i % 2 == 0 ))
  then
    echo "$i Even"
  else
    echo "$i Odd"
  fi
done
```

## Testing Results
When tested with the input file `numbers-input` containing:
```
5
```
The script outputs:
```
1 Odd
2 Even
3 Odd
4 Even
5 Odd
```

You should also verify:
- That negative or zero inputs are handled gracefully (optional).  
- That input `10` produces alternating Odd/Even lines up to 10.  

## Example Validations
| Input | Output Behavior |
|--------|------------------|
| 3 | 1 Odd  2 Even  3 Odd |
| 7 | 1 Odd  2 Even  3 Odd  4 Even  5 Odd  6 Even  7 Odd |

## Challenges and Solutions
[Optional: When creating this script the only issue that I had was uploading to github. However, I did have a little bit of trouble when getting the program to analize if the numbers inside of 'numbers-input' was odd or even.]

## Resources
I used ChatGPT to help me solve how to upload the files to github when I was having a little bit of trouble.

## License
This project is part of coursework for Chapman University and is intended for educational purposes.
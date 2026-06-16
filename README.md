# Advent of Code 2024 — Day 2: Red-Nosed Reports
 
## The Problem
 
We're given a list of reports, where each report is a row of numbers. The goal is to count how many reports are **safe**.
 
A report is safe if:
- The numbers are **either all going up or all going down** (no mixing)
- Each step between two adjacent numbers is **between 1 and 3** (not too big, not too small, never flat)
### Part 2 — The Problem Dampener
 
A new rule is added: if a report is unsafe, we can try removing **one number** from it. If removing any single number makes it safe, the report still counts as safe.
 
## My Logic
 
### Part 1
1. Go through each report line by line
2. Calculate the difference between each pair of neighbouring numbers
3. Check if all differences are between +1 and +3 (increasing) OR all between -1 and -3 (decreasing)
4. If either condition is fully true, the report is safe
5. Count up all the safe reports
### Part 2
1. If a report is already safe, count it
2. If not, try removing each number one at a time and test the remaining list
3. If any single removal makes it safe, count it as safe
## My Answer
 
1. **Part 1** - 326 safe reports
2. **Part 2** - 381 safe reports

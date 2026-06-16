# Advent of Code 2024 — Day 2: Red-Nosed Reports
 
## The Problem
 
We're given a list of reports, where each report is a row of numbers. The goal is to count how many reports are **safe**.
 
A report is safe if:
- The numbers are **either all going up or all going down** (no mixing)
- Each step between two adjacent numbers is **between 1 and 3** (not too big, not too small, never flat)
## My Logic
 
1. Go through each report line by line
2. Calculate the difference between each pair of neighbouring numbers
3. Check if all differences are between +1 and +3 (increasing) OR all between -1 and -3 (decreasing)
4. If either condition is fully true, the report is safe
5. Count up all the safe reports
## How to Run
 
1. Save your puzzle input as `input.txt` in the same folder as the script
2. Run with Python: `python solution.py`
## My Answer
 
**326 safe reports**

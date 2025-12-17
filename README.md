# Canvas Student Randomizer

A lightweight, browser-based tool for randomly selecting students across multiple
Canvas gradebook CSV files.  
No backend, no data storage — everything runs locally in the browser.

## Features

- Upload **one or more Canvas gradebook CSVs** (from different courses)
- Automatically combines all students across files
- Filters to include only students who scored **≥ 1 on every assignment**
- Randomly selects the number of students you specify
- Exports selected students as a CSV

## How It Works

The app uses:
- **PapaParse** for robust CSV parsing  
- A custom eligibility filter:
  - Students must score ≥ 1 on *every* assignment column
- Fisher–Yates shuffle for random selection
- Pure client-side JavaScript (no server required)

## Usage

1. Open `canvas_student_randomizer.html` in any modern browser.
3. Select one or more Canvas CSV gradebook files.
4. Enter the number of students to randomly select.
5. View results directly on the page.
6. Optionally download the CSV output.

## File Structure


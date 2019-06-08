# test-randomizer
Script for randomizing a test. Works both for questions and answers.

## Requirements
Python3

## Installation
`pip install -r requirements.txt`

## Usage
Edit **test.docx** in order to contain all your desired questions. Questions must be written in bold, answers must have at least some non-bold character.
You can use bullets to keep everything tidy if you want but these will be ignored by the script since python-docx does not handle bullet lists very well.
However a bullet list for questions and answers will be created when generating the output. Numbers are added automatically for questions.
The script will generate a new file with 6 question per page, assuming that a question will occupy a fairly reduced amount of lines.

Images are currently not supported.

Configure quiz.py by changing the input file, the number of copies you want to obtain and whether to randomize questions and/or answers.

Run `python quiz.py` to parse test.docx and generate the new file containing the desired copies of tests with or without randomization.
This will generate the **output.docx** file, containing the tests.

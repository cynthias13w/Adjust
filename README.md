# Adjust

<a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a>

This repository serves as a demonstration of fundamental Linux skills.

## Table of Contents
- Setup
- Questions
  - Count Lines
  - Count "Z" Characters
  - Find positions of specific words
  - Replace Word
- Explanations
- Thank you

## Setup

I'm currently running Ubuntu 20.04.4 LTS (Focal Fossa). With its user-friendly interface and robust command-line capabilities, Ubuntu provides a stable platform for me to efficiently manage tasks and customize my system to fit my needs. I'm using the Zsh shell.

1️⃣ To start this task, I created this GitHub repo and cloned it locally.

Then I created the text file using the following commands:

```bash
# Create File
touch file.txt
nano file.txt
```

The text was then copied and pasted in, then saved 💾

## Questions

1. How many lines in this file?

```bash
wc -l file.txt
```

Answer: 98

2. How many “Z” Characters in this file ?
```bash
grep -o 'Z' file.txt | wc -l
```

Answer: 44

3. Find on which line is “Junior”, “Platform” and “Engineer”, not case
sensitive.
```bash
grep -in 'Junior' file.txt
grep -in 'Platform' file.txt
grep -in 'Engineer' file.txt
```

Junior: 65

Platform: 28

Engineer: 88

4. Change “Junior” to “Senior”
```bash
sed -i 's/Junior/Senior/g' file.txt
```

## Explanations

wc: "word count"

-l: Tells the wc command to count only the lines

grep: Searching for lines

-o: Output only the matching parts of the lines

'Z': Pattern to search for

|: Redirects output of previous command to input of next command.

-i: Case-insensitive

-n: Line numbering

sed: Parsing and transforming text

-i: Modifies file directly

's/Junior/Senior/g': Subsitute every occurrence of Junior with Senior. g: replace all occurrences on each line

## Thank you
Thank you for your time.

Please feel free to reach out to me.
📧 mcynsiew@gmail.com

<div style="width:100%;height:0;padding-bottom:56%;position:relative;"><iframe src="https://giphy.com/embed/MdkQdz1CG2KIymkiYr" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/brooklynninenine-nbc-brooklyn-nine-b99-MdkQdz1CG2KIymkiYr">via GIPHY</a></p>

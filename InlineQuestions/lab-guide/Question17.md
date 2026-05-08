## Metadata
Question Type : Single Choice

## Question
17. What is the AIX ODM (Object Data Manager)?

## Options
Option 1: A relational database for application data
Option 2: A binary configuration database that stores device, software, and customized object information for the AIX kernel and subsystems
Option 3: A Linux-style /etc text-file replacement that AIX dropped in 7.2
Option 4: A monitoring agent

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. ODM is AIX's binary configuration database (under /etc/objrepos and others). It holds device classes (CuDv, CuAt, PdDv), software config (LPP), and customized predefined attributes. Tools like odmget / odmadd / odmchange operate on it.

## Incorrect Answer Feedback
ODM is not a relational DB. It still exists in AIX 7.x. It is not a monitoring agent.

## Tags
AIX
ODM
Practitioner

## Number of Retries
0

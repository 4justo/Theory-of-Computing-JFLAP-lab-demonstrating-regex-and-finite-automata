# Email Validation Using Regular Expressions and Finite Automata

## Overview

This project demonstrates the use of Regular Expressions (Regex) and Finite Automata concepts to validate email addresses. The implementation was developed as part of Theory of Computing practical exercises using JFLAP and Linux command-line tools.

The project illustrates how formal language concepts can be applied to real-world pattern matching problems such as email validation.

## Objectives

* Understand the structure of valid email addresses.
* Design a Regular Expression for email validation.
* Convert the Regular Expression into a Finite Automaton using JFLAP.
* Test valid and invalid email inputs.
* Demonstrate pattern matching using Linux commands.

## Regular Expression

```regex
[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}
```

### Explanation

| Component           | Description      |
| ------------------- | ---------------- |
| `[a-zA-Z0-9._%+-]+` | Username section |
| `@`                 | Email separator  |
| `[a-zA-Z0-9.-]+`    | Domain name      |
| `\.`                | Literal dot      |
| `[a-zA-Z]{2,}`      | Top-level domain |

## Sample Input File

```text
john@gmail.com
mary@yahoo.com
invalid@email
user123@company.co.ke
test.com
```

## Linux Command Demonstration

```bash
grep -E '[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}' contacts.txt
```

### Expected Output

```text
john@gmail.com
mary@yahoo.com
user123@company.co.ke
```

## JFLAP Implementation

1. Create a Regular Expression in JFLAP.
2. Convert the expression to an NFA.
3. Test accepted and rejected strings.
4. Analyze state transitions.
5. Verify correctness of the automaton.

## Technologies Used

* JFLAP
* Kali Linux
* Regular Expressions (Regex)
* Finite Automata
* Theory of Computing Concepts

## Learning Outcomes

Through this project, I gained practical experience in:

* Designing regular expressions
* Constructing finite automata
* Pattern matching in Linux
* Applying formal language theory to real-world problems

## Author

**Symon Onoka**

Bachelor of Science in Computer Science

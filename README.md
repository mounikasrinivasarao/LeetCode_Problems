# LeetCode Daily Practice (Python)

![GitHub last commit](https://img.shields.io/github/last-commit/your-username/leetcode-daily-practice)
![GitHub repo size](https://img.shields.io/github/repo-size/your-username/leetcode-daily-practice)
![GitHub stars](https://img.shields.io/github/stars/your-username/leetcode-daily-practice?style=social)

## Table of Contents
- [Introduction](#introduction)
- [Why This Repository](#why-this-repository)
- [Repository Structure](#repository-structure)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [How to Add a New Solution](#how-to-add-a-new-solution)
- [Example Solution](#example-solution)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

Welcome to the **LeetCode Daily Practice (Python)** repository! This project is dedicated to my journey of solving one LeetCode problem every day using Python. Through consistent practice, I aim to sharpen my problem-solving skills and deepen my understanding of algorithms and data structures.

## Why This Repository

- **Consistency**: Solving a problem daily helps build and maintain coding momentum.
- **Learning**: Tackling a wide range of problems provides exposure to different algorithmic patterns.
- **Sharing**: Sharing my solutions helps others benefit from different approaches and explanations.
- **Progress Tracking**: This repository is a track record of my growth as a Python programmer.

## Repository Structure

| Folder/File                                       | Description                                               |
|---------------------------------------------------------------------------------------------------------------|
| `README.md`                                       | This file providing an overview of the repository.        |
| `solutions/`                                      | Directory containing all Python problem solutions.        |
| `solutions/YYYY-MM-DD_problem-name/`              | Sub-folder for each day's problem, named by date and name.|
| `solutions/YYYY-MM-DD_problem-name/solution.py`   | Python solution file.                                     |
| `solutions/YYYY-MM-DD_problem-name/README.md`     | Problem description and explanation.                      |
| `LICENSE`                                         | Specifies the repository's licensing.                     |

### Detailed Structure

| Path                                               | Type       | Description                                      |
|------------------------------------------          |------------|--------------------------------------------------|
| `/README.md`                                       | File       | Overview of the repository.                      |
| `/solutions/`                                      | Directory  | Contains all solution folders.                   |
| `/solutions/YYYY-MM-DD_problem-name/`              | Directory  | Folder for each daily problem.                   |
| `/solutions/YYYY-MM-DD_problem-name/solution.py`   | File       | Python solution.                                 |
| `/solutions/YYYY-MM-DD_problem-name/README.md`     | File       | Detailed problem description and approach.       |
| `/LICENSE`                                         | File       | Licensing information (e.g., MIT License).        |

## Technologies Used

- **Programming Language**: Python
- **Version Control**: Git & GitHub for tracking changes and collaboration.
- **Markdown**: For writing clear and organized documentation.

## Getting Started

### Prerequisites

- **Git**: To clone the repository.
- **Python**: For running and testing the solutions.

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/mounikasrinivasarao/LeetCode_Problems
   cd leetcode-daily-practice

Navigate to Solutions Folder

bash
Copy code
cd solutions
How to Add a New Solution
Create a New Folder

Create a folder with the current date and problem name. For example:

bash
Copy code
2024-04-27_two-sum/
Add Python Solution

Inside the folder, add your Python solution file:

Copy code
solution.py
Add Problem Description

Create a README.md inside the problem folder with the problem statement and your approach.

markdown
Copy code
# Two Sum

**LeetCode Problem:** [Two Sum](https://leetcode.com/problems/two-sum/)

## Problem Description

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

## My Approach

- **Hash Map**: Iterate through the list and store each number's index in a hash map. For each number, check if `target - number` exists in the map.
- **Time Complexity**: O(n)
- **Space Complexity**: O(n)

## Solution

Refer to `solution.py` for the Python implementation.
Commit and Push

After adding your solution, commit and push the changes to GitHub.

bash
    - git add .
    - git commit -m "Add solution for Two Sum - 2024-04-27"
    - git push origin main

**Example Solution**
Here's an example of how a solution file (solution.py) might look:

python
Copy code
# solution.py

from typing import List

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        seen = {}
        for i, num in enumerate(nums):
            complement = target - num
            if complement in seen:
                return [seen[complement], i]
            seen[num] = i
            
**Contributing**
  - Contributions are welcome! Whether it's improving existing solutions, adding new ones, or enhancing documentation, your help is appreciated.

**Fork the Repository**
     - Create a New Branch (git checkout -b feature/YourFeature)
     - Make Your Changes
     - Commit Your Changes (git commit -m 'Add some feature')
     - Push to the Branch (git push origin feature/YourFeature)
     - Open a Pull Request
     - Please ensure that your contributions adhere to the repository's coding standards and include appropriate documentation.

**License**
This project is licensed under the MIT License.

**Acknowledgements**
    - LeetCode for providing a platform with diverse and challenging coding problems.
    - GitHub for hosting the repository and enabling collaboration.
    - Markdown for easy and readable documentation formatting.

**Tips for Maintaining Your Repository**
    - Consistency: Always follow the same folder and file naming conventions.
    - Documentation: Clearly document your approach and any insights in each problem's README.md.
    - Regular Commits: Commit your solutions daily to keep track of your progress.

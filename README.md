# Python Learning & Interview Prep 🐍

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Solutions](https://img.shields.io/badge/Solutions-20%2F20%20Complete-brightgreen.svg)](#-coding-interview-solutions-table)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](#-license)

Welcome to the **Python Learning & Interview Prep** repository! A curated, practical collection of notes, cheatsheets, and coding interview solutions designed to help you master Python — from foundational syntax to cracking algorithmic technical interviews.

---

## 📑 Table of Contents

- [📚 What's Included?](#-whats-included)
- [📓 Interactive Jupyter Notebooks](#-interactive-jupyter-notebooks)
- [🧩 Coding Interview Solutions Table](#-coding-interview-solutions-table)
  - [🔤 Strings & Palindromes](#-strings--palindromes)
  - [🔢 Arrays, Lists & Hashing](#-arrays-lists--hashing)
  - [🔗 Linked Lists](#-linked-lists)
  - [🔍 Searching, Math & Logic](#-searching-math--logic)
- [🚀 How to Run the Solutions](#-how-to-run-the-solutions)
- [🗺️ Roadmap](#️-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 📚 What's Included?

This repository contains structured study guides, reference cheat sheets, interactive notebooks, and 20 fully documented Python solutions:

1. **[Python Basics Notes](Python_Basics_Notes_with_Borders.pdf)**
   - A step-by-step guide covering the fundamental concepts of Python (variables, loops, data types, functions, exception handling). Perfect for beginners or as a quick refresher.
2. **[Python Cheatsheet](Python_Cheatsheet.pdf)**
   - Rapid-fire reference covering basic syntax, control flow, built-in functions, and standard library modules (`collections`, `itertools`, `datetime`, etc.).
3. **[Interview Questions Guide](interview_questions.pdf)**
   - Core Python theory and behavioral/conceptual questions frequently asked during technical screens.
4. **[20 Coding Interview Problems Guide](20_Coding_Interview_Problems.pdf)**
   - Problem statements and thought processes for 20 classic algorithmic challenges.
5. **[Complete Python Solutions (`solutions/`)](solutions/)**
   - Clean, idiomatic, well-commented Python implementations with time/space complexities and built-in test runs.
6. **[Interactive Jupyter Notebooks (`notebooks/`)](notebooks/)**
   - Hands-on runnable `.ipynb` notebooks for core Python syntax and algorithmic problem patterns with 1-click Google Colab support.
7. **[Git Fundamentals Guide](Git_Fundamentals.pdf)** ([Markdown Reference](git_fundamentals.md))
   - Quick-reference guide covering 18 essential Git commands and workflows (`init`, `clone`, `status`, `add`, `commit`, `push`, `pull`, `fetch`, `checkout`/`switch`, `merge`, `rebase`, `log`, `diff`, `stash`, `reset`, `revert`, `cherry-pick`, and `tag`).

---

## 📓 Interactive Jupyter Notebooks

Prefer interactive learning? You can run and edit every topic directly in VS Code or in your browser using Google Colab:

| Notebook | Focus Areas | Run in Cloud |
|---|---|:---:|
| **[01: Python Fundamentals](notebooks/01_python_fundamentals.ipynb)** | Data types, comprehensions, `*args`/`**kwargs`, lambdas, exceptions | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kuvaleshcd-hue/ai-engineer-handbook/blob/main/notebooks/01_python_fundamentals.ipynb) |
| **[02: Strings & Palindromes](notebooks/02_strings_and_palindromes.ipynb)** | Two Pointers, Palindromes, Anagrams, Frequency Counting | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kuvaleshcd-hue/ai-engineer-handbook/blob/main/notebooks/02_strings_and_palindromes.ipynb) |
| **[03: Arrays, Lists & Hashing](notebooks/03_arrays_lists_and_hashing.ipynb)** | Two Sum, Duplicates, Merging Sorted Lists, Flattening, Sorting | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kuvaleshcd-hue/ai-engineer-handbook/blob/main/notebooks/03_arrays_lists_and_hashing.ipynb) |
| **[04: Searching, Math & Logic](notebooks/04_searching_math_and_logic.ipynb)** | Binary Search, Prime Check ($\mathcal{O}(\sqrt{n})$), Fibonacci, FizzBuzz | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kuvaleshcd-hue/ai-engineer-handbook/blob/main/notebooks/04_searching_math_and_logic.ipynb) |
| **[05: Linked Lists & Pointers](notebooks/05_linked_lists_and_pointers.ipynb)** | Floyd's Cycle Detection, Middle Node, Reversing Linked List | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kuvaleshcd-hue/ai-engineer-handbook/blob/main/notebooks/05_linked_lists_and_pointers.ipynb) |


---

## 🧩 Coding Interview Solutions Table

All 20 interview problems are implemented in the [`solutions/`](solutions/) directory with approach notes, Big-O complexity analyses, and test cases.

### 🔤 Strings & Palindromes

| # | Problem | Solution File | Pattern / Approach | Time | Space |
|:---:|---|---|---|:---:|:---:|
| 01 | **Reverse String** | [`01_reverse_string.py`](solutions/01_reverse_string.py) | Two Pointers (In-place swap) | `O(n)` | `O(n)` |
| 02 | **Valid Palindrome** | [`02_palindrome.py`](solutions/02_palindrome.py) | Two Pointers (Alpha-numeric filter) | `O(n)` | `O(1)` |
| 09 | **First Non-Repeating Character** | [`09_first_non_repeating.py`](solutions/09_first_non_repeating.py) | Hash Map / Frequency Table | `O(n)` | `O(1)` |
| 13 | **Valid Anagram** | [`13_anagrams.py`](solutions/13_anagrams.py) | Hash Map / Character Frequency | `O(n)` | `O(1)` |

---

### 🔢 Arrays, Lists & Hashing

| # | Problem | Solution File | Pattern / Approach | Time | Space |
|:---:|---|---|---|:---:|:---:|
| 06 | **Find Duplicates in List** | [`06_duplicates.py`](solutions/06_duplicates.py) | Hash Set (Seen tracking) | `O(n)` | `O(n)` |
| 07 | **Element Frequency Count** | [`07_frequency.py`](solutions/07_frequency.py) | Hash Map / `collections.Counter` | `O(n)` | `O(k)` |
| 08 | **Two Sum** | [`08_two_sum.py`](solutions/08_two_sum.py) | Hash Map (Complement lookup) | `O(n)` | `O(n)` |
| 10 | **Merge Two Sorted Lists** | [`10_merge_sorted_lists.py`](solutions/10_merge_sorted_lists.py) | Two Pointers (Merge step) | `O(n + m)` | `O(n + m)` |
| 11 | **Flatten Nested List** | [`11_flatten_list.py`](solutions/11_flatten_list.py) | Recursion / Depth-First Traversal | `O(n)` | `O(d)` |
| 15 | **Find Max and Min Elements** | [`15_max_min.py`](solutions/15_max_min.py) | Linear Scan (Single pass) | `O(n)` | `O(1)` |
| 16 | **Remove Duplicates (Preserve Order)** | [`16_remove_duplicates_order.py`](solutions/16_remove_duplicates_order.py) | Set + Order Preservation | `O(n)` | `O(n)` |
| 17 | **Sort Dictionary by Value** | [`17_sort_dict.py`](solutions/17_sort_dict.py) | Key Function (`lambda` / Sorting) | `O(n log n)` | `O(n)` |

---

### 🔗 Linked Lists

| # | Problem | Solution File | Pattern / Approach | Time | Space |
|:---:|---|---|---|:---:|:---:|
| 19 | **Detect Cycle in Linked List** | [`19_detect_cycle.py`](solutions/19_detect_cycle.py) | Floyd's Cycle-Finding (Tortoise & Hare) | `O(n)` | `O(1)` |
| 20 | **Find Middle of Linked List** | [`20_middle_linked_list.py`](solutions/20_middle_linked_list.py) | Fast & Slow Pointers | `O(n)` | `O(1)` |

---

### 🔍 Searching, Math & Logic

| # | Problem | Solution File | Pattern / Approach | Time | Space |
|:---:|---|---|---|:---:|:---:|
| 03 | **Factorial (Recursive & Iterative)** | [`03_factorial.py`](solutions/03_factorial.py) | Recursion vs Loop | `O(n)` | `O(n)` rec / `O(1)` iter |
| 04 | **Fibonacci Sequence** | [`04_fibonacci.py`](solutions/04_fibonacci.py) | Iterative Generator | `O(n)` | `O(n)` |
| 05 | **Prime Number Check** | [`05_prime.py`](solutions/05_prime.py) | Optimized Trial Division up to $\sqrt{n}$ | `O(√n)` | `O(1)` |
| 12 | **Swap Two Numbers** | [`12_swap_numbers.py`](solutions/12_swap_numbers.py) | Tuple Unpacking / Math / Bitwise XOR | `O(1)` | `O(1)` |
| 14 | **FizzBuzz** | [`14_fizzbuzz.py`](solutions/14_fizzbuzz.py) | Modulo Logic / Control Flow | `O(n)` | `O(1)` |
| 18 | **Binary Search** | [`18_binary_search.py`](solutions/18_binary_search.py) | Divide and Conquer / Binary Search | `O(log n)` | `O(1)` |

---

## 🚀 How to Run the Solutions

Each solution file is standalone and can be executed directly using Python 3:

```bash
# Clone the repository
git clone https://github.com/kuvaleshcd-hue/ai-engineer-handbook.git
cd ai-engineer-handbook

# Run any solution file directly
python3 solutions/01_reverse_string.py
python3 solutions/08_two_sum.py
python3 solutions/19_detect_cycle.py
```

---

## 🗺️ Roadmap

- [x] Complete optimal Python implementations for all 20 interview problems (`solutions/`).
- [ ] Add an automated `pytest` test suite with edge-case validation.
- [ ] Set up GitHub Actions CI workflow for automated testing on push and PR.
- [ ] Add an `advanced/` guide covering Decorators, Generators, Context Managers, and `asyncio`.
- [x] Create interactive Jupyter Notebooks (`.ipynb`) for hands-on exercises.
- [ ] Implement foundational data structures from scratch (BST, Doubly Linked List, Heap, Trie).

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
1. Fork this repository.
2. Create your feature branch (`git checkout -b feature/new-problem-or-topic`).
3. Commit your changes (`git commit -m 'Add solution or guide'`).
4. Push to the branch (`git push origin feature/new-problem-or-topic`).
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE). Feel free to use these notes and solutions for your personal learning and interview preparation! not more 
   

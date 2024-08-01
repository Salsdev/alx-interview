# 0x01. Lockboxes

**Algorithm | Python**

**Author:** Carrie Ybay, Software Engineer at Holberton School

## Project Description

This project explores the Lockboxes Challenge, focusing on efficient algorithm implementation in Python. The goal is to determine if a set of numbered boxes, each potentially containing keys to other boxes, can all be unlocked starting with the first box.

## Lockboxes Challenge

You are given `n` locked boxes numbered from 0 to `n - 1`. Each box may contain keys to other boxes.

**Task:**

Write a method `canUnlockAll(boxes)` that determines if all boxes can be opened.

**Conditions:**

- `boxes` is a list of lists representing the boxes and their contents.
- A key with the same number as a box opens that box.
- All keys are positive integers.
- There may be keys that do not correspond to any box.
- The first box, `boxes[0]`, is unlocked.
- Return `True` if all boxes can be opened, otherwise return `False`.

**Example:**
```python
boxes = [[1], [2], [3], [4], []]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
print(canUnlockAll(boxes))  # Output: False

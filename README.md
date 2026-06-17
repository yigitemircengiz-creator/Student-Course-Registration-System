# Student Course Registration System

A console-based Student Course Registration System developed in C for the CENG110 – Programming and Computation II course.

## 🚀 Overview
This project is a fully encapsulated system that allows for the management of students and courses. It supports adding, removing, searching, and sorting operations, alongside a robust registration mechanic allowing students to enroll in or drop courses with full validation.

## 🏗️ Architecture
The system is built using three primary Abstract Data Types (ADTs):
* **Student ADT:** Stores numeric ID, full name, academic year, and enrolled courses.
* **Course ADT:** Manages course ID, name, maximum capacity, and current enrollment count.
* **RegistrationManager ADT:** The central coordinator owning two singly-linked lists (for students and courses) that handles all higher-level operations.

All internal representations are strictly encapsulated, with interactions happening exclusively through function interfaces.

## 📊 Data Structures & Algorithms
* **Singly-Linked Lists:** Both student and course collections utilize singly-linked lists with O(1) head insertion. This was chosen to support dynamic sizing without fixed upper bounds.
* **Time Complexity:**
  * Add / Register / Drop: O(n).
  * Remove / Search: O(n) worst case.
  * Sort (Insertion Sort): O(n²).

## ⚙️ How to Build & Run
The project includes a standard `Makefile` for easy compilation.
1. Open your terminal in the project directory.
2. Compile the source code by running:
   ```bash
   make

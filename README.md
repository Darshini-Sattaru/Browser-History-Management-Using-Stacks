🌐 Browser History Management Using Two Stacks in C

📌 Overview

A menu-driven C application that simulates browser navigation using two stacks implemented with linked lists. It supports visiting pages, navigating backward and forward, displaying browsing history, and clearing history.

This project demonstrates the practical application of stack operations and dynamic memory management to a real-world navigation problem.

✨ Features

- Visit Page: Opens a new page and updates browsing history.
- Back & Forward Navigation: Moves between previously visited pages.
- Current Page: Displays the currently open page.
- Browsing History: Displays the back stack, current page, and forward stack.
- Clear History: Clears both stacks and resets the current page.
- Input Validation: Handles invalid choices, empty URLs, and excessively long URLs.
- Memory Management: Uses dynamic memory allocation and safely frees allocated nodes.

🧠 Concepts Used

- Stack Data Structure (LIFO)
- Linked Lists
- Pointers and Structures in C
- Dynamic Memory Allocation ("malloc()" and "free()")
- Input Validation and Error Handling

⚙️ How It Works

The application maintains three components:

- Back Stack: Stores previously visited pages.
- Forward Stack: Stores pages available for forward navigation.
- Current Page: Stores the page currently being viewed.

Operation| Description
Visit| Saves the current page in the back stack and clears forward history.
Back| Moves the current page to the forward stack and restores the previous page.
Forward| Moves the current page to the back stack and restores the next page.
Clear History| Empties both stacks and resets the current page.

Key behavior: Visiting a new page after navigating backward clears the forward history, just as expected in standard browser navigation.

🛠️ Technologies Used

- Language: C
- Data Structures: Stacks and linked lists
- Libraries: "stdio.h", "stdlib.h", "string.h"
- Compiler: GCC

🚀 Getting Started

Compile

gcc browser_history.c -o browser_history

Run

Linux/macOS:

./browser_history

Windows:

browser_history.exe

⏱️ Complexity Analysis

Let "n" represent the number of pages stored in the stacks.

Operation| Time Complexity
Push / Pop| O(1)
Back / Forward| O(1)
Show Current Page| O(1)
Display History| O(n)
Clear History| O(n)

Space Complexity: O(n)

📚 Key Takeaways

- Applied stack operations to simulate browser navigation.
- Implemented stacks using linked lists.
- Practiced dynamic memory allocation and memory cleanup.
- Handled edge cases and invalid user inputs.
- Understood how data structures support real-world applications.

👩‍💻 Author

Darshini Sattaru

Computer Science Student | Data Structures & Algorithms

---

⭐ If you find this project interesting, feel free to explore the code!

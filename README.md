# Library Management System (C++)

This project is a simple **Library Management System** implemented in C++. It allows users to manage a collection of books with functionalities to **create**, **update**, **display**, and **delete** book records. The system uses an **AVL Tree** for efficient data management, along with additional data structures like **doubly linked lists**.

## Features

- 📚 Add new book records with:
  - ISSN (unique identifier)
  - Title
  - List of Authors
  - Total Copies
  - Copies Available
- ✏️ Update existing book records
- 🔍 Display individual records by ISSN
- ❌ Delete records by ISSN
- 🔁 Handles invalid or non-existent record operations gracefully

## Project Structure

- `main.cpp`: Demonstrates the use of the `Library` class with test records and operations.
- `Library.h / Library.cpp`: Main class to manage the collection of book records.
- `Record.h / Record.cpp`: Defines the structure and data for each book record.
- `AVL.h / AVL.cpp`: Provides an AVL Tree implementation for efficient record storage and lookup.
- `Doubly.h / Doubly.cpp`: Implements a doubly linked list, possibly used for managing authors or related metadata.
- `Node.h`: Defines nodes used in AVL Tree.

## Example Usage

The current `main.cpp` does the following:

1. Creates two book records:
   - `ISSN: 420` - *Data Structures And Algo* by *Faisal Aslam*
   - `ISSN: 6940` - *Discrete Structures* by *Laila Yawar* and *Sarah Ahmad*
2. Displays the record with ISSN `420`.
3. Updates the record with ISSN `420`.
4. Displays the updated record.
5. Deletes the record with ISSN `420`.
6. Attempts to display the deleted record.
7. Tries to delete a non-existent record (`69420`).
8. Displays the remaining valid record (`6940`).

## How to Compile

Make sure all the `.cpp` and `.h` files are in the same directory. Then compile using g++:

```bash
g++ main.cpp Record.cpp AVL.cpp Doubly.cpp Library.cpp -o LibrarySystem
```

Then run:

```bash
./LibrarySystem
```

## Dependencies

- Standard C++17 or later
- No external libraries required

## Author

**Azib Naeem**  
📧 azibnaeem17official@gmail.com

---

Feel free to fork this project and build upon it to include more features like searching by author name, issuing books to users, persistent storage, and a GUI!


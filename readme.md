# Design a Library Management System

<img src="./color-library.webp" width="500" height="500">

This exercise provides a solid foundation in understanding how to create ERDs, identify entities and their relationships, and how to define the attributes of each entity. As you become more comfortable with ERDs, you can increase the complexity of the systems you design.

## Objective

Create an ERD for a Library Management System. The system should be able to track books, borrowers, and loans.

### Step 1: Identify Entities

Start by identifying the key entities involved in a library management system. For this exercise, consider the following entities:

- **Book:** Represents the books available in the library.

- **Borrower:** Represents the individuals who can borrow books from the library.

- **Loan:** Represents the transaction of borrowing a book.

### Step 2: Define Attributes for Each Entity

Next, define some attributes for each entity. Attributes are the properties or details we want to store for each entity.

**Book**

- BookID (Primary Key)
- Title
- Author
- ISBN
- PublicationYear

**Borrower**

- BorrowerID (Primary Key)
- Name
- Email
- MembershipDate

**Loan**

- LoanID (Primary Key)
- BookID (Foreign Key from Book)
- BorrowerID (Foreign Key from Borrower)
- LoanDate
- DueDate
- ReturnDate

### Step 3: Identify Relationships

Determine how these entities interact with each other and the nature of these relationships.

- A Book can be borrowed by many Borrowers over time, but each Loan transaction involves only one Book at a time.

- A Borrower can have multiple Loans over time, but each Loan is associated with only one Borrower at a time.

### Step 4: Draw the ERD

Using the information above, draw the ERD. This involves creating rectangles for each entity, listing their attributes within, and connecting the entities with lines to represent relationships. Indicate the type of relationship (one-to-many, many-to-many, etc.) with appropriate symbols near the connecting lines (crow's feet for many, a single line for one).

Use a line with a crow's foot near the Loan entity to connect Book and Loan indicating a one-to-many relationship (a book can be involved in many loans).

Similarly, connect Borrower and Loan to indicate that a borrower can have many loans.

Here is a really nice key (but note, there are a lot of different flavors to these symbols)
![](https://cacoo.com/wp-app/uploads/2018/05/ER-notation-1.png)

**Step 5: Review and Revise**

Review the ERD to ensure it accurately represents the system and revise as needed.

Check for:

- Missing entities or attributes.
- Incorrect relationships.
- Redundant data that could be normalized.

### Submission

If you drew your ERD on paper, you may take a photo and attach it to this repo. Make a pull request. Submit the pull on Canvas.

If you used an ERD application and have a public shareable link, submit the application link in canvas instead of this repo.

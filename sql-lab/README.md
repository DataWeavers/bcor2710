# SQL Lab

A browser-based SQL workspace for BCOR 2710 (Business Information Technology) at Loyola Marymount University, used in the database sessions (D1 to D5), Assignment 3 and Exam 4.

It holds a real SQLite engine (sql.js, MIT license) inside one web page. Students see their tables and relationships the way Access shows them, run SQL, and keep everything in their own browser. Nothing is sent anywhere.

## Using it

Open `index.html` from the Pages link for this folder, or open the file itself in any browser. No install, login or server is needed.

- **Relationships** draws the ERD: primary and foreign keys, with 1 and ∞ or crow's foot line ends. Hovering a column shows what it means. In a database you build, drag a column onto another table's primary key (or a primary key onto another table's title) to relate them; **Arrange** lays the tables out again.
- **Design** builds tables and relationships without SQL, the way Access's table designer and Relationships window did: column names, types (text, integer, real, date, yes/no), primary keys (one column or two), required fields, and what each column means. Relationships are one-to-many or one-to-one with a real foreign key, or a sketch with any cardinality and no keys yet (for drawing an ERD before keys are taught; a many-to-many sketch waits for a composite entity). Every change runs real SQL, shown in a log. The course database is locked here.
- **Browse** shows each table's rows, with "What the columns mean" above them. In a database you build, it also adds and deletes rows, and explains in plain words when a row breaks a rule.
- **Query** runs SQL (Ctrl/⌘ + Enter). Each result shows its row count, including "0 rows" when a query finds nothing.
- **Database** picks the course database (Bluff Trail Outfitters, the company from the Odoo ERP lab) or an empty database for building your own tables. Adding `?db=empty` to the link opens the empty one on the Design tab; `?tab=query` (or `rel`, `design`, `browse`) picks the opening tab.
- **Download my copy** saves the database with your changes, including the diagram layout and relationship names; **Open a database file** reopens it later.
- **Save queries (.sql)** and **Open queries (.sql)** move query text between computers. Query text is also kept in the browser automatically.
- **Copy schema for AI** copies the table definitions only (no data rows) to paste into an AI tool.

## Checking a browser

`check.html` is the same page with a built-in test. It runs 25 checks when it opens and lists PASS or FAIL at the top. Use it on a new computer or browser before class.

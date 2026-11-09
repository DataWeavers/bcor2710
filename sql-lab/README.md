# SQL Lab

A browser-based SQL workspace for BCOR 2710 (Business Information Technology) at Loyola Marymount University, used in the database sessions (D3 to D5), Assignment 3 and Exam 4.

It holds a real SQLite engine (sql.js, MIT license) inside one web page. Students see their tables and relationships the way Access shows them, run SQL, and keep everything in their own browser. Nothing is sent anywhere.

## Using it

Open `index.html` from the Pages link for this folder, or open the file itself in any browser. No install, login or server is needed.

- **Relationships** draws the ERD: primary and foreign keys, and 1 to ∞ lines. Hovering a column shows what it means.
- **Browse** shows each table's rows, with "What the columns mean" above them.
- **Query** runs SQL (Ctrl/⌘ + Enter). Each result shows its row count.
- **Database** picks the course database (Bluff Trail Outfitters, the company from the Odoo ERP lab) or an empty database for building your own tables. Adding `?db=empty` to the link opens the empty one.
- **Download my copy** saves the database with your changes; **Open a database file** reopens it later.
- **Save queries (.sql)** and **Open queries (.sql)** move query text between computers. Query text is also kept in the browser automatically.
- **Copy schema for AI** copies the table definitions only (no data rows) to paste into an AI tool.

## Checking a browser

`check.html` is the same page with a built-in test. It runs 20 checks when it opens and lists PASS or FAIL at the top. Use it on a new computer or browser before class.

---

## How to Run

 **Create Schema:** Open `library_schema.sql`, copy contents, paste into [SQLite Online](https://sqliteonline.com/), and click **"Run"**. You should see eight tables appear on the left.

 **Import Data:** Import the 8 CSV files from the `CSVs/` folder using the **File -> Import -> CSV** menu.
    * **IMPORTANT:** You *must* check the box **"First line contains column names"**.
    * **IMPORTANT:** Import in this order:
        1.  `authors`, `books`, `branches`, `patrons`
        2.  `book_authors`, `copies`
        3.  `loans`
        4.  `fines`

  **Run Reports & Views:**
    * Open `reports.sql`, and run any query.
    * Open `views.sql`, run the entire file to create the views. You can then query them (e.g., `SELECT * FROM v_patron_activity;`).

  **Run Checks:**
    * Run the queries in `dq_checks.sql` (they should return 0 rows).
    * Run the steps in `performance.md` to see how indexes improved query speed.

---

## 📁 Project Files

* `README.md`
* `ERD.png`
* `library_schema.sql`
* `reports.sql`
* `views.sql`
* `dq_checks.sql`
* `performance.md`
* `CSVs/` (Folder with 8 data files)

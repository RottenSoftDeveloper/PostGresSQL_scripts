```markdown
# CSV to PostgreSQL Data Importer

A Python script to automate the process of importing data from multiple CSV files into a PostgreSQL database. The script reads all CSV files from a specified directory, combines them into a single dataset, and uploads the data to a PostgreSQL table, replacing any existing data.

---

## 🚀 Features

- **Batch CSV Import**: Reads all `.csv` files in a specified directory.
- **Data Concatenation**: Combines data into a single DataFrame for seamless upload.
- **PostgreSQL Integration**: Replaces the specified table with the new data.
- **Lightweight and Fast**: Uses `pandas` and `SQLAlchemy` for efficient data processing.

---

## 🛠 Prerequisites

- **Python 3.x** installed on your system.
- Required Python libraries:
  - `pandas`
  - `sqlalchemy`
  - `psycopg2` (PostgreSQL driver)
- Access to a PostgreSQL database.

---

## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/csv-to-postgresql.git
   cd csv-to-postgresql
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Update the script with your PostgreSQL connection details and CSV directory path.

---

## ⚙️ Configuration

### Database Connection

Edit the following details in the script:

```python
# PostgreSQL connection details
db_name = 'database_name'
table_name = 'table_name'
username = 'username'
password = 'password'
host = '127.0.0.1'
port = '5432'
```

### CSV Directory

Set the path to the folder containing your CSV files:

```python
# Directory containing the CSV files
directory = r'C:\path\to\your\csv\files'
```

---

## ▶️ Usage

1. Place all `.csv` files in the specified directory.
2. Run the script:
   ```bash
   python csv_to_postgresql.py
   ```
3. The script will:
   - Read all `.csv` files in the directory.
   - Combine them into a single dataset.
   - Replace the specified table in the PostgreSQL database with the combined data.

---

## 📁 Directory Structure Example

```plaintext
csv-to-postgresql/
│
├── csv_to_postgresql.py
├── requirements.txt
├── README.md
└── data/
    ├── file1.csv
    ├── file2.csv
    └── file3.csv
```

---

## 📊 Output

- **Database Update**:
  - The PostgreSQL table is replaced with the combined data from the CSV files.
- **Console Feedback**:
  - Displays success upon completion:
    ```plaintext
    Data imported successfully!
    ```

---

## 🔔 Notes

- All CSV files should have a consistent structure (e.g., same columns and data types).
- Make sure your PostgreSQL credentials and table permissions allow for replacing the table data.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🧑‍💻 Author

**Fabien N.**  
_“Automate smarter, not harder.”_
```

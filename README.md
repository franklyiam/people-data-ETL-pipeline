
# Simple ETL Pipeline

This project implements a basic ETL (Extract, Transform, Load) pipeline in Python. It extracts data from multiple file formats (CSV, JSON, XML), performs simple transformations (unit conversions and formatting), and loads the cleaned data into a consolidated CSV file. The process includes logging at each major step for traceability.

## 🛠️ Features

- Extracts data from:
  - CSV files
  - JSON files (line-delimited)
  - XML files (custom structure)
- Transforms data by:
  - Converting height from inches to meters
  - Converting weight from pounds to kilograms
  - Capitalizing names
- Loads data into a CSV file
- Logs progress of each ETL phase with timestamps

## 🧪 Example Output

```
Transformed Data
       name  height  weight
0      John    1.75    70.3
1     Alice    1.62    59.0
...
```

## 🗂️ Project Structure

```
.
├── etl_pipeline.py         # Main ETL script
├── log_file.txt            # Log file with timestamps and phase messages
├── transformed_data.csv    # Output CSV after loading
├── *.csv / *.json / *.xml  # Input data files (placed in the same directory)
```

## 🚀 How to Run

1. Clone this repository or download the script:
   ```bash
   git clone https://github.com/your-username/simple-etl-pipeline.git
   cd simple-etl-pipeline
   ```

2. Add your `.csv`, `.json`, and `.xml` data files to the project directory.

3. Run the ETL pipeline:
   ```bash
   python etl_pipeline.py
   ```

4. Check the output:
   - `transformed_data.csv` for the cleaned data
   - `log_file.txt` for process logs

## 📝 Notes

- JSON files should be newline-delimited (`.jsonl`)
- XML files must have the structure:
  ```xml
  <root>
    <person>
      <name>John</name>
      <height>68</height>
      <weight>155</weight>
    </person>
    ...
  </root>
  ```

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Made with ❤️ for data processing enthusiasts.

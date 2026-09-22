---
tags:
  - data-analysis
  - dataframe
  - csv
---

```python 
def csv_to_pd(file_path):
    try:
        with open(file_path, 'rt') as f:
            reader = csv.reader(f, delimiter=';')
                        
            # Read the first row to get the column names
            column_names = next(reader)
            df = pd.DataFrame(reader, columns=column_names)
        return df
        
    except Exception as e:
        print(f"Error reading {file_path}: {e}")
        return None
```


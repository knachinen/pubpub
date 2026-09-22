---
title: joblib - save & load variables
tags:
  - python
  - joblib
  - save
  - load
  - variable
---

...

변수를 파일로 저장하고 로딩하는 모듈.  
pickle 대신 joblib 를 씀.  


```python
import os
import joblib
import logging

from datetime import datetime

def ensure_directory_exists(directory: str) -> None:
    """
    Ensures a directory exists, creates it if it doesn't.

    Parameters:
    - directory: The directory path.
    """
    if not os.path.exists(directory):
        os.makedirs(directory)


def rename_existing_file(file_path: str) -> None:
    """
    Renames an existing file by appending the current timestamp.

    Parameters:
    - file_path: The path of the existing file.
    """
    timestamp = datetime.now().strftime('%Y%m%d_%H%M%S')
    new_name = f"{os.path.splitext(os.path.basename(file_path))[0]}_{timestamp}.pkl"
    new_file_path = os.path.join('save', new_name)
    os.rename(file_path, new_file_path)
    logging.info(f'Renamed existing file to: {new_file_path}')


def save_var(var, name: str = "var") -> None:
    """
    Saves a variable to a pickle file.

    Parameters:
    - var: The variable to be saved.
    - name (optional): The name of the pickle file (without extension). Defaults to "var".
    """
    ensure_directory_exists('save')
    file_path = os.path.join('save', f'{name}.pkl')

    if os.path.exists(file_path):
        rename_existing_file(file_path)

    try:
        with open(file_path, 'wb') as f:
            joblib.dump(var, f)

        file_size = os.path.getsize(file_path) / (1024 ** 2)  # Get size in MB
        logging.info(f'Saved: {file_path} (Size: {file_size:.2f} MB)')
    except Exception as e:
        logging.error(f"Error saving variable to {file_path}: {e}")


def load_var(name: str = "var"):
    """
    Loads a variable from a pickle file.
    
    Parameters:
    - name (optional): The name of the pickle file (without extension). Defaults to "var".
    
    Returns:
    - Loaded variable.
    """
    ensure_directory_exists('save')
    file_path = os.path.join('save', f'{name}.pkl')
    
    try:
        with open(file_path, 'rb') as f:
            # var = pickle.load(f)
            var = joblib.load(f)
        
        file_size = os.path.getsize(file_path) / (1024 ** 2)  # Get size in MB
        logging.info(f'Loaded: {file_path} (Size: {file_size:.2f} MB)')
        return var
    except Exception as e:
        logging.error(f"Error loading variable from {file_path}: {e}")
        return None
```


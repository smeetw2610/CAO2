# Student Information Filter Using YAML

## Overview
This project is a simple Python application that reads student information from a YAML file and provides functionalities to display all students and filter them based on their GPA.

## Features
- Load student data from a YAML file.
- Display all student details.
- Filter students based on a minimum GPA provided by the user.

## Prerequisites
Ensure you have Python installed on your system. You also need the PyYAML library, which you can install using:

```sh
pip install pyyaml
```

## File Structure
```
|-- students.yaml  # Contains student data
|-- app.py         # Main Python script
|-- README.md      # Project documentation
```

## students.yaml (Sample Data)
```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
  - name: Charlie
    age: 20
    major: Physics
    gpa: 3.9
  - name: David
    age: 23
    major: Chemistry
    gpa: 3.2
  - name: Eva
    age: 21
    major: Computer Science
    gpa: 3.7
```

## Usage

1. Clone the repository or download the files.
2. Ensure `students.yaml` is in the same directory as `app.py`.
3. Run the script using:

```sh
python app.py
```

4. The script will display all students and then prompt you to enter a minimum GPA for filtering.
5. It will then display students who have a GPA equal to or above the specified value.

## Expected Output
```
All Students:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Bob, Age: 22, Major: Mathematics, GPA: 3.5
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: David, Age: 23, Major: Chemistry, GPA: 3.2
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7

Enter minimum GPA to filter students: 3.6

Students with GPA >= 3.6:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7
```

## Additional Features
- The code is structured in functions for better readability and maintainability.
- Uses `yaml.safe_load()` to safely read YAML data.
- Handles invalid inputs gracefully.

## License
This project is open-source and free to use. Modify and enhance as needed!

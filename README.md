# Java Class Dependency Analyzer

## Description

This project is a tool for analyzing Java projects and obtaining detailed information about classes and their dependencies. It allows you, given a directory and a specific class, to determine all the classes that this class recursively uses, along with their attributes and constructors.

The program is especially useful for generating request or response templates for testing in applications with artificial intelligence. It recognizes Lombok annotations that automatically generate constructors.

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/Manflack/recursively-java-objects.git
   ```
   
2. Navigate to the project directory:

   ```bash
   cd recursively-java-objects
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```
   
## Usage

To run the program, use the following command, providing the path to the base directory of the project and the full name of the class to analyze:

```bash
python main.py /path/to/project package.name.TargetClass
```

For example:

```bash
python main.py /home/user/my_project com.example.MyClass
```

## Notes

- Ensure that the project's base directory contains `.java` source files.
- The program may take a while to build the class index, depending on the size of the project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.


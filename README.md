# generate-array-files

A Java utility that generates sequential and random integer arrays and saves them to comma-separated text files.

---

## About

Written in Java, this program fills an integer array with values, writes the array to a `.txt` file with values separated by commas and grouped ten per line, and reads the file back into memory. It also provides a helper method for generating arrays of random integers up to a configurable maximum value.

## Usage

Run the program once. It will:

1. Generate a sequential array of integers from `0` to `arraySize - 1`.
2. Write that array to `input1000000BestCase.txt` in the working directory.
3. Read the file back and load the values into a new array.
4. Print `Done!` when the write step is complete.

No command-line arguments are required.

---

## Getting Started

### Prerequisites

- Java 17 or later
- Maven 3.5+

### Building

**Unix / macOS**
```bash
mvn package
```

**Windows**
```cmd
mvn package
```

### Running

**Unix / macOS**
```bash
java -cp target/GenerateArraysFiles-1.0-SNAPSHOT.jar Main
```

**Windows**
```cmd
java -cp target\GenerateArraysFiles-1.0-SNAPSHOT.jar Main
```

---

## Configuration

The following constants are defined directly in `Main.java` and can be changed before building.

| Constant | Location | Default | Description |
|---|---|---|---|
| `arraySize` | `main()` | `1000000` | Number of elements in the generated array |
| `maxIntegerSize` | `generateArray()` parameter | n/a | Upper bound (inclusive) for random integer generation |
| Output filename | `main()` | `input1000000BestCase.txt` | Name of the file written and read back |

---

## License

MIT - see [LICENSE](LICENSE).

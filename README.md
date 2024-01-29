# shellxec

`shellxec` is a Python library for running shell commands on both Windows and Linux systems.

## Installation

You can install `shellxec` using pip:

```bash
pip install shellxec
```

## Usage

### Basic Usage

Import the `ShellExec` class and create an instance:

**Basic example to compile a CPP/C++ file**
```python
import shellxec as sx

command = "g++ main.cpp" 
sx.run_command(command)
```

#### Run a Shell Command

```python
command = "echo 'Hello, ShellExec!'"
shellexec.run(command)
```

#### Run a Shell Command and Capture Output

```python
command = "echo 'Hello, ShellExec!'"
output = shellexec.run_output(command)
print("Output:", output)
```

### Advanced Usage

#### Run a Command in a Specific Directory

```python
command = "ls"
directory = "/path/to/directory"
shellexec.run_in_directory(command, directory)
```

#### Run a Command with Custom Environment Variables

```python
command = "echo $MY_VARIABLE"
env = {"MY_VARIABLE": "Hello from ShellExec"}
shellexec.run_with_env(command, env)
```

#### Run a Batch of Commands

```python
commands = ["echo 'Command 1'", "echo 'Command 2'", "echo 'Command 3'"]
shellexec.run_batch(commands)
```

## Running Tests

To run the tests, use the following command:

```bash
python -m unittest test_shellxec.py
```

## Contributing
**Status**: Not open

Contributions are not open for this project yet. Please check again in a week to stay updated for the status!
<!-- Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests. -->

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

In this template:

- The "Installation" section provides a simple installation command using pip.
- The "Usage" section includes basic and advanced usage examples, demonstrating how to run commands, capture output, and use additional features.
- The "Running Tests" section includes instructions for running tests.

You can customize this template further based on your specific library features and requirements. If you have any additional sections or specific information you'd like to include, feel free to let me know!
# `@entry`

Tired of the traditional python `if __name__ == '__main__':` pattern? Try `@entry` instead!

`@entry` is designed to be a simple decorator for declaring main functions in python. In the backend, the same module name check is performed, but it keeps your code a little cleaner.

## Usage

**Simple example:**

```python
from atentry import entry

@entry
def main():
    print("Hello, world!")
```

**Using a return value:**

```python
from atentry import entry

@entry
def main() -> int:
    print("Hello, world!")
    return 128 # Program exit code
```

## Installation

Loading this library in your project is as simple as:

```sh
# Using Poetry
poetry add atentry

# Using PiP
python3 -m pip install atentry
```

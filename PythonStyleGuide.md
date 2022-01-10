## Naming Conventions
- Use lowercase and underscores (pothole case) to name variables, functions, and methods
- Use uppercase and underscores to name constants
- Use CamelCase for class names
- Use one-;etter variable names for math symbols and indices (do not use I, l, and O due to similar appearances to other characters)

## Function Length
- Maintain functions with bodies of around 25 lines 

## Test Code
- Code that will be tested or demonstrates the module's functions and classes must be placed in an `if __name__ == "__main__"` block

## Whitespace
- Use 4 spaces for indentation (Recall that Python is dependent on indentation)
- Do not double space code
- There should be at least one blank line between function definitions or class definitions
- Put one space between every binary operator and its operands
- Put a space between colon and type in function annotation (ex. `def fxn(in: int)`) and on either side of arrow if return type is specified (ex. ` def fxn() -> int:`)

Note: Avoid putting a space after a comma and before a parenthesis (ex. `foo = (0,)` is proper)

## Line Wrapping
- If a sequence of comma-seperated items is split across multiple lines, subsequent lines line up with the start of the sequence

## Comparisons
- Do not use redundant Boolean comparisons (ex. `if (a and b) == True:` is redundant)
- Use *is* to compare a value to None (ex. `if self is None:`)
- Move common code outside of if/else statements (don't repeat it under both)
- Only use parentheses with if/while statements to change order of evaluation

## Comments
- Comments begin with `#`
- Docstrings immediately follow the header

Docstrings:
- First line: What function does in terms of the parameters
- Write description as command rather than a statement
- Explain preconditions assumed to be true
- Include 2-3 shell examples
- Closing quotation marks should be on a seperate line from text

# Markdown Practice

## Headings and Text
A pound key (#) precedes a heading, with more pound keys indicating a smaller heading (up to 6 #s):

\# H1 ... \###### H6

**Appearance**: 

# H1

vs.

###### H6

Text is regularly typed.

A double carriage return will create a blank line between text.

## Lists
Lists can be created with either hyphens (-), plus signs (+), or numbers with periods (#.) acting as bullet points:

\- Item 1
\+ Item 2 

**Appearance**: 

- Item 1
+ Item 2
  - Indented, inner list created by preceding the hyphen with two spaces
- Back to this

1. This is a numbered list
        1. This is an inner list
2. Hey
3. Four

## Links and Pictures
Link words with the following formatting (replace *Linked words*):
\[Linked words\]\(URL\) 

Insert pictures (where the pictures are in the same directory as the .md file) with the following formatting (do not replace *alt text*):
!\[alt text\]\(URL\)

## Coding
To indicate an `in-line code`/highlight a word, surround the word with \`backticks\`.

To create a block of code, surround the code with three backticks on either side, and indicate the language beside the opening backticks:

\``` *language* 

*code block* 

\```

**Example**:

\```python

x = 3   

\```

**Appearance**: 

```python
x = 3
```

## Text Styling
To put a word in *italics*, surround it with \*single\* astericks.

To put a word in **bold**, surround it with \*\*double\*\* astericks.

To put a word in ***both*** **bold** and *italics*, surround it with \*\*\*three\*\*\* astericks.

To ~~strikethrough~~ a word, surround it with \~single\~ or  \~\~double\~\~ tilde.

To put text in block quote style, place a '>' in front:

\> blockquote

**Appearance**:

> blockquote

**NOTE**: You cannot underline in MD, since it is reserved for links.

## Creating Tables
Place all headers between straight lines, then seperate the content with an equivalent amount of columns, with at least three hyphens in each, then below create the respective content rows/columns (do not put an empty line between each; stack):

\| H1 \| H2 \| H3 \|

\| --- \| --- \| --- \|

\| C1 \| C2 \| C3 \|

\| C4 \| C5 \| C6 \|

**Appearance**: 

| H1 | H2 | H3 |
| --- | --- | --- |
| C1 | C2 | C3 |
| C4 | C5 | C6 |


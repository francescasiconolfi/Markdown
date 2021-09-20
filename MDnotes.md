# Markdown

## Headings and Text
A pound key (#) precedes a heading, with more pound keys indicating a smaller heading (up to 6 #s):

\# H1 ... \###### H6

**Appearance**: 

# H1

vs.

##### H5

Text is regularly typed.

A double carriage return will create a blank line between text.

---

### Ordered Lists 
Use numbers with periods (#.) (do not have to be numerically ascending or descending):

1. This is a numbered list
2. Hey
3. Four

Unordered:

\1. List

\8. Still

\4. Yup

**Appearance**:

1. List
8. Still
4. Yup

### Unordered Lists
Use hyphens (-), astericks (\*), or  plus signs (+) (if indent, inner lists are created): 

\- Item 1

\+ Item 2

\* Item 3 

**Appearance**: 

- Item 1

+ Item 2
  - Indented, inner list created by preceding the hyphen with two spaces
* Back to this

---

## Links and Pictures
Link words with the following formatting (replace *Linked words*):
\[Linked words\]\(URL\) 

Insert pictures (where the pictures are in the same directory as the .md file) with the following formatting (do not replace *alt text*):
!\[alt text\]\(URL\)

---

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
**NOTE**: Preceding text with a tab will also create a block of code, like so:

\<Tab> *code block*

**Appearance**:

        code block

**NOTE**: If placing within a list, indent twice instead of once

---

## Text Styling
To put a word in *italics*, surround it with \*single\* astericks.

To put a word in **bold**, surround it with \*\*double\*\* astericks.

To put a word in ***both*** **bold** and *italics*, surround it with \*\*\*three\*\*\* astericks.

To ~strikethrough~ a word, surround it with \~single\~ or  \~\~double\~\~ tilde.

To put text in block quote style, place a '>' in front:

\> blockquote

**Appearance**:

> blockquote

To create multiple lines within a blockquote, ensure every line has a '>' as the first character:

\> blockquote

\>

\> still a blockquote

**Appearance**:

> blockquote
>
> still a blockquote

Blockquotes within blockquotes:

> just one
>> inside once
>>> inside again

**NOTE**: You cannot underline in MD, since it is reserved for links.

---

## Creating Tables
Place all headers between straight lines, then seperate the content with an equivalent amount of columns, with at least three hyphens in each, then below create the respective content rows/columns:

\| H1 \| H2 \| H3 \|\
\| --- \| --- \| --- \|\
\| C1 \| C2 \| C3 \|\
\| C4 \| C5 \| C6 \|

**Appearance**: 

| H1 | H2 | H3 |
| --- | --- | --- |
| C1 | C2 | C3 |
| C4 | C5 | C6 |

---

## Horizontal Rules (Lines)
Use <= 3 astericks, dashes, or underscores on a line by themselves:

\*\*\*

\-\-\-

\_\_\_

**Appearance**:

*** 

**NOTE**: prefer dashes since the other two sometimes cause bold and italics to be activated

---

## Ending a Line
To end a line without double carriage return afterwards, put \ at end of line.

**Appearance:**

Example line\
Now, this text is on the next line

## Superscripts and Subscripts

Surround a superscript with "sup" like so: \<sup> superscript \</sup>

Surround a subscript with "sub" like so: \<sub> subscript \</sub>

## Aligning Text

Surround text with div tags.

To center: \<div align="center">text\</div>

To right justify: \<div align="right">text\</div>

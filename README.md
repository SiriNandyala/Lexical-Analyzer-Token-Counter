# Lexical Analyzer & Token Counter

## 1. Objective

Develop a C program that reads a source-code file and performs
lexical analysis by identifying and counting different types of tokens.

## 2. Problem Statement

The program identifies the following token types:

- Keywords
- Identifiers
- Operators
- Constants/Literals
- Separators/Delimiters
- Special Symbols
- Comments

## 3. Algorithm

1. Start the program.
2. Open the source-code file.
3. Read the file character by character.
4. Identify keywords and identifiers.
5. Identify operators.
6. Identify constants and string literals.
7. Identify separators and special symbols.
8. Identify comments.
9. Count each type of token.
10. Display the token type and token count.
11. Close the file.
12. Stop.

## 4. Source Code

The complete C source code is available in `lexical_analyzer.c`.

## 5. Sample Input

```c
int i = 1;
while (i <= 5) {
    printf("%d", i);
    i++;
}
```

## 6. Sample Output
```
TOKEN TYPE
------------------------------------------------
int Keyword
i Identifier
= Operator
1 Constant
; Separator
while Keyword
( Separator
i Identifier
<= Operator
5 Constant
) Separator
{ Separator
printf Identifier
( Separator
"%d" String Literal
, Separator
i Identifier
) Separator
; Separator
i Identifier
++ Operator
; Separator
} Separator
------------------------------------------------
```
## 7. Token Classification

| Token  | Type           |
| ------ | -------------- |
| int    | Keyword        |
| i      | Identifier     |
| =      | Operator       |
| 1      | Constant       |
| ;      | Separator      |
| while  | Keyword        |
| <=     | Operator       |
| 5      | Constant       |
| {      | Separator      |
| printf | Identifier     |
| "%d"   | String Literal |
| ,      | Separator      |
| ++     | Operator       |
| }      | Separator      |

## 8. Test Cases

Test Case 1

Input:

int i = 1;

Expected tokens:

int → Keyword
i → Identifier
= → Operator
1 → Constant
; → Separator
Test Case 2

Input:

while (i <= 5)

Expected tokens:

while → Keyword
( → Separator
i → Identifier
<= → Operator
5 → Constant
) → Separator

## 9. Conclusion

The lexical analyzer successfully identifies and classifies
different types of tokens from a source-code file and counts
the occurrences of each token type.


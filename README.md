# Little-Quilt
Quilt programming is used to implement quilt operations. I had implemented two Quilt operation ‘SEW’ and ‘TURN’, where ‘SEW’ operation has two parameters and ‘TURN’ has one parameter. We used two type of pattern ‘A’ and ‘B’, initially pattern name for ‘A’ and ‘B’ is ‘A0’ and ‘B0’ respectively. ‘SEW’ operation is used to sew two block of quilt of same height where ‘TURN’ operation turn the quilt block 90 degree clockwise which generates a new pattern. Using pattern ‘A’ and ‘B’ we can generate four patterns from each. Using these pattern we can design quilt. There are four levels of quilt implementation:
• In Level 0, We generated ‘TURN’ and ‘SEW’ operation.
• In Level 1, We extend Level 0 to head/tail operations for row and columns.
• In level 2, We extend Level 1 to let bindings for deﬁning ‘VAL’ and ‘FUN’.
• In Level 3, We extend Level 2 to If-then-else to support Recursion.

Problem Deﬁnition
Implementation of “Little Quilt” operations ‘SEW’ and ‘TURN’, where The language is deﬁned by the following BNF [3] (Backus-Naur-Form) grammar: QUILT ::= A|B|TURN(QUILT(A))|SEW(QUILT(A),QUILT(B))

Trouble in running lex and yacc ?

1) flex calc.l (this creates lex.yy.c file)

2) yacc -b parse -dv calc.y (this creates parse.output  parse.tab.c  parse.tab.h)

3) g++ lex.yy.c parse.tab.c -ll -ly (creates a.out file)

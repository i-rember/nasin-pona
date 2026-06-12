# nasin pona
sina wile e lipu pi toki pona la o luka e [ni](https://github.com/i-rember/nasin-pona/blob/main/README.md).

nasin pona is a programming language based on toki pona. Its goal is to make code simple and expressive using toki pona syntax.

## Variables
Variables are created with this syntax:
```
nanpa N li tu wan -- you can also use numerals explicitly
nimi S li "toki"
lon B li lon
```

Variables can be reassigned like so:
```
N li luka
S li "pona"
B li ala
```

## I/O
The program can print to the console like so:
```
o toki e "toki a, ma o!"
```

You can also output variables.
```
o toki e N -- "luka"; if the variable was assigned with an explicit numeral, a numeral is printed
o toki e S -- "pona"
o toki e B -- "ala"
```

You can print multiple values like so:
```
o toki e ni: "sina li jo e mani" N
```

The program can ask for input like so:
```
S li kama jo: "nimi sina li seme? "
N li kama jo: "sina jo e tenpo sike seme? "
B li kama jo: "sina pona ala pona? "
```

## Mathematics
Arithmetic can be done with their respective symbols, or these words:
```
nanpa a li luka
nanpa b li tu wan

nanpa sum li a wan b -- 8
nanpa sum li a weka b -- 2
nanpa sum li a mute b -- 15
nanpa sum li a tu b -- 1.666...
```

Comparisons are similar.
```
a sama b -- a == b
a lili tawa b -- a < b
a suli tawa b -- a > b
a ante b -- a != b
a sama anu lili tawa b -- a <= b
a sama anu suli tawa b -- a >= b
```

## "la"
The word "la" is used for conditionals and loops.

This is equivalent to "if":
```
a sama b la
  o toki e "sama"
pini
```

This is equivalent to "if-else":
```
a sama b la
  o toki e "sama"
ante la
  o toki e "ante"
pini
```

This is equivalent to "while":
```
tenpo b suli tawa a la
  o toki e b
  b li b wan wan
pini
```

This is equivalent to "for":
```
tenpo la
  nanpa i li ala
  li lili tawa luka luka
  li kama i wan wan
la
  o toki e i
pini
```

## Functions
Functions are created like this:
```
nasin add(nanpa a, nanpa b)
  o pana e ni: a wan b
pini
```

You can also define them inline:
```
nasin add li nasin(nanpa a, nanpa b)
  o pana e ni: a wan b
pini
```

or as a lambda:
```
nasin add li nasin(nanpa a, nanpa b): a wan b
```

## Additional features
You can also use sitelen pona! This is optional when writing an interpreter/compiler.
(this may not appear correctly)
```
󱤽󱦐󱤌󱦑󱤧󱤂
󱥫󱥍󱦐󱤌󱦑󱤨󱥩󱤭󱤭󱤡
    󱥄󱥬󱤉󱦐󱤌󱦑
    󱦐󱤌󱦑󱤧󱦐󱤌󱦑󱥳󱥳
󱥐
```

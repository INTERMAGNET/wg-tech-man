# RST Header Levels

In RST, a header is made by underlining the title text with a repeated character.
The level is determined by the order of first appearance.
We use in the technical manual the following rules:

## Level 1 — `---`

```rst
Section Title
-------------
```

## Level 2 — `` ``` ``

~~~rst
  Subsection Title
  ````````````````
~~~

## Level 3 — `"""`

```rst
Sub-subsection Title
""""""""""""""""""""
```

## Level 4 — `###`

```rst
Paragraph Title
###############
```

**Rules:**
- The underline must be **at least as long** as the title text.
- RST has no fixed mapping — the first character used becomes level 1, the second becomes level 2, etc.
- The order `---`, `` ``` ``, `"""`, `###` is a convention, not enforced by RST itself.

# YAML (Yaml ain't markup language)

### **Author** : _Vipul Vaishnav_

![YAML](https://github.com/vipul-vaishnav/Devops/YAML/Screenshots/Yaml.png)

This is a repo for Yaml Practice code
There is also a little comparison all different
markup languages like XML, JSON and YAML

> 1. YAML Structure,
> 2. DataTypes,
> 3. Advanced Data types,
> 4. Comparison with otherLanguages,

## Overview of YAML

1. All members of a list are lines beginning at the same indentation level starting with a "- " (a dash and a space):

```sh
---
# A list of tasty fruits
- Apple
- Orange
- Strawberry
- Mango
```

2. A dictionary is represented in a simple key: value form (the colon must be followed by a space):

```sh
# An employee record
martin:
  name: Martin Dillinger
  job: Developer
  skill: Elite
```

3. More complicated data structures are possible, such as lists of dictionaries, dictionaries whose values are lists or a mix of both:

```sh
# Employee records
- martin:
    name: Martin Dillinger
    job: Developer
    skills:
      - python
      - perl
      - pascal
- tabitha:
    name: Tabitha Bitumen
    job: Developer
    skills:
      - lisp
      - fortran
      - erlang
```

4. Dictionaries and lists can also be represented in an abbreviated form if you really want to:

```sh
---
martin: {name: Martin D'vloper, job: Developer, skill: Elite}
fruits: ['Apple', 'Orange', 'Strawberry', 'Mango']
```

5. Values can span multiple lines using | or >. Spanning multiple lines using a “Literal Block Scalar” | will include the newlines and any trailing spaces. Using a “Folded Block Scalar” > will fold newlines to spaces; it’s used to make what would otherwise be a very long line easier to read and edit. In either case the indentation will be ignored. Examples are:

```sh
include_newlines: |
            exactly as you see
            will appear these three
            lines of poetry

fold_newlines: >
            this is really a
            single line of text
            despite appearances
```

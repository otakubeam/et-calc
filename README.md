# Basic Arithmetic Interpreter in Etude

## Run

```
etc 2> /dev/null | qbe | as -o out && gcc out

./a.out "1 + 3"

# For example:
# > ./a.out "-3 + -5 - 3 + 3 - 3 + 55"

# Input string: -3 + -5 - 3 + 3 - 3 + 55
# -3 + -5 - 3 + 3 - 3 + 55
# 3 + -5 - 3 + 3 - 3 + 55
#  + -5 - 3 + 3 - 3 + 55
#  -5 - 3 + 3 - 3 + 55
# 5 - 3 + 3 - 3 + 55
#  - 3 + 3 - 3 + 55
#  3 + 3 - 3 + 55
#  + 3 - 3 + 55
#  3 - 3 + 55
#  - 3 + 55
#  3 + 55
#  + 55
#  55
#
# 44
```

## How to install etc on your system?

Etc stands for Etude compiler.  
Build it from sources following the instructions from
[Etude project](https://sr.ht/~orazov_ae/Etude/)

Otherwise you can inspect the compiled program from
the attached `a.out` file.

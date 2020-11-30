# grand_exchange
Generate files using variable lists -- originally desiged for PBS Pro QSUBs

```
python grand_exchange.py -h

usage: grand_exchange.py [-h] -r RUBRIC [-d DICT] [-f FILE]

Read a rubric file and generate individual files                     
based upon a custom set of variables.                     

Usage: python grand_exchange.py -r rubric_file -d variable,list 

optional arguments:
  -h, --help            show this help message and exit
  -d DICT, --dict DICT  variable to be changed and the values to be
                        substituted. (-d NUMBER,[1:20] --> replaces NUMBER
                        with the range of 1-20) (-d CHARACTER,[A,B,C] -->
                        replaces CHARACTER with each value) (-d
                        NUMBER,[1:20]/CHARACTER,[A,B,C]) --> will create all
                        permutations
  -f FILE, --file FILE  file of key-value pairs to change useful when all
                        permutations are not necessary. File format:
                        VARIABLE_A,VALUE_A/VARIABLE_B,VALUE_B

required arguments:
  -r RUBRIC, --rubric RUBRIC
                        input rubric file. Contains variables in <> such as
                        <NUM>
```

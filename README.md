# Banknotes-ATM-Machine-Output-Note
In this problem you have to read an integer value and calculate the smallest possible number of banknotes in which the value may be decomposed. The possible banknotes are 100, 50, 20, 10, 5, 2 e 1. Print the read value and the list of banknotes.
beecrowd | 1018
Banknotes
Adapted by Neilor Tonin, URI  Brazil

Timelimit: 1
In this problem you have to read an integer value and calculate the smallest possible number of banknotes in which the value may be decomposed. The possible banknotes are 100, 50, 20, 10, 5, 2 e 1. Print the read value and the list of banknotes.

Input
The input file contains an integer value N (0 < N < 1000000).

Output
Print the read number and the minimum quantity of each necessary banknotes in Portuguese language, as the given example. Do not forget to print the end of line after each line, otherwise you will receive “Presentation Error”.

Input Sample	Output Sample
576

576
5 nota(s) de R$ 100,00
1 nota(s) de R$ 50,00
1 nota(s) de R$ 20,00
0 nota(s) de R$ 10,00
1 nota(s) de R$ 5,00
0 nota(s) de R$ 2,00
1 nota(s) de R$ 1,00

11257

11257
112 nota(s) de R$ 100,00
1 nota(s) de R$ 50,00
0 nota(s) de R$ 20,00
0 nota(s) de R$ 10,00
1 nota(s) de R$ 5,00
1 nota(s) de R$ 2,00
0 nota(s) de R$ 1,00

503

503
5 nota(s) de R$ 100,00
0 nota(s) de R$ 50,00
0 nota(s) de R$ 20,00
0 nota(s) de R$ 10,00
0 nota(s) de R$ 5,00
1 nota(s) de R$ 2,00
1 nota(s) de R$ 1,00

```base
s = int(input())
h = s//100
f = (s % 100)//50
t = ((s % 100) % 50)//20
d = (((s % 100) % 50) % 20)//10
p = ((((s % 100) % 50) % 20) % 10)//5
dui = (((((s % 100) % 50) % 20) % 10) % 5)//2
a = (((((s % 100) % 50) % 20) % 10) % 5) % 2
print(s)
print(f'{h} nota(s) de R$ 100,00')
print(f'{f} nota(s) de R$ 50,00')
print(f'{t} nota(s) de R$ 20,00')
print(f'{d} nota(s) de R$ 10,00')
print(f'{p} nota(s) de R$ 5,00')
print(f'{dui} nota(s) de R$ 2,00')
print(f'{a} nota(s) de R$ 1,00')
```

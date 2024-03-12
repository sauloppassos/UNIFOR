# UNIFOR
**Disciplina: raciocínio logico algorítmico**
**Orientador:** Prof. Ricardo Carubbi
## Lista de exercícios 
### Exercício 03
Represente em Fluxograma ou Pseudocódigo, um algoritmo para determinar se um numero inteiro e positivo é par ou impar.
#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite um número}}
B --> C[/numero/]
C --> D{numero > 0}	
D --NÃO--> E{{O numero informado é negativo!}}
E --> Z([FIM])
D --SIM--> F[resto é = numero % 2]
F --> G{resto == 0}
G --NÃO--> H{{O numero é impar!}}
G --SIM--> I{{O numero é par!}}
H --> Z
I --> Z
```
#### Pseudocodigo
```
1 ALGORITMO verifica_par_impar
2 DECLARE numero, resto NUMERICO
3 ESCREVA "Digite um numero"
4 LEIA numero
5 SE numero > 0 ENTAO 
6    resto = numero % 2
7    SE resto == 0 ENTAO 
8        ESCREVA "O numero e par!"
9    SENAO 
10        ESCREVA "O numero é impar!"
11  SE NAO 
12      ESCREVA "O numero deve ser positivo!"
13 FIM_ALGORITMO
```






# TESTE DE MESA 
#### Teste
#### EXERCICIO 01
| numero | numero > 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | -- | 
| -1 | F |   |   | "O número deve ser postivo!" |
| 2 | V | 0 | V | "O número é par!" |
| 3 | V | 1 | F | "O número é impar!" |
| 8 | V | 0 | V | "O número é par!" |
| 9 | V | 1 | F | "O número é ímpar!" |

#### EXERCICIO 02 
| número  |  número = n*3 | 


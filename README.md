# MAC0323 - Algoritmos e Estruturas de Dados II (2022)

## Dados EP2 - Tabela de símbolos

## Regras utilizadas para a normalização das palavras.

1. Caracter simples serão considerados como palavras, quando sozinhos: a => a, a++ => a++
2. Maiúsculo => Minúsculo
3. Removida a pontuação no final das palavras: magnet, => magnet
4. O que esta sendo considerado como pontuação no final das palavras são:
    1. , vígual (ch == 44)
    2. . ponto final (ch == 46)
    3. ? interrogação (ch == 63)
    4. ! exclamação (ch == 33)
    5. : dois pontos (ch == 58)
    6. ; ponto e vírgula (ch == 59)
5. A lista caracters abaixo não são considerados na palavra
    1. " Aspas duplas (ch=34)
    2. ' Aspas simples(ch=39)
    3. .( Abre parênteses (ch=40)
    4. ) Fecha parênteses (ch=41)
    5. .[ Abre colchetes (ch=91)
    6. ] Fecha colchetes (ch=93)
    7. _ Underline (ch=95)
    8. ` Aspas invertida (ch=96)
    9. { Abre chave (ch=123)
    10. } Fecha chave (ch=125)
    11. ” Caracters como Aspas duplas de citação (ch>=0)
6. Preservados os pontos internos das palavras: www.gutenberg.org => www.gutenberg.org. O problema de separar palavras
   que possuem ponto interno é que siglas como U.S, se tornan US. Desse modo, encontra-se US que não existe no
   texto original. Tanto as palavras inseridas na estrutura, quanto as palavras das operações são normalizadas com as
   regras acima.

## Arquivos para testes

### 1. Livro: Frankenstein, by Mary Wollstonecraft (Godwin) Shelley

1. [Origital](Frankenstein.txt) - 438K
2. [Teste](FrankensteinTest.txt) - 438K
3. [Palavras](FrankensteinWords.txt) - 1.1M

| Total de Palavras | Operações |
|:------------------|----------:|
| 78.121            |         4 |

## Resultados

| Operação |    VO | Tempo |
|:---------|------:|------:|
| 1 78121  |       | 0.0   |
| 2 the    |  4377 | 0.0   |
| 3 email  | 2232  | 0.0   |
| 4 5000   |plainly| 0.0   |

### 2. Arquivo de IP's EDI

1. [Origital](https://vpublic-files.s3.amazonaws.com/IPs.txt.zip) - 70M
2. [Teste](https://vpublic-files.s3.amazonaws.com/IPSTest.txt.zip) - 70M
3. [Palavras](https://vpublic-files.s3.amazonaws.com/IPSWords.txt.zip) - 144M

| Total de Palavras | Operações |
|:------------------|----------:|
| 7.558.560         |         8 |

## Resultados

| Operação          |       VO | Tempo |
|:------------------|---------:|------:|
| 1 560             |          |   0.0 |        
| 4 0               |        - | 0.0   |          
| 3 193.201.224.225 |       12 | 0.0   |
| 2 -               |      224 | 0.0   |   
| 1 7558000         |          |   23s |
| 4 0               |        - | 0.0   |
| 3 193.201.224.225 |    65376 | 0.0   |
| 2 -               | 3023424  | 0.0   |

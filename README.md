# t2-sisop
# MemSim — Grupo 06
## Simulador de Gerência de Memória (Paginação)

**Disciplina:** Sistemas Operacionais – 2026/I  
**Professor:** Filipo Mór  
**Grupo:** 06  
**Alunos:** Luana Thurow e Sergio Duarte  
**Algoritmos:** FIFO vs. Segunda Chance (Clock)  
**Frames:** 4  

---

## Como executar

```bash
Seleção do algoritmo

O algoritmo utilizado é definido diretamente no código, nas linhas 148 e 149:

# tabela_paginas = TabelaPaginas(num_frames, "FIFO")
tabela_paginas = TabelaPaginas(num_frames, "CLOCK")

Para utilizar o algoritmo FIFO, deixe:

tabela_paginas = TabelaPaginas(num_frames, "FIFO")
# tabela_paginas = TabelaPaginas(num_frames, "CLOCK")

Para utilizar o algoritmo Segunda Chance (Clock), deixe:

# tabela_paginas = TabelaPaginas(num_frames, "FIFO")
tabela_paginas = TabelaPaginas(num_frames, "CLOCK")

python simulador_memoria.py entrada.txt 

```

A primeira linha do `entrada.txt` define o número de frames.  
As linhas seguintes são os números de páginas acessadas, uma por linha.

## Exemplo de entrada

```
4
7
0
1
2
0
3
0
4
2
3
0
3
```

## Funcionalidades implementadas
- Processamento da sequência de páginas;
- Detecção de Hits e Page Faults;
- Alocação em frames vazios;
- Substituição de páginas utilizando FIFO;
- Substituição de páginas utilizando Segunda Chance (Clock);
- Controle do bit de referência;
- Ponteiro circular do algoritmo Clock;
- Exibição do mapa da memória a cada passo;
- Indicação do frame alterado;
- Estatísticas finais da execução:
  - Total de acessos;
  - Total de Page Faults;
  - Taxa percentual de falhas.

## Requisitos

- Python 3.10 ou superior
- Nenhuma dependência externa


## Referência

Silberschatz, Abraham; Galvin, Peter B.; Gagne, Greg.
Operating System Concepts, 9ª edição.

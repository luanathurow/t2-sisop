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
python simulador_memoria.py entrada.txt fifo
python simulador_memoria.py entrada.txt clock
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
```

## Requisitos

- Python 3.10 ou superior
- Nenhuma dependência externa
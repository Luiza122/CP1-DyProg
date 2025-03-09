# Checkpoint 1 – Dynamic Programming

# Visão Geral
Este projeto explora o uso de Programação Dinâmica para implementar algoritmos de ordenação. O objetivo principal é aplicar diferentes abordagens de ordenação e comparar seus desempenhos em cenários distintos. Os principais desafios abordados no projeto incluem:

- Ordenação de pontos com base na distância de Manhattan.
- Ordenação de palavras segundo uma ordem personalizada.
- Comparação de desempenho entre os algoritmos Merge Sort e Quick Sort.

Os códigos foram desenvolvidos em Python 3.x e executados no Jupyter Notebook para facilitar a visualização e análise.

---

# Estrutura do Projeto

 Arquivos principais:
- `ordenacao_manhattan.ipynb` → Algoritmo para ordenar pontos com base na distância de Manhattan.
- `ordenacao_palavras.ipynb` → Ordenação de palavras conforme uma ordem definida.
- `comparacao_merge_quick.ipynb` → Comparação de desempenho entre os algoritmos Merge Sort e Quick Sort.
- `README.md` → Documentação detalhada do projeto.

---

## Tecnologias Utilizadas
- Python 3.x
- **Jupyter Notebook
- Bibliotecas: 
  - `time` → Medição do tempo de execução.
  - `sys` → Medição de uso de memória.

---

# Como Executar o Projeto

# Passo 1: Instalar Dependências

No terminal, execute o seguinte comando para instalar o Jupyter Notebook:

```bash
pip install jupyter notebook
```

# Passo 2: Executar o Jupyter Notebook

Após a instalação, inicie o Jupyter Notebook:

```bash
jupyter notebook
```

Isso abrirá o Jupyter no navegador. Localize o arquivo desejado (`.ipynb`) e execute-o para visualizar os resultados.

---

# Detalhamento das Soluções

# 1. Ordenação de Pontos pela Distância de Manhattan

O algoritmo implementado utiliza o método Merge Sort para ordenar uma lista de pontos (x, y) de acordo com a distância de Manhattan. A distância de Manhattan é definida como a soma dos valores absolutos das coordenadas.

# Cálculo da Distância de Manhattan:
```python
def distancia_manhattan(x, y):
    return abs(x) + abs(y)
```

- Destaques:
  - Utilização de **list comprehension** para reestruturar e manipular os dados.
  - Os pontos e suas distâncias são armazenados de forma eficiente em um **dicionário**.

---

### 2. Ordenação de Palavras com Ordem Personalizada

Nesta tarefa, foi implementado um algoritmo de ordenação utilizando **Merge Sort** para classificar palavras de acordo com uma ordem definida. Para isso, usamos um **dicionário de prioridade** que mapeia cada caractere para um valor de prioridade.

# Exemplo de Dicionário de Prioridade:
```python
prioridade = {'a': 1, 'b': 2, 'c': 3, ...}
```

- Destaques:
  - O uso de **list comprehension** para otimizar a entrada de dados.
  - A ordenação é feita considerando a prioridade de cada caractere de acordo com o dicionário.

---

# 3. Medição de Desempenho: Merge Sort vs Quick Sort

As tarefas 2.1 e 2.2 visam comparar os algoritmos **Merge Sort** e **Quick Sort**, tanto em termos de tempo de execução quanto de uso de memória.

# Medição de Tempo:
Utilizamos o módulo `time` para medir o tempo de execução dos algoritmos:

```python
import time
start = time.time()
merge_sort(lista)
end = time.time()
print(f"Tempo: {end - start}s")
```

#### Medição de Memória:
Através do módulo `sys`, foi possível medir o uso de memória dos algoritmos:

```python
import sys
print(f"Uso de memória: {sys.getsizeof(lista)} bytes")
```

---

# Considerações Finais

Este projeto aplica conceitos avançados de programação, com ênfase em **Programação Dinâmica**, para resolver problemas de ordenação e análise de desempenho. As implementações foram cuidadosamente organizadas para facilitar a compreensão dos algoritmos e seus impactos no desempenho.

As soluções implementadas e testadas são ideais para quem deseja explorar o comportamento de algoritmos de ordenação em diferentes cenários e analisar seu desempenho de forma eficaz.



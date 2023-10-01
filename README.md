# HeuroGraph Library

![GitHub stars](https://img.shields.io/github/stars/alexgiving/HeuroGraph-Library?style=social)
![GitHub forks](https://img.shields.io/github/forks/alexgiving/HeuroGraph-Library?style=social)
![GitHub issues](https://img.shields.io/github/issues/alexgiving/HeuroGraph-Library)
![GitHub contributors](https://img.shields.io/github/contributors/alexgiving/HeuroGraph-Library)

Welcome to the HeuroGraph-Library! This is a Python library designed for solving graph-related problems using heuristic algorithms. Whether you're working on graph coloring, maximum clique, or other graph optimization problems, this library provides a set of powerful heuristic algorithms to assist you in finding efficient solutions.

## Features

- **Graph Coloring**: Solve graph coloring problems using various heuristic techniques.
- **Maximum Clique**: Find maximum cliques in graphs through heuristic methods.
- **Scalability**: Designed for handling large-scale graphs efficiently.
- **Easy Integration**: Simple and straightforward integration into your Python projects.

## Getting Started

1. Clone this repository:

   ```shell
   git clone https://github.com/alexgiving/HeuroGraph-Library.git
   ```

2. Install dependencies

    ```shell
    pip install -r requirements.txt
    ```

3. Set environment

    ```bash
    export PYTHONPATH=${PYTHONPATH}:$(pwd)
    ```

## Greedy Heuristic Vertex Coloring Solver

Simple usage
<<<<<<< HEAD
=======

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```python
from pathlib import Path

from graph_lib import Graph
from graph_lib.coloring import color_graph_greedy_sorted_shuffled

graph_DIMACS_path = Path('myciel3.col')
graph = Graph(graph_DIMACS_path)

coloring_result = color_graph_greedy_sorted_shuffled(graph)

coloring_result.num_colors
>> 4
```

<<<<<<< HEAD
### Benchmarking
=======
### Benchmarking Coloring

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
Get benchmark data

```bash
bash scripts/download_coloring.sh
```

Run evaluation script

```bash
python benchmark_coloring.py
```

Result table
<<<<<<< HEAD
=======

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```text
       Instance  Time, s  Colors
    myciel3.col     0.00       4
    myciel7.col     0.01       8
    school1.col     0.05      31
school1_nsh.col     0.04      30
       anna.col     0.00      11
  miles1000.col     0.01      43
  miles1500.col     0.01      73
   le450_5a.col     0.04      11
  le450_15b.col     0.04      17
 queen11_11.col     0.00      15
```

## Greedy Randomized Clique Solver

Simple usage
<<<<<<< HEAD
=======

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```python
from pathlib import Path

from graph_lib import Graph
from graph_lib.clique import greedy_randomized_clique

graph_DIMACS_path = Path('graph.clq')
graph = Graph(graph_DIMACS_path)

coloring_result = color_graph_greedy_sorted_shuffled(graph)

coloring_result.num_colors
>> [1, 2, 3, 4]
```

<<<<<<< HEAD
### Benchmarking
Get benchmark data
=======
### Benchmarking Clique

Get benchmark data

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```bash
bash scripts/download_clique.sh
```

Run evaluation script
<<<<<<< HEAD
=======

>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```bash
python benchmark_clique.py
```

Result table
<<<<<<< HEAD
```text
          Instance  Time, s  Clique size
        C125.9.clq     0.00           26
    brock200_3.clq     0.00           10
    brock400_4.clq     0.00           16
  johnson8-2-4.clq     0.00            4
    p_hat300-3.clq     0.00           15
      MANN_a27.clq     0.00           39
    brock200_4.clq     0.00           12
gen200_p0.9_44.clq     0.00           27
       keller4.clq     0.00            9
    p_hat500-3.clq     0.00           28
       MANN_a9.clq     0.00           12
    brock400_1.clq     0.00           15
gen200_p0.9_55.clq     0.00           29
   p_hat1000-1.clq     0.00            5
       san1000.clq     0.01            7
    brock200_1.clq     0.00           14
    brock400_2.clq     0.00           16
    hamming8-4.clq     0.00           16
   p_hat1000-2.clq     0.01           21
   sanr200_0.9.clq     0.00           27
    brock200_2.clq     0.00            7
    brock400_3.clq     0.00           16
 johnson16-2-4.clq     0.00            8
   p_hat1500-1.clq     0.01            6
   sanr400_0.7.clq     0.00           13
=======

```text
          Instance  Time, s  Clique size
    brock200_1.clq     0.73           21
    brock200_2.clq     0.24           12
    brock200_3.clq     0.39           15
    brock200_4.clq     0.49           17
    brock400_1.clq     3.30           23
    brock400_2.clq     3.04           22
    brock400_3.clq     3.02           22
    brock400_4.clq     3.00           23
        C125.9.clq     0.77           34
gen200_p0.9_44.clq     1.95           38
gen200_p0.9_55.clq     1.99           52
    hamming8-4.clq     0.65           16
 johnson16-2-4.clq     0.25            8
  johnson8-2-4.clq     0.01            4
       keller4.clq     0.33           11
      MANN_a27.clq    43.12          125
       MANN_a9.clq     0.11           16
   p_hat1000-1.clq     1.33           10
   p_hat1000-2.clq     8.36           38
   p_hat1500-1.clq     3.60           11
    p_hat300-3.clq     1.88           32
    p_hat500-3.clq     5.67           43
       san1000.clq     7.81           10
   sanr200_0.9.clq     1.89           40
   sanr400_0.7.clq     2.27           20
>>>>>>> ac0aa742a770d26c25d89f20c6a08ecc87ab69f9
```

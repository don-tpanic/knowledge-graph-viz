# knowledge-graph-viz

* Place a paper's knowledge graph as `papers/<doi>_original.json` (for original KG) and `papers/<doi>_perm_<index>.json` (for permuted KG).

* Visualize the original knowledge graph of a paper: `python viz_graph.py -p <doi> -o`
e.g.,
  ```
  python viz_graph.py -p 10.1016:j.cognition.2020.104244 -o
  ```

* Visualize an altered knowledge graph of a paper: `python viz_graph.py -p <doi> -pe -pi <index-of-the-permutation>`
e.g., 
  ```
  python viz_graph.py -p 10.1016:j.cognition.2020.104244 -pe -pi 1
  ```

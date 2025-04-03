# knowledge-graph-viz

* Work with the repo locally:
  ```
  git clone git@github.com:don-tpanic/knowledge-graph-viz.git
  ```

* Install dependencies:
  ```
  pip install -r requirements.txt
  ```

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

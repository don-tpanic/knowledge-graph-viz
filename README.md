# knowledge-graph-viz

* Work with the repo locally:
  ```
  git clone git@github.com:don-tpanic/knowledge-graph-viz.git
  ```

* Install dependencies:
  ```
  pip install -r requirements.txt
  ```

* Place a paper's knowledge graph as `papers/<doi>/label_<uid>_kg_original.json` (for original KG) and `papers/<doi>/label_<uid>_kg_perm_<index>.json` (for permuted KG). You should use `<uid>` to identify your work because others might also work on this paper and create different KGs.

* Visualize the original knowledge graph of a paper: `python viz_graph.py -p <doi> -u <uid> -o`
e.g.,
  ```
  python viz_graph.py -p 10.1016:j.cognition.2020.104244 -u ken_c137 -o
  ```

* Visualize an altered knowledge graph of a paper: `python viz_graph.py -p <doi> -u <uid> -pe -pi <index-of-the-permutation>`
e.g., 
  ```
  python viz_graph.py -p 10.1016:j.cognition.2020.104244 -u ken_c137 -pe -pi 1
  ```

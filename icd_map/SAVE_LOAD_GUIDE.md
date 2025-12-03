# ICD Graph Save/Load Example

## Saving the Graph

```python
# After building your graph from CSV
csv_graph.save_to_file('icd_graph.pkl')
```

## Loading the Graph

```python
# Load the graph without rebuilding from CSV
loaded_graph = Graph.load_from_file('icd_graph.pkl')

# Use the loaded graph
print(f"Loaded graph has {len(loaded_graph.adjacency_list)} nodes")

# Query children
children = loaded_graph.get_neighbors("A00")
for child in children:
    desc = loaded_graph.get_node_data(child).get('description', '')
    print(f"{child}: {desc}")
```

## Benefits

- **Fast**: Loading from pickle is much faster than re-parsing the CSV
- **Complete**: Preserves all node data and relationships
- **Simple**: Just one line to save, one line to load

## File Created

The graph is saved to `icd_graph.pkl` in your project directory.

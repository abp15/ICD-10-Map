# ICD Graph Database Project

## Main Files (Keep These)

### Essential Files
- **`Neo4j_ICD_database.ipynb`** - Your primary working notebook with all functionality
- **`icd_codes.csv`** - Your ICD-10 code data (1.2 MB)
- **`icd_graph.pkl`** - Saved graph for fast loading (1.6 MB)

### Optional Files
- **`graph_visualization.png`** - Generated visualization (can be regenerated)
- **`SAVE_LOAD_GUIDE.md`** - Documentation for save/load feature

## Files You Can Delete

These were created for testing/development and are no longer needed:
- `notebook.py` - Old Python script (functionality now in .ipynb)
- `test_save_load.py` - Test script (functionality now in .ipynb)
- `reload_helper.py` - Helper script (no longer needed)
- `ICDGraphDatabase.ipynb` - Old notebook (if it exists)

## Quick Start

1. Open `Neo4j_ICD_database.ipynb` in Jupyter/VS Code
2. Run all cells to load your ICD graph
3. Use the saved `icd_graph.pkl` for fast loading in future sessions

## Features in Your Notebook

✅ Graph class with save/load functionality
✅ CSV import with parent-child relationships
✅ Neo4j integration (when you're ready)
✅ Visualization capabilities
✅ Query and navigation methods

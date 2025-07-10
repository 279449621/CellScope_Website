TreeStructured: ``ts``
======================

Generation and visualization of tree-structured representations of cell clustering using UMAP and various steps.

.. list-table::

   * - ``CellScope.ts.find_map``
     - Create a mapping matrix between two sets of cluster labels.

   * - ``CellScope.ts.generate_tree_structured``
     - Generate the tree-structured representation of data based on clustering labels.

   * - ``CellScope.ts.visualize_tree_structured``
     - Visualize the tree-structured UMAP embeddings for different levels of clustering.

   * - ``CellScope.ts.tree_structure_visualization_static``
     - Generate the static tree-structured visualization.

   * - ``CellScope.ts.tree_structure_visualization_dynamic``
     - Generate the dynamic tree-structured visualization.

   * - ``CellScope.ts.tree_structure_visualization_step``
     -  Generate the each step of tree-structured visualization.

.. toctree::
   :maxdepth: 2

   CellScope.ts.find_map
   CellScope.ts.generate_tree_structured
   CellScope.ts.visualize_tree_structured
   CellScope.ts.tree_structure_visualization_static
   CellScope.ts.tree_structure_visualization_dynamic
   CellScope.ts.tree_structure_visualization_step

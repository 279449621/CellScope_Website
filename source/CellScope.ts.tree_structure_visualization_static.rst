CellScope.ts.tree_structure_visualization_static
============================================================================

CellScope.ts. ``tree_structure_visualization_static`` (**T**, **step0**, **step1**, **Title_1**, **Title_all**, **Y_initial**,  
**Y_1**, **Y_all**, **index_1**, **index_all**, **save_figure** = False, **filename** = '')

The ``tree_structure_visualization_static``  function automatically generates hierarchical
 tree structured visualization (up to three levels) through a series of UMAP scatter 
 plots derived from the ``generate_tree_structured function``, 
 with an option to save the figures to a specified directory.

.. rubric:: Parameters

- **T** (:class:`np.ndarray`): 

   Matrix of clustering labels for different levels of clustering.

- **step0** (:class:`int`): 

   Final starting level for the tree-structured visualization.

- **step1** (:class:`int`): 

   Final ending level for the tree-structured visualization.

- **Title_1** (:class:`list`): 

   List of titles for the first-level clusters.

- **Title_all** (:class:`list`): 

   List of titles for clusters at all levels.
   
- **Y_initial** (:class:`np.ndarray`): 

   Initial 2D UMAP embedding of all cells.

- **Y_1** (:class:`list` of :class:`np.ndarray`): 

   List of UMAP embeddings for clusters at the first level.

- **Y_all** (:class:`list` of :class:`np.ndarray`): 

   List of UMAP embeddings for clusters at all levels.

- **index_1** (:class:`list`): 

   List of indices corresponding to cells in each cluster at the first level.

- **index_all** (:class:`list`): 

   List of indices corresponding to cells in each cluster at all levels.

- **save_figure** (:class:`bool`, optional, default=False): 

   If True, saves the figures to the specified path.

- **filename** (:class:`str`, optional, default=''): 

   Directory path to save the figures. Required if `save_figure=True`.

.. rubric:: Return

- This function does not return any values. It directly renders the tree structured visualization in CellScope.

CellScope.ts.tree_structure_visualization_dynamic
============================================================================

CellScope.ts. ``tree_structure_visualization_dynamic`` (**T**, **step0**, **step1**, **Title_1**, **Title_all**, **Y_initial**,  
**Y_1**, **Y_all**, **index_1**, **index_all**, **interval** = 800, **save_gif** = False, **gif_filename**="tree_animation.gif", **dpi**=100)

The ``tree_structure_visualization_dynamic``  function Dynamically constructs a three-tiered hierarchical visualization system with native support for GIF animation export.

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

- **interval** (:class:`int`,optional, default=800)

   Controls the time interval between animation frames (unit: milliseconds).

- **save_gif** (:class:`bool`, optional, default=False): 

   If True, saves the GIF to the specified path.

- **gif_filename** (:class:`str`, optional, default=''): 

   Directory path to save the GIF. Required if `save_gif=True`.

- **dpi** (:class:`int`,optional, default=100)

   Dots per inch (DPI) defines the pixel density, where dpi=100 corresponds to a resolution of 100 pixels along one linear inch.
   
.. rubric:: Return

- This function does not return any values. It directly renders the tree structured visualization in CellScope.

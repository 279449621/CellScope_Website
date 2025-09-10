CellScope.ts.tree_structure_visualization_step
=============================================

CellScope.ts. ``tree_structure_visualization_step`` (**T**, **step0**, **step1**, **Title_1**, **Title_all**, **Y_initial**,  
**Y_1**, **Y_all**, **index_1**, **index_all**, **main_radius**=2.0, **orbit_radius**=1.5, **orbit_distance**=4.0,  
**branch_params**=None, **save_fig**=False, **save_path**='')

The ``tree_structure_visualization_step`` function progressively constructs the main trunk and branch components of the tree-structured visualization, enabling users to freely assemble them.

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

- **main_radius** (:class:`float`, optional, default=2.0): 
   The node radius of the zeroth-layer nodes.

- **orbit_radius** (:class:`float`, optional, default=1.5): 
   The node radius of the first-layer nodes.

- **orbit_distance** (:class:`float`, optional, default=4.0): 
   The distance between the centers of the first-layer nodes and the zeroth-layer nodes.

- **branch_params** (:class:`None` or :class:`dict`, optional, default=None): 
   Additional parameters for branch customization.

- **save_fig** (:class:`bool`, optional, default=False): 
   If True, saves the figures to the specified path.

- **save_path** (:class:`str`, optional, default=''): 
   Directory path to save the figures. Required if `save_figure=True`.
   
.. rubric:: Returns

- Two dictionaries ``R_dict`` and ``C_dict``, containing node radii and center coordinates for plotting.
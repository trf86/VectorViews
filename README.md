# VectorViews
This header-only library provides support for various views of the std::vector class.  

The aim of this work is to provide various "viewers" for contiguous data stored in a vector.  These viewers are especially useful in scientific computing applications where contiguous data has performance advantages, but single-value indexing makes reading the code difficult.  This library provides various views including arrays (1D, 2D, 3D, n-D), jagged arrays (2D, 3D, etc.), and sparse matrices (CSR, BSR, etc.). 

These viewers will be just that: viewers.  They do not own the data and instead take shared pointers to ensure the data is not freed before the viewer.

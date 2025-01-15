# Implementation and Application of the Paper  
**Reference**: Ryu, S. (2018). *“Deeply learning molecular structure-property relationships using attention- and gate-augmented graph convolutional network”*. arXiv:1805.10988  

## Summary  
- Developed a graph convolutional network (GCN) combining molecular structure and atomic features to predict molecular properties.  
- Converted the original TensorFlow model into PyTorch.  

## Key Improvements  
1. **One-Hot Encoding Issue**:  
   - One-hot encoding makes the input matrix size data-dependent, requiring inefficient padding for varying matrix sizes.  
   - **Solution**: Numerical representation and normalization of feature values for efficient mapping.  

2. **Performance Enhancements**:  
   - Replacing one-hot encoded atomic features with atomic feature values and a combination of atomic & molecular feature values improved performance.  
   - **Results**:  
     - Reduced Mean Absolute Error (MAE).  
     - Increased R² value, indicating better predictive accuracy.  

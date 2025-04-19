# Clustering

# Clustering Algorithms Comparative Study

## Introduction
This project compares the performance of K-Means, Hierarchical, and Mean Shift clustering algorithms on the Iris dataset using different preprocessing techniques and evaluation metrics.

## Dataset
Used the Iris dataset from UCI repository with 150 samples and 4 features.

## Methodology
1. Applied 6 preprocessing techniques:
   - No processing
   - Normalization
   - Standardization
   - PCA
   - Standardization + Normalization
   - Standardization + Normalization + PCA
2. Applied 3 clustering algorithms:
   - K-Means
   - Hierarchical
   - Mean Shift
3. Evaluated with 3 metrics:
   - Silhouette Score
   - Calinski-Harabasz Score
   - Davies-Bouldin Score

## Performance Results

### Silhouette Scores (Higher is better)

#### Hierarchical Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.554      | 0.489      | 0.484      |
| Normalization       | 0.556      | 0.479      | 0.466      |
| PCA                 | 0.598      | 0.541      | 0.549      |
| T+N                 | 0.498      | 0.477      | 0.436      |
| T+N+PCA             | 0.647      | 0.615      | 0.558      |
| Transform           | 0.447      | 0.401      | 0.331      |

#### K-Means Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.553      | 0.497      | 0.494      |
| Normalization       | 0.576      | 0.537      | 0.502      |
| PCA                 | 0.598      | 0.561      | 0.535      |
| T+N                 | 0.555      | 0.495      | 0.404      |
| T+N+PCA             | 0.645      | 0.615      | 0.557      |
| Transform           | 0.457      | 0.386      | 0.361      |

#### Mean Shift Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.686      | N/A        | N/A        |
| Normalization       | 0.819      | N/A        | N/A        |
| PCA                 | 0.710      | N/A        | N/A        |
| T+N                 | 0.547      | N/A        | N/A        |
| T+N+PCA             | 0.649      | N/A        | N/A        |
| Transform           | 0.582      | N/A        | N/A        |

---

### Calinski-Harabasz Scores (Higher is better)

#### Hierarchical Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 558.06     | 515.08     | 488.48     |
| Normalization       | 1386.78    | 1063.77    | 917.20     |
| PCA                 | 688.62     | 673.95     | 665.88     |
| T+N                 | 242.27     | 245.72     | 218.64     |
| T+N+PCA             | 449.14     | 522.11     | 562.47     |
| Transform           | 222.72     | 201.25     | 192.68     |

#### K-Means Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 561.63     | 530.39     | 492.51     |
| Normalization       | 1447.00    | 1157.35    | 982.04     |
| PCA                 | 693.71     | 715.90     | 595.47     |
| T+N                 | 288.68     | 218.32     | 231.56     |
| T+N+PCA             | 468.13     | 522.11     | 589.53     |
| Transform           | 241.32     | 206.79     | 168.88     |

#### Mean Shift Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 509.70     | N/A        | N/A        |
| Normalization       | 1634.00    | N/A        | N/A        |
| PCA                 | 565.73     | N/A        | N/A        |
| T+N                 | 215.35     | N/A        | N/A        |
| T+N+PCA             | 481.72     | N/A        | N/A        |
| Transform           | 251.35     | N/A        | N/A        |

---

### Davies-Bouldin Scores (Lower is better)

#### Hierarchical Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.656      | 0.795      | 0.820      |
| Normalization       | 0.694      | 0.868      | 0.995      |
| PCA                 | 0.560      | 0.655      | 0.653      |
| T+N                 | 0.829      | 0.889      | 0.880      |
| T+N+PCA             | 0.464      | 0.521      | 0.541      |
| Transform           | 0.803      | 0.979      | 0.974      |

#### K-Means Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.662      | 0.771      | 0.813      |
| Normalization       | 0.644      | 0.806      | 0.858      |
| PCA                 | 0.565      | 0.620      | 0.577      |
| T+N                 | 0.736      | 1.148      | 0.908      |
| T+N+PCA             | 0.496      | 0.521      | 0.576      |
| Transform           | 0.832      | 0.877      | 1.180      |

#### Mean Shift Clustering
| Preprocessing       | 3 clusters | 4 clusters | 5 clusters |
|---------------------|------------|------------|------------|
| No Processing       | 0.389      | N/A        | N/A        |
| Normalization       | 0.241      | N/A        | N/A        |
| PCA                 | 0.355      | N/A        | N/A        |
| T+N                 | 0.689      | N/A        | N/A        |
| T+N+PCA             | 0.516      | N/A        | N/A        |
| Transform           | 0.593      | N/A        | N/A        |


### Key Findings
1. **Best Algorithm**: [Your observation]
2. **Best Preprocessing**: [Your observation]
3. **Optimal Cluster Number**: [Your observation]

## Visualizations
## Results

### Silhouette Scores
![Silhouette Score Comparison](silhouette.png)

### Calinski-Harabasz Scores
<img src="calinski.png" width="500">

### Davies-Bouldin Scores
![Davies-Bouldin Results](davies.png "Lower values are better")


## Conclusion
## Key Findings

- **Mean Shift** performed best overall:
  - Highest Silhouette = `0.819`  
  - Lowest Davies-Bouldin = `0.241` (with normalization)  
  - Auto-detects clusters (less control)

- **K-Means (3 clusters + T+N+PCA)** was the top configurable method:
  - Silhouette = `0.649`  
  - Davies-Bouldin = `0.516`  

- **Cluster Count Insight**:  
  `3 clusters` consistently outperformed 4–5 clusters, matching the Iris dataset's natural structure.

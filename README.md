# DSC-212-Assignment-SwizzleSJain
Research Assignment: Modularity on the Karate Club Grap

### Overview
In this notebook, I implemented Newman's recursive spectral bisection algorithm to detect communities in Zachary's Karate Club network. Starting from the modularity matrix B = A - (k kᵀ) / 2m, the code splits subgraphs along the signs of the leading eigenvector u₁ of the restricted generalized modularity matrix, stopping once the leading eigenvalue satisfies λ₁ ≤ 0. After each split, I tracked and plotted how node-level metrics—degree, betweenness, closeness centrality, and clustering coefficient—shift as communities separate

I used Gemini to help structure the NetworkX visualization and multi-panel metric plotting code. Before putting everything together, I went through the mathematical derivations in the handout myself—specifically why the Rayleigh–Ritz theorem gives the leading eigenvector as the relaxed maximizer, and why λ₁ ≤ 0 guarantees no further split gives a positive modularity gain (ΔQ > 0)]—and wrote the discussion based on my own observations of the plots

# CaltechImageSearch

Originally Done by Mohamed Aly at http://vision.caltech.edu/malaa/software/research/image-search/
This Matlab package implements several algorithms used for large scale image search. The algorithms are implemented in C++, with an eye on large scale databases. It can handle millions of images and hundreds of millions of local features. It has MEX interfaces for Matlab, but can also be used (with possible future modifications) from Python and directly from C++. It can also be used for approximate nearest neighbor search, especially using the KdTrees or LSH implementations. The algorithms can be divided into two broad categories, depending on the approach taken for image search:

    Bag of Words (BoW)
    The images are represented by histograms of visual words.

    It includes algorithms for computing dictionaries:
        K-Means.
        Approximate K-Means (AKM).
        Hierarchical K-Means (HKM).

    It also includes algorithms for fast search:
        Inverted File Index.
        Inverted File Index with Extra Information (for example for implementing Hamming Embedding).
        Min-Hash.

    Full Representation (FR)
    The images are represented by the individual features.

    It includes algorithms for fast approximate nearest neighbor search:
        Kd-Trees (Kdtree).
        Hierarchical K-Means (Hkm).
        Locality Senstivie Hashing (LSH), with several hash functions:
            Hamming hash function (bit sampling, approximates hamming distance) i.e. h = x[i]
            Cosine hash function (random hyperplanes through the origin, approximates dot product) i.e.h = sign(<x,r>)
            L1 hash function (approximates the L1 distance) i.e. h = floor((x[i]-b) / w)
            L2 hash function (random hyperplanes with bias, approximates euclidean distance, similar to E2LSH) i.e. h = floor((<x,r> - b) / w)
            Spherical Simplex (approximates distances on the unit hypersphere)
            Spherical Orthoplex (approximates distances on the unit hypersphere)
            Spherical Hypercube (approximates distances on the unit hypersphere)
            Binary Gausian Kernels (approximates gaussian kernel)






This is just a modification of origial built to get it sucessfully compiled with MATLAB 2015 and VS2013.



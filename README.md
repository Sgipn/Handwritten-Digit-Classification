# Handwritten Digit Classification

This is a term project for MAT167:Applied Linear Algebra, Fall 2021 at the University of California, Davis.  
All computations are performed on MATLAB.

MATLAB Toolboxes: Statistics and Machine Learning Toolbox

Our objective is to find the most accurate algorithm with the lowest time complexity for classifying handwritten images. We evaluated the five algorithms: simple algorithm, k means clustering, k nearest neighbors, tangent distance, and singular value decomposition.

We identified the K-nearest-neighbors algorithm (k=1, inverse-weighting, and Euclidean distances) to be the highest performing algorithm at 96.6% classification accuracy and 34.6s run time. The lowest performing algorithm was Tangent distance with a 10.66% classification accuracy and 2417s run time. 

Note: 
* If cubic distances were used for the k-nearest-neighbors-- the accuracy could be bumped up to 97.7% but this increased runtime to 1144.6s. Cosine, Euclidean and Manhattan distances had a similar prediction accuracy to run time ratio; A visualization of performance comparisons between these algorithms can be found on slide 10 of "MAT 167 Final Group Project.pptx". 
* k=1 yielded the most accurate results in knn-- even with 10-fold cross validation. With a low bias/high variance model; we speculate that our data exhibits a high degree of noise.  
* If smoothing was implemented on the Tangent distance algorithm; performance classification accuracy could potentially be increased signfiicantly to ~90%; this is shown from MNIST implementation of tangent distances (using an alternate data source) with a 21.35% classification accuracy without smoothing and 91.41% classification accuracy with smoothing. 

Collaborators: Kevin Xu, Darya Petrov, Katya Katsy, Jedidiah Harwood.

# Image_Search_Engine
Created a image search engine  for small database of images using Color Histograms

Image Search Engine is also named as Content-Based Image Retrieval System. Any retrieval system includes 4 distinct steps:
* Defining image descriptor: Image descriptor provides feature vectors which draw from images based on color Histograms
* Indexing Dataset: After getting the Image descriptor ready, apply same process to each and every image to extract features and store them separately in a file.
* Similarity Metric: To compare two images, there should be some measure like Euclidean distance, Cosine distance, and chi-squared distance. The similarity metric depends on the features.
* Searching: In searching section, a query image is passed to retrieve the images which are similar. Most relevant images are retrieved from the indexed images based on the similarity metric.

#### One of the limitations for this type of search engine is the Scalability.

To run the code, command arguments are used
- for indexing: `python index.py --dataset dataset --index index.csv`
- for retrieving: `python search.py --index index.csv --query queries/imageName.jpg --result-path dataset`

Reference: [Image search engine based on the Color Histograms](https://www.pyimagesearch.com/2014/12/01/complete-guide-building-image-search-engine-python-opencv/)









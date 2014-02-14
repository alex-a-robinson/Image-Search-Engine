# Image search engine
This project is following the [Hobbits and histograms](http://www.pyimagesearch.com/2014/01/27/hobbits-and-histograms-a-how-to-guide-to-building-your-first-image-search-engine-in-python/) tutorial. It is being used by me to learn basic image processing in python.

## Example uses
1. Index the files - Create an index of all the files in the dataset, this will be the images which queries will be run against.
    `python index.py -d dataset/ -i index`
2. Query the indexed files
    `python main.py -d dataset/ -i index -q queries/shire-query.png`
    
## Options
### index.py
* -d, --dataset : Path to the directory that contains the images which will be indexed. (Note: only collects .png files)
* -i, --index : Path to where the index will be stored

### main.py
* -d, --dataset : Path to the directory that contains the images which have been indexed (needed so images can be displayed)
* -i, --index : Path to the index file
* -q, --query : Path to the query image
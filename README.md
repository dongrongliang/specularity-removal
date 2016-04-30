# Specularity removal in multi-viewpoint images

The package is an open source utility to remove specularity in Images that has been captured from multiple viewpoints.

#### Disclaimer
The method uses Homography to find the best pixels available in other viewpoint images. It will not work if the object is not planar.

## Requirements:
- Numpy
- OpenCV

Works with both Python 2.7+ and Python 3+

## Usage
```python
fnames = [
    'data/pshycology-book-1.jpg',
    'data/pshycology-book-2.jpg',
    'data/pshycology-book-3.jpg'
]
remove_specularity(fnames)
```

## Example 1
#### Using two input images
<img src="data/calculus-book-1.jpg" alt="Calculus Book 1" width="200" />
<img src="data/calculus-book-2.jpg" alt="Calculus Book 2" width="200" />
### Output
<img src="results/calculus-book-1.jpg" alt="Calculus Book 1" width="200" />
<img src="results/calculus-book-2.jpg" alt="Calculus Book 2" width="200" />

## Example 2
#### Using three input images
<img src="data/pshycology-book-1.jpg" alt="Calculus Book 1" width="200" />
<img src="data/pshycology-book-2.jpg" alt="Calculus Book 2" width="200" />
<img src="data/pshycology-book-3.jpg" alt="Calculus Book 2" width="200" />
### Output
<img src="results/pshycology-book-1.jpg" alt="Calculus Book 2" width="200" />
<img src="results/pshycology-book-2.jpg" alt="Calculus Book 2" width="200" />
<img src="results/pshycology-book-3.jpg" alt="Calculus Book 2" width="200" />


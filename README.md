# kerfex
Generic feature extraction using [keras pre-built CNN's](https://keras.io/api/applications/) with imagenet weights.

## Getting Started
#### Dependencies
You need Python 3.7 or later to run **kerfex**. You can find it at [python.org](https://www.python.org/).

You aso need pandas, numpy, keras and tensorflow packages, which is available from [PyPI](https://pypi.org). If you have PyPI, run:
```
pip install pandas numpy keras tf-nightly
```
#### Installation
Clone this repo to your local machine using:
```
git clone https://github.com/caiocarneloz/kerfex.git
```
Or install it using pip:
```
pip install kerfex
```
### Usage
The [demo.py](https://github.com/caiocarneloz/kerfex/blob/main/demo.py) file shows a simple example using VGG16 with three [Unsplash](https://unsplash.com/) images from the authors [@mybibimbaplife](https://unsplash.com/@mybibimbaplife), [@davidbraud](https://unsplash.com/@davidbraud), and [@analoglugunler](https://unsplash.com/@analoglugunler). The "extract" function requires:

- **CNN instance itself**
- **CNN pre-processing module**
- **List of images**
- **Images shape**

As return, the function will send a pandas Dataframe containing the numerical features extracted from every image, where each line represents a single image and each column represents a single feature:
```
                0          1          2   ...      15599     15600     15601
	
0  	 0.000000   0.000000   0.000000   ...   0.000000  0.000000  3.754401
1  	 0.000000  15.284859  37.369953   ...  22.756908  6.398854  0.000000
2  	12.172541   0.000000   0.000000   ...   0.000000  0.000000  0.000000
```

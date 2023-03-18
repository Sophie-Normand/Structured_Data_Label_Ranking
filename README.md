# Structured_Data_Label_Ranking
## Authors: CLERGUE Eva, NORMAND Sophie
### Analysis of the paper "A Structured Prediction Approach for Label Ranking" 

The code has been adapted from https://github.com/akorba/Structured_Approach_Label_Ranking. 
It has been adapted in Python 3.

In order to run our code correctly in Python 3, you will need to install the "operalib" library, and then make the following changes:

- In the file awful.py, that can be found in "/opt/anaconda3/lib/python3.8/site-packages/operalib/datasets":
    - comment the imports beginning by ``from numpy import``
    - replace the ``np.bool`` and ``np.float`` instructions by ``bool`` and  ``float`` from Python.

- In the file signal.py, that can be found in "/opt/anaconda3/lib/python3.8/site-packages/operalib/datasets":
    - comment the line ``from sklearn.externals.six.moves import xrange``
    - replace it by ``import six``
                    ``from six.moves import xrange``

## Performing Numerical Experiments

To run the Kemeny approach:

```
python Kemeny.py
```

To run the Hamming approach:

```
python Hamming.py
```

To run the Lehmer approach:

```
python Lehmer.py
```


## Improvement of the Hamming approach

We have improved the performance of the Hamming approach. We have corrected the way Hamming embedding is calculated.

To run our improved Hamming approach:

```
python Hamming_v2.py
```

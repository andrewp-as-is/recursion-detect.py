[![](https://img.shields.io/pypi/pyversions/recursion-detect.svg?longCache=True)](https://pypi.org/pypi/recursion-detect/)
[![](https://img.shields.io/pypi/v/recursion-detect.svg?maxAge=3600)](https://pypi.org/pypi/recursion-detect/)
[![Travis](https://api.travis-ci.org/looking-for-a-job/recursion-detect.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/recursion-detect.py/)

#### Install
```bash
$ [sudo] pip install recursion-detect
```

#### Functions
function|description
-|-
`recursion_detect.depth()`|return recursion depth. 0 if no recursion

#### Examples
```python
>>> import recursion_detect
>>> def recur():
    depth = recursion_detect.depth()
    print("depth = %s" % depth)
    if depth==5:
        return
    recur()

>>> recur()
0
1
2
3
4
```

<p align="center"><a href="https://pypi.org/project/readme-md/">readme-md</a> - README.md generator</p>
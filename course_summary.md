# Course Summary

## Day 1: Getting started and Basics of Python
### Goals
1) Navigate in the shell application: terminal/cmd
2) Python installation (through anaconda installed)
3) Running Python (and Ipython) console in terminal/cmd
4) Creating (and running) Python scripts
5) Running Jupyter lab
6) Python data structures: int, float, string,
7) Introduction to Collections/sequences (Tuples, Lists, Dictionaries). Talk about differences between each data type (summarize in a table)
8) Indexing and Slicing
9) Loops
10) Functions

### Content
- learn shell commands like `ls, cd, pwd, mkdir, cp, mv, rm, rm -r, touch, echo, cat` (and the associated commands on windows cmd)
- Download and install anaconda, run Python console in terminal/cmd (i,e., open, close, etc.)
- Open console, getting help, advantage compared to python console.
- Open it, create a notebook, write code in cells, write markdown in cells, execute and create cells, delete cells, restart the kernel, close the notebook, stop the notebook server.
- python data types: `boolean, int float, string, list, dict, tuple`
- operators: `+, -, /, *, **, %`
- methods associated with data types, e.g., essential string methods, essential list methods.
- if-elif-else statements, conditional variable assignment, `in` operator
- list and tuple indexing, dict indexing, mutability vs. immutability,
- `while` loops, `for` loops, concept of iterator and generator, using `enumerate`,  and `zip`, combining them.
- iterating through dictionaries

### Resources
- https://www.codecademy.com/learn/learn-the-command-line
- https://www.python.org/about/
- https://ipython.readthedocs.io/en/stable/
- https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook
- https://jupyter-notebook.readthedocs.io/en/stable/
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

### Exercise
- https://www.practicepython.org/exercise/2014/01/29/01-character-input.html

---

## Day 2: (Cont.) Basics of python; Numpy and Matplotlib
### Goals
1) Recap of Day 1
2) Boolean and flow control (if-else statements)
3) List comprehension (combines loop, slicing, and if statement)
4) What is a Numpy array, and why to use them? (motivation)
5) Importing and Generating Data
6) Getting insight about the Data (type, dimension, size, etc.)
7) Manipulating the array (arithmetic operations, transpose, etc.)
8) Create different types of figures (e.g., line, scatter, etc.)

### Content
- Boolean data structure, logical operations (and, or, etc.) and flow control
- list comprehension, conditional list comprehension
- Import data:
    - `np.load()`
    - `np.loadtxt()`
    - `np.genfromtxt()`<br><br>
- Creating Numpy arrays
    - `np.zeros()`
    - `np.ones()`
    - `np.random.random()`
    - `np.empty()`
    - `np.full()`
    - `np.full_like()`
    - `np.eye()`
    - `np.identity()`<br><br>
- Data Inspection (assuming we have Numpy a array object called `data`)
    - `data.dtype`
    - `data.ndim`
    - `data.shape`
    - `data.size`
    - `data.strides`
    - `data.min()`
    - `data.max()`
    - `data.mean()`
    - `data.std()`
    - `data.cumsum()`<br><br>
- Data Transformation (assuming we have a Numpy array object called `data`)
    - `data.T`
    - `data.reshape()`
    - `data.resize()`
    - `np.expand_dims()`
    - `np.ravel()`
    - `np.add()`, `np.subtract()`, `np.multiply()`, `np.divide()`, `np.remainder()`
    - `np..exp()`, `np.log()`
    - Masking using list (or array) of True and False values <br><br>
- Create a simple line plot using `plt.plot()`
- Create a simple scatter plot using `plt.scatter()`

### Resources
- https://github.com/cne-tum/msne-datascience-2018/blob/master/notebooks/block1/block1_session2_basic_python.ipynb
- https://github.com/cne-tum/msne-datascience-2018/blob/master/notebooks/block1/block1_session2_programming_concepts.ipynb
- https://www.codecademy.com/learn/learn-python
- https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PythonForDataScience.pdf

### Exercises
- https://www.practicepython.org/exercise/2014/02/26/04-divisors.html
- https://www.practicepython.org/exercise/2014/03/19/07-list-comprehensions.html
- https://www.practicepython.org/exercise/2017/01/24/33-birthday-dictionaries.html
- https://www.datacamp.com/courses/intro-to-python-for-data-science

---

## Day 3: Numpy and Matplotlib; Pandas (and Seaborn)
### Goals
1) Recap of Day 1 and 2
2) Slicing and Masking
3) Combining arrays
4) Saving data
5) Customize the figure (e.g., color, style, size, etc.)
6) Put several figures together (i.e., subplots)
7) Save the figure (after this we'll have an exercise for image processing)
8) Understand the positioning of Pandas in the data science pipeline and the convenience supplied by /labeled data structures/, /automatic missing data handling/, /column-oriented layouts/, /embodiment of relational algebra/ and /rich C-level implementation of a functional map/reduce like API/.
9) Understand row and column-oriented access patterns, know the customary layout of observations x attributes for data science.
10) Understand `pd.DataFrames` data structures and its properties as compared to known basic Python data structures.
11) Be able to read textual tabular data from the file system and remote URLs.
12) Practice access to data and metadata.
13) Use grouping operations and allowable reductions on them ('split-apply-combine')
14) Express composable map operations in Pandas with anonymous functions
15) Appreciate the advantages of splitting (/normalizing/) observational statements to prevent duplication and how table joins allow to operate practically in this setting.

### Content
- Combining multiple arrays and splitting an array
    - `np.concatenate()`
    - `np.append()`
    - `np.hstack()`
    - `np.vstack()`
    - `np.hsplit()`
    - `np.vsplit()` <br><br>
- Saving Numpy arrays
    - save(): saves data in .npy format
    - savez(): Save several arrays into an uncompressed .npz archive
    - savez_compressed():
    - savetxt():
- Modify the data representation (line color, width, point size, markers, and style)
- Modify the axes (xlim, ylim, ticks and ticklabels, etc.)
- Save a (high quality) figure using `plt.savefig()`
- Series and data frames created from dictionaries and (nested) lists.
- `read_csv` with different urls, separators.
- metadata accessors (`index`, `columns`, `info`, `dtypes`, `shape`, `len`) and data (`.values`, .`iloc`, `loc`, `head`, `tail`). Multiple uses of `[]`: element access in series, column access in data frames, boolean indexing with conforming arrays.
- grouping operations `groupby`, `value_counts`, `(n)unique`.
- chainable mapping with `apply` and `lambda` functions. Compare with for-loop iteration.
- caveats in assignment, `df.attribute = something` will not create a new column
- reduction operations `min`, `max`, `mean`, `std`, `median`, `count` and descriptive statistics with `describe`
- sorting with `sort_values`
- `merge` and the join key
- understand the relationship of seaborn with matplotlib and the added value of the former.

### Resources
* https://www.datacamp.com/community/tutorials/python-numpy-tutorial
* [Cheat sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)
- https://www.datacamp.com/courses/introduction-to-data-visualization-with-python (first two blocks)
- https://matplotlib.org/gallery.html
- https://github.com/matplotlib/AnatomyOfMatplotlib
- https://github.com/jbmouret/matplotlib_for_papers
- https://jakevdp.github.io/blog/2013/07/10/XKCD-plots-in-matplotlib/
- https://jakevdp.github.io/blog/2012/10/07/xkcd-style-plots-in-matplotlib/
- [Cheat sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Matplotlib_Cheat_Sheet.pdf)
- [Pandas cheatsheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
- [Pandas exercises](https://github.com/guipsamora/pandas_exercises)
- [Pandas documentation](https://pandas.pydata.org/)
- [Seaborn Gallery](http://seaborn.pydata.org/examples/index.html)
- [Seaborn introduction](https://seaborn.pydata.org/introduction.html)
- [Jake van der Plas' intro to Seaborn](https://jakevdp.github.io/PythonDataScienceHandbook/04.14-visualization-with-seaborn.html)

### Exercises
#### Pandas
Looking at the Pandas cheatsheet and recurring to the interactive documentation or the API docs linked above, try to solve the following three notebooks. Then, check your answers against the provided solutions, try to understand and come up with precise questions for any remaining doubt.
- https://github.com/guipsamora/pandas_exercises/tree/master/02_Filtering_%26_Sorting/Fictional%20Army
- https://github.com/guipsamora/pandas_exercises/tree/master/03_Grouping/Alcohol_Consumption
- https://github.com/guipsamora/pandas_exercises/tree/master/05_Merge/Fictitous%20Names

If you want more challenges, go for the following:
- https://github.com/guipsamora/pandas_exercises/tree/master/02_Filtering_%26_Sorting/Euro12
- https://github.com/guipsamora/pandas_exercises/tree/master/03_Grouping/Regiment
- https://github.com/guipsamora/pandas_exercises/tree/master/05_Merge/Housing%20Market

## Day 4: OOP, Debugging, Practical aspects (e.g., git (and GitHub, etc.)
### Goals
1) Recap of Day 1, 2, and 3
2) An introduction to Object-oriented programming. What are classes and objects
3) Learning how to debug (or explore) the code and the tools available for such purpose
4) Some practical aspects of programming and handling projects:
  - git and GitHub
  - How to navigate in file systems in Python (os and glob packages)
  - How to import functions from different python scripts
  - How to organize projects
  - How to package and publish code on PyPI
  - etc.

### Content
- Start by a recap from previous days, and a warm up exercise which integrates and refreshes as many taught concepts as possible
- A brief explanation (and discussion) about utility of a debugger
- What are different tools available for debugging Python code, and how to use them
- And introduction to OOP (classes, objects, and inheritance)
- Introduction to GitHub. Everyone is to have a GitHub account during this session. Create Repos, Clone, Make changes, Push, Pull, create branch(es), Push, Merge, Pull, etc.
- We will finish by a fun project (something that involves a group discussion and planning, have most of the concepts within it and can be visualized) and we will practice collaboration, and peer programming for this project and at the end we have something nice which reminds us of this Workshop and will publish it on out GitHub accounts

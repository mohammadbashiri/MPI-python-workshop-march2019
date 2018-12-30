# Course Summary
# Block 1 

## Day 1: Getting started and Basics of Python 
### Goals 
1) Navigate in the shell application: terminal/cmd
2) Python installation (through anaconda installed)
3) Running Python (and Ipython) console in terminal/cmd
4) Creating (and running) Python scripts
5) Running Jupyter lab
6) Basics of Python: Python data types: int, float, string (a little bit of indexing)

### Content 
**Shell**: learn shell commands like `ls, cd, pwd, mkdir, cp, mv, rm, rm -r, touch, echo, cat` (and the associated commands on windows cmd)
**Python**: download and install anaconda, run Python console in terminal/cmd (i,e., open, close, etc.)
**IPython**: open console, getting help, advantage compared to python console.
**Jupyter notebook**: open it, creat a notebook, write code in cells, write markdown in cells, execute and create cells, delete cells, restart the kernel, close the notebook, stop the notebook server. 

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

## Day 2: (Cont.) Basics of python
### Goals
1) Recap of Day 1: Console, Script, Jupyter notebook, (some of the) Python data types
2) Contibuation with python variables and data types
3) Introduction Collections/sequences (Tuples, Lists, Dictionaries). Talk about differences between each data type (simmarize in a table)
4) Indexing, slicing
5) Loops
6) Functions
7) Booleans and flow control (if-else statements)

### Content 
- python data types: `boolean, int float, string, list, dict, tuple`
- operators: `+, -, /, *, **, %`
- methods associated with data types, e.g., essential string methods, essential list methods. 
- if-elif-else statements, conditional variable assignment, `in` operator
- list and tuple indexing, dict indexing, mutability vs. immutability, 
- `while` loops, `for` loops, concept of iterator and generator, using `enumerate`,  and `zip`, combining them. 
- iterating through dictionaries
- list comprehension, conditional list comprehension

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

## Day 3: Numpy and Matplotlib;
### Goals 

1) Recap of Day 1 and Day 2
2) List comprehension (combines loop, slicing, and if statement)
3) What is a Numpy array, and why to use them? (motivation)
4) Importing and Generating Data
5) Getting insight about the Data (type, dimension, size, etc.)
6) Manipulating the array (arithmetic operations, transpose, etc.)
7) Slicing and Masking
8) Combining arrays
9) Saving data
10) Create different types of figures (e.g., line, scatter, etc.)
11) Customize the figure (e.g., color, style, size, etc.)
12) Put several figures together (i.e., subplots)
13) Save the figure


### Content 

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
- Data Inspection (assuming we have numpy a array object called `data`)
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
- Data Transformation (assuming we have a numpy array object called `data`)
    - `data.T`
    - `data.reshape()`
    - `data.resize()`
    - `np.expand_dims()`
    - `np.ravel()`
    - `np.add()`, `np.subtract()`, `np.multiply()`, `np.divide()`, `np.remainder()`
    - `np..exp()`, `np.log()`
    - Masking using list (or array) of True and False values <br><br>
- Combining multiple arrays ans splitting an array
    - `np.concatenate()`
    - `np.append()`
    - `np.hstack()`
    - `np.vstack()`
    - `np.hsplit()`
    - `np.vsplit()` <br><br>
- Saving numpy arrays
    - save(): saves data in .npy format
    - savez(): Save several arrays into an uncompressed .npz archive
    - savez_compressed():
    - savetxt():
- Create a simple line plot using `plt.plot()`
- Create a simple scatter plot using `plt.scatter()`
- Modify the data representation (line color, width, point size, markers, and style)
- Modify the axes (xlim, ylim, ticks and ticklabels, etc.)
- Save a (high quality) figure using `plt.savefig()`

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

---


# Block 2
## Session 6: Pandas and seaborn
### Goals 
1. Understand the positioning of Pandas in the data science pipeline and the convenience supplied by /labeled data structures/, /automatic missing data handling/, /column-oriented layouts/, /embodiment of relational algebra/ and /rich C-level implementation of a functional map/reduce like API/. 
1. Understand row and column-oriented access patterns, know the customary layout of observations x attributes for data science.
1. Understand `pd.Series` and `pd.DataFrames` data structures and their properties as compared to known basic Python data structures.
1. Be able to read textual tabular data from the filesystem and remote urls.
1. Practice access to data and metadata.
1. Use grouping operations and allowable reductions on them ('split-apply-combine')
1. Express composable map operations in Pandas with anonymous functions
1. Appreciate the advantages of splitting (/normalizing/) observational statements to prevent duplication and how table joins allow to operate practically in this setting.
1. Enumerate available dimensions of graphical variation to accomodate categorical and continuous data
 
### Content
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

For even more you can choose directly from the list of available topics.

#### Seaborn
Choose one graphical display from the Seaborn gallery (see Resources above), choose one of the datasets now known to you from the exercises (or any other of your interest, check out kaggle.com or data.world) and make a Seaborn plot with at least four dimensions of variation reflecting a mixture of continuous and discrete attributes.

For your upcoming final project, make at least one of the final presentation plots using Seaborn.

## Session 7: scikit-learn

### Goals 
1. Understand (short) programs
1. Exposure to central concepts of machine learning
1. Examples of data analysis workflows
1. Learn scikit syntax

### Content 
- Short introduction to machine learning
- sklearn tutorials:
    - Load datasets and explore (identify input data, target data within numpy arrays)
    - Visualize data (with matplotlib)
    - Apply simple ML methods with .fit(): PCA, KMeans

### Resources
- https://scikit-learn.org/
- https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html
- https://scikit-learn.org/stable/auto_examples/cluster/plot_cluster_iris.html

# Block 3 
## Session 1 
### Goals
- have an overview of editors and programming environments for python.
- know why and how to use anaconda environments.
- find a project and decide.
- create an environment for your project, choose an editor for your project.
- start working on your project. 

### Lecture 1 Editors
Overview of editors: 
- [pycharm](https://www.jetbrains.com/pycharm/), 
- [atom](https://atom.io/), 
- [emacs](https://www.gnu.org/software/emacs/tour/index.html), 
- [vi](https://www.guru99.com/the-vi-editor.html)

[Slides in a notebook: link](notebooks/block3/block3_session1_editors.ipynb)
    
### Lecture 2 Anaconda environments 
Short intro to anaconda envs, demo. Have a look at 
- https://medium.freecodecamp.org/why-you-need-python-environments-and-how-to-manage-them-with-conda-85f155f4353c
- https://conda.io/docs/user-guide/tasks/manage-environments.html

### Choosing projects
overview of projects: [here](projects/project_overview.md)


## Block 4 
### Session 2 -- Introduction to deep learning frameworks

#### Goals

-   Understand the scaffolding of deep learning: function learning, empirical risk minimization + regularization, matrix products, taking derivatives, following gradients, expressing complex computational graphs.
-   Understand the forward pass in terms of function composition of matrix products and nonlinearities
-   Appreciate the interest of moving matrix products to the GPU and how to do it in PyTorch.
-   Understand the principle of backpropagation, and how to indicate in PyTorch that gradients will be required.
-   Obtain a qualitative understanding of the pitfalls and limitations of gradient learning. Know where to find optimizers and tune learning rates in PyTorch.
-   Find in PyTorch the building blocks to conveniently create multilayer neural networks.
-   Identify helpful framework services for the industrialisation of deep networks: distributed training, model serving, checkpointing, model porting (onnx), monitoring, export to embedded/mobile.

#### Content

See the [slides](slides/block_4/deep_learning.pdf).

#### References

-   [Deep learning with PyTorch: a 60-minute blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)
-   Géron: hands-on machine learning with scikit-learn and tensoflow
-   [Deep Learning Book](https://www.deeplearningbook.org/)


#### Exercises

Find an example of a network defined in PyTorch and identify in the code the places where a) network definition b) loss function specification c) optimizer choice d) learning rate scheduling (if applicable) e) checkpointing or monitoring (if applicable) are happening. Discuss what aspects of the code represent regularization strategies and if there are any explicit regularization terms in the cost function.

# Pandas 🐼 and Git 🫴🏼 task
This task is fully customizable, you can choose to do it however may you like, but you have to do it. You are encouraged to use the internet to search for answers, use information from the task Menna sent you, and use info from this task there. And of course ask your colleagues for help whenever you need it! 🤗
## Pandas 🐼

### 1. What is Pandas?

Pandas is a Python library used for working with data sets, you should know this by now. It has functions for analyzing, cleaning, exploring, and manipulating data. The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

Speaking of *analyzing, cleaning, exploring, and manipulating* data, what functions can you use for each of these tasks? 🤔:
- **A**nalyze data?
- **C**lean data?
- **E**xplore data?
- **M**anipulate data?

**Fill the table below:**
  

function | what it does | category
------------ | ----------- | ---------
`astype()` |  Convert the data type of columns  |  clean
`groupby()` | Group data based on one or more columns  |  analyze
`sort_values()` | Sort the rows of a DataFrame |  manipulate 
`pivot_table()` | pivots a DataFrame |  manipulate
`merge()` | Combine two DataFrames |  manipulate
`plot()` | Create plots and visualizations  | explore  
`corr()` | Compute the correlation between columns |   analyze
`cov()` | Compute the covariance between columns   | analyze 
`apply()` | Apply a function on a DataFrame  | manipulate 
`loc()` | Access rows and columns by labels |  explore
`iloc()` | Access rows and columns by index |  explore  
`iterrows()` | Iterate over DataFrame rows as pairs. |  explore 
`aggregate()` | Apply one or more aggregation operations to the data. | analyze

$\rightarrow$ You may insert code snippets here if you like!

### 2. Pandas and NumPy 🔢 [BONUS 🎁](https://www.imdb.com/title/tt1068680/)

Pandas is built on top of the NumPy package, which means that many of the methods in NumPy are also available in Pandas. Data in pandas is often used to feed statistical analysis in SciPy, plotting functions from Matplotlib, and machine learning algorithms in Scikit-learn.

Speaking of NumPy, here are questions about it:

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.vstack((a, b))

print(c[1][2])
```
- answer: `6`
- explaination : vstack vertically stacks arrays a and b to form a new 2D array. which means a become the first row and b become the second row and when accessing `c[1][2]` you access the second row and third column which is `6`

---

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.intersect1d(a, b)

print(c)
```
- answer: `[]` (empty array)
- explaination : `np.intersect1d()` function finds the intersection of arrays a and b (elements in both a and b). Because there is no common numbers between a and b the result is an empty array

---

  
- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.setdiff1d(a, b)

print(c)
```
- answer: `[1 2 3]`
- explaination : `np.setdiff1d()` function finds the set difference of arrays a and b (element in a not in b). So the result is a because there is no common numbers between a and b
---

- Which of the following is a function in NumPy used for carrying out Einstein summations?

    - [ ]  `np.tensordot()`
    - [ ]  `np.dot()`
    - [x]  `np.einsum()`
    - [ ]  `np.outer()`

- The `np.outer` function is primarily intended for:

    - [ ]  Computing the tensor dot product of two arrays.
    - [x]  Computing the outer product of two arrays.
    - [ ]  Computing the inner product of two arrays.
    - [ ]  Computing the cross product of two arrays.


### 3. Pandas and Matplotlib 📈
Pandas can be used to visualize data using a wrapper for `matplotlib.pyplot.plot()`. You can plot data directly from your DataFrame using certain functions.

- What functions can you use to plot data directly from your DataFrame? 🤔
  
  `DataFrame.plot(kind='')`, you can specify the kind parameter with the plot you want

  ---


- What is the output of the following code? And why is it so?

``` python
df = pd.DataFrame(np.random.randn(10, 4), columns=['a', 'b', 'c', 'd'])
df.plot.scatter(x='a', y='b')
```
first a DataFrame with random data with 10 rows and 4 columns is created. then  a scatter plot is created using the plot.scatter() function. 

---
- What do you know about `np.random.randn()`? And how does it depend on `np.random.seed()`?

    `np.random.randn()` is a function that generates random numbers from a standard normal distribution (the mean is 0 and the standard deviation is 1), `np.random.seed()` specifies a seed (initial value that determines the sequence of random numbers generated). if specifymthe sequence of random numbers generated is the same every time you run your code. 

---
## Git 🫴🏼
I know you are all familiar with Git, but let's see how much you know about it! 🤓

- What is the default text editor for the Bash shell with a Windows-based Git install?

    - [ ] Emacs
    - [x] Vim
    - [ ] Notepad++
    - [ ] Bash

- Before you install Git, which of the following prerequisite products must be present and configured on your local OS?

    - [ ] Python
    - [ ] Java Development Kit 1.8 or newer
    - [ ] Apache Maven
    - [x] Nothing


- After you install Git and prior to issuing the first commit, which two configuration properties does the tool expect to be configured?

    - [x] username and email address
    - [ ] username and password
    - [ ] email address and password
    - [ ] username and IP address

- Which of the following commands is used to create a new Git repository?

    - [x] git init
    - [ ] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to clone a remote Git repository?

    - [ ] git init
    - [x] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to stage a file for inclusion in the next commit?

    - [x] git add
    - [ ] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to commit staged changes to the local repository?

    - [ ] git add
    - [x] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to push committed changes to a remote repository?

    - [ ] git add
    - [ ] git commit
    - [x] git push
    - [ ] git pull

- Who is attributed with inventing Git?

    - [ ] Junio Hamano
    - [ ] James Gosling
    - [ ] Kohsuke Kawaguchi
    - [x] Linus Torvalds

- After you initialize a new Git repository and create a file named git-quiz.html, which of the following commands will not work if issued?

    - [x] git add git-quiz.html
    - [ ] git status
    - [ ] git add .
    - [ ] git commit -m "git quiz web file added"

- Which file can you configure to ensure that certain file types are never committed to the local Git repository?

    - [ ] ignore.git
    - [x] .gitignore
    - [ ] gitignore.txt
    - [ ] git.ignore

- Under which circumstance should you use a single dash within a bash command, as opposed to a double dash?

  if the option is a single char use single dash if more use double dash

   ---

- Which vendor acquired GitHub for $7.5 billion in June 2018?

  Microsoft

  ---

You may want to check [this](https://www.youtube.com/watch?v=Q6G-J54vgKc&t=16813s)

## Problem Solving 🤔
[A. Panoramix's Prediction](https://codeforces.com/problemset/problem/80/A)

https://codeforces.com/problemset/submission/80/220528269

[A. Again Twenty Five!](https://codeforces.com/problemset/problem/630/A)

https://codeforces.com/problemset/submission/630/220539013

# **Visualization Library Documentation:**

The process of finding trends and correlations in our data by representing it pictorially is called Data Visualization.

To perform data visualization in python, we can use various python data visualization modules such as Matplotlib, Seaborn, Plotly, etc

## **Data Visualization in Python**

Python offers several plotting libraries, namely [Matplotlib](https://www.simplilearn.com/tutorials/python-tutorial/matplotlib), [Seaborn](https://www.simplilearn.com/tutorials/python-tutorial/python-seaborn) and many other such data visualization packages with different features for creating informative, customized, and appealing plots to present data in the most simple and effective way.

##  Table of Contents

- [Introduction](#introduction)
- [Matplotlib](#matplotlib)
  - [Installation](#installation)
  - [Basic Syntax](#basic-syntax)
  - [Graph Types](#graph-types)
- [Seaborn](#seaborn)
  - [Installation](#installation-1)
  - [Basic Syntax](#basic-syntax-1)
  - [Graph Types](#graph-types-1)
- [Comparison](#-comparison-matplotlib-vs-seaborn)
- [Strengths & Limitations](#strengths-and-limitations)
- [Conclusion](#conclusion)


### **Matplotlib:**

Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.

- Matplotlib makes easy things easy and hard things possible.
- Create publication quality plots.
- Make interactive figures that can zoom, pan, update. Customize visual style and layout

#### **Installation:**
```python
pip install matplotlib

#### **Basic syntax:**
```python
import matplotlib.pyplot as plt

#### **Graph types :**

##### **Line plot**

```python
| import matplotlib.pyplot as plt |
| --- |
| x = \[1, 2, 3, 4, 5\] |
| y = \[10, 20, 25, 30, 40\] |
| plt.plot(x, y, marker='o', linestyle='-', color='b') |
| plt.xlabel("X-axis") |
| plt.ylabel("Y-axis") |
| plt.title("Line Plot Example") |
| plt.show() |

##### **Bar chart**

```python
| categories = \['A', 'B', 'C', 'D'\] |
| --- |
| values = \[3, 7, 1, 8\] |
| plt.bar(categories, values, color='g') |
| plt.xlabel("Categories") |
| plt.ylabel("Values") |
| plt.title("Bar Chart Example") |
| plt.show() |

##### **Histogram**

```python
| import numpy as np |
| --- |
| data = np.random.randn(1000) |
| plt.hist(data, bins=30, color='purple', edgecolor='black') |
| plt.xlabel("Value") |
| plt.ylabel("Frequency") |
| plt.title("Histogram Example") |
| plt.show() |

### **Seaborn:**

Seaborn is a Python data visualization library based on matplotlib.

- It provides a high-level interface for drawing attractive and informative statistical graphics.
- Seaborn is a library for making statistical graphics in Python. It builds on top of matplotlib and integrates closely with pandas data structures.

#### **Installation:**

```python
pip install seaborn

#### **Basic syntax:**

```python
| import seaborn as sns |
| --- |
| import matplotlib.pyplot as plt |

#### III. **Graph Types:**

##### **1.Scatter Plot:**

```python
| import seaborn as sns |
| --- |
| import matplotlib.pyplot as plt |
| iris = sns.load_dataset("iris") |
| sns.scatterplot(x="sepal_length", y="sepal_width", data=iris, hue="species") |
| plt.title("Scatter Plot Example") |
| plt.show() |

##### **2.Box plot:**

```python
| sns.boxplot(x="species", y="petal_length", data=iris) |
| --- |
| plt.title("Box Plot Example") |
| plt.show() |

##### **3.Heatmap:**

```python
| import numpy as np |
| --- |
| data = np.random.rand(5, 5) |
| sns.heatmap(data, annot=True, cmap="coolwarm") |
| plt.title("Heatmap Example") |
| plt.show() |

## **Comparison:**


| Feature                           | Matplotlib                                                       | Seaborn                                                                  |
|--------------------- -------------|------------------------------------------------------------------|--------------------------------------------------------------------------|
| **Purpose**                       | General-purpose plotting library                                 | Statistical data visualization library                                   |
| **Complexity**                    | Requires more code for styling and customization                 | Simpler, with built-in themes and styles                                 |
| **Customization**                 | Highly customizable                                              | Limited compared to Matplotlib                                           |
| **Ease of Use**                   | More complex for advanced plots                                  | Easier and more intuitive for quick plots                                |
| **Statistical Plots**             | Limited built-in statistical functions                           | Built-in support for statistical plots like violin, box, and swarm plots |
| **Integration**                   | Works well with NumPy and Pandas                                 | Works seamlessly with Pandas                                             |
| **Interactivity**                 | Mostly static (requires additional libraries for interactivity)  | Limited interactivity, best for static plots                             |
| **Themes & Styles**               | Default style is basic                                           | Aesthetic and readable default themes                                    |
| **Annotations & Legends**         | Requires manual addition                                         | Handles legends and annotations automatically                            | 
| **Performance on Large Datasets** | Can handle large datasets but may require optimization           | Slower performance on very large datasets                                |
| **Basic syntax**                  |import matplotlib.pyplot as plt                                   |import seaborn as sns   import matplotlib.pyplot as plt


## **Strengths and limitations:**

### Strengths

| **Matplotlib**                                       | **Seaborn**                               |
| -----------------------------------------------------|-------------------------------------------|
| Highly Customizable                                  | Aesthetic and Readable Plots              |
| Supports Multiple Output Formats                     | Built-in Statistical Visualization        |
| Wide Range of Plot Types                             | Works Well with Pandas DataFrames         |
| Integration with Other Libraries                     | Less Code, More Insights                  |
| Animation and 3D Support                             | Automatic Handling of Legends and Labels  |
| Offline Usage                                        | Built-in Themes and Color Palettes        |
| Large Community Support                              | Seamless Integration with Matplotlib      |

### Limitations

| **Matplotlib**                                       | **Seaborn**                                  |
| ---------------------------------------------------- | -------------------------------------------- |
| Complex Syntax for Advanced Plots                    | Limited Customization Compared to Matplotlib |
| Not as Aesthetic by Default                          | Not as Versatile for General Plots           |
| Static by Nature                                     | No Built-in Interactivity                    |
| Performance Issues with Large Datasets               | Slower with Large Datasets                   |
| Requires Additional Code for Legends and Labels      | Requires Matplotlib Backend                  |
| Limited Statistical Plotting                         | Less Control Over Axes and Layouts           |

## **Conclusion:**

Both **Matplotlib** and **Seaborn** are essential libraries for data visualization in Python, each with its strengths:

- **Matplotlib** is a **low-level, flexible** library that provides complete control over plot customization. It is best suited for **general-purpose** visualizations where fine-tuned adjustments are needed.
- **Seaborn** is a **high-level, aesthetically pleasing** library built on Matplotlib, making it ideal for **statistical visualizations** with minimal coding effort
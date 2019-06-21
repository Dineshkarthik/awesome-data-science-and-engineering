# Data Science & Engineering

A curated list of Data Science and Engineering frameworks, tools, libraries and related list of tutorials.
This mostly covers python related opensource ones ranging from beginner to intermediate levels.


## Table of Contents

<!-- MarkdownTOC depth=4 -->
- [Big Data](#big-data)
	- [PySpark - Apache Spark Python API](#big-data-pyspark)
- [Frameworks](#frameworks)
	- [Apache Airflow](#frameworks-apache-airflow)
- [Libraries](#libraries)
    - [Pandas](#libraries-pandas)
    - [NumPy](#libraries-numpy)
    - [Alembic](#libraries-alembic)
- [Tools](#tools)
	- [JupyterLab](#tools-jupyterlab)
	- [Google Colab](#tools-colab)

<!-- /MarkdownTOC -->

<a name="big-data"></a>
## Big Data

<a name="big-data-pyspark"></a>
#### PySpark - Apache Spark Python API - [pypi](https://pypi.org/project/pyspark/)
Apache Spark is a fast and general-purpose cluster computing system. It provides high-level APIs in Java, Scala, Python and R, and an optimized engine that supports general execution graphs. It also supports a rich set of higher-level tools including [Spark SQL](https://spark.apache.org/docs/latest/sql-programming-guide.html) for SQL and structured data processing, [MLlib](https://spark.apache.org/docs/latest/ml-guide.html) for machine learning, [GraphX](https://spark.apache.org/docs/latest/graphx-programming-guide.html) for graph processing, and [Spark Streaming](https://spark.apache.org/docs/latest/streaming-programming-guide.html).
- [Homepage](https://spark.apache.org/)
- [Installation](https://www.roseindia.net/bigdata/pyspark/install-pyspark-on-ubuntu.shtml)
- [Documentation](https://spark.apache.org/docs/latest/api/python/index.html)
- [Getting Started](https://www.guru99.com/pyspark-tutorial.html) - overview os sparkcontext, sqlcontext, spark ml, basic operations, data processing.
- [Introduction to Dataframes in PySpark](https://docs.databricks.com/spark/latest/dataframes-datasets/introduction-to-dataframes-python.html) - creating dataframes, commonly used functions on dataframes.
- [Introduction to Dataframes in PySpark - Part 2](https://dzone.com/articles/pyspark-dataframe-tutorial-introduction-to-datafra) - hands on dataframe using opensource datasets.
- [PySpark SQL](https://github.com/apache/spark/blob/master/examples/src/main/python/sql/basic.py) - basics of pyspark sql.
- [Spark SQL, DataFrames and Datasets Guide](https://spark.apache.org/docs/2.2.0/sql-programming-guide.html) - sql, dataframe operations, dataset, aggregation, global temp view,  interoperating with RDDs ...
- [PySpark SQL Cheatsheet](https://cdn.qubole.com/wp-content/uploads/2017/08/PySpark_SQL_Cheat_Sheet_Python.pdf)
- [UDF - User-Defined Functions](https://changhsinlee.com/pyspark-udf/) - register UDFs, invoke UDFs.
- [Using Parquet files](https://spark.apache.org/docs/2.2.0/sql-programming-guide.html#parquet-files) - loading data, paritions, schema merging, metadata refreshing.
- [Structured streaming](https://docs.databricks.com/_static/notebooks/structured-streaming-python.html) - batch/interactive processing, stream processing.
- [Example scripts](https://github.com/apache/spark/tree/master/examples/src/main/python) - set of example scriupts from Apache spark github repo.
- [PySpark Streaming with Kafka/](https://www.rittmanmead.com/blog/2017/01/getting-started-with-spark-streaming-with-python-and-kafka/) - using pyspark StreamingContext connect to kafka and process the data from kafka stream.

#### Study Material
- [Learning Apache Spark with Python](https://runawayhorse001.github.io/LearningApacheSpark/pyspark.pdf)

<a name="frameworks"></a>
## Frameworks

<a name="frameworks-apache-airflow"></a>
#### Apache Airflow - [pypi](https://pypi.org/project/apache-airflow/)
Apache Airflow (or simply Airflow) is a platform to programmatically author, schedule, and monitor workflows.

Use Airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed.
- [Homepage](http://airflow.apache.org/)
- [Installation](http://airflow.apache.org/installation.html)
- [Getting started](https://towardsdatascience.com/getting-started-with-apache-airflow-df1aa77d7b1b) - simple airflow setup and running dags.
- [Key concepts](https://medium.com/@dustinstansbury/understanding-apache-airflows-key-concepts-a96efed52b1a) - DAGs, operators, sensors, tasks
- [Executors](https://www.astronomer.io/guides/airflow-executors-explained/) - explanation on different type of executors
- [Triggering DAGs](https://dabble-of-devops.com/learn-airflow-by-example-part-3-start-building/) - triggering DAG via UI, REST api, Command Line
- [Custom Operator and Sensor](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/) - write your own operator and sensor.
- [Multiple workers with Celery executor](https://blog.sicara.com/using-airflow-with-celery-workers-54cb5212d405) - Using celery executor run mutiple airflow workers
##### Advanced Concepts:
- [Kubernetes operator](https://kubernetes.io/blog/2018/06/28/airflow-on-kubernetes-part-1-a-different-kind-of-operator/) - explanation on how to use k8s operator
- [Using kubernetes executor](https://gist.github.com/kppullin/54d07f557c7c64c321786d6ed40b46e1) - run airflow with kubernetes executor in mini-kube using helm.
- [ Tips, Tricks and Best practises](https://medium.com/datareply/airflow-lesser-known-tips-tricks-and-best-practises-cf4d4a90f8f)
- [Deep Dive into airflow on kubernetes executor](https://www.datacouncil.ai/hubfs/DataEngConf/Data%20Council/Slides%20SF%2019/Running%20Airflow%20reliably%20with%20Kubernetes.pdf) - Running airflow reliabley with Kubernetes. 

<a name="libraries"></a>
## Libraries

<a name="libraries-pandas"></a>
#### Pandas - [pypi](https://pypi.org/project/pandas/)
Library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.
* [Homepage](https://pandas.pydata.org/)
* [Documentation](https://pandas.pydata.org/pandas-docs/stable/index.html) 
* [Basics](https://data36.com/pandas-tutorial-1-basics-reading-data-files-dataframes-data-selection/) - Reading files into data frames and selecting.
* [Aggregation and grouping](https://data36.com/pandas-tutorial-2-aggregation-and-grouping/) - aggregation (such as min, max, sum, count, etc.) and grouping.
* [Data wrangling](https://data36.com/pandas-tutorial-3-important-data-formatting-methods-merge-sort-reset_index-fillna/) - merge, sort, reset_index, fillna.
* [Pivot table](https://pbpython.com/pandas-pivot-table-explained.html) - explains the pandas [pivot_table](http://pandas.pydata.org/pandas-docs/stable/generated/pandas.tools.pivot.pivot_table.html) function and how to use it for data analysis.
* [Pandas plotting](https://towardsdatascience.com/a-guide-to-pandas-and-matplotlib-for-data-exploration-56fad95f951c) - Pandas and Matplotlib to produce the graphs.
* [Time series analysis](https://www.dataquest.io/blog/tutorial-time-series-analysis-with-pandas/) - about powerful time series tools in the pandas library.
* [Pandas Cheatsheet](https://s3.amazonaws.com/dq-blog-files/pandas-cheat-sheet.pdf)

<a name="libraries-numpy"></a>
#### NumPy - [pypi](https://pypi.org/project/numpy/)
NumPy is the fundamental package for scientific computing with Python.
Besides its obvious scientific uses, NumPy can also be used as an efficient multi-dimensional container of generic data. Arbitrary data-types can be defined. This allows NumPy to seamlessly and speedily integrate with a wide variety of databases.
* [Homepage](https://www.numpy.org/)
* [Documentation](https://docs.scipy.org/doc/numpy/user/)
* [Basics](https://docs.scipy.org/doc/numpy/user/basics.html) - Data types, Array creation, I/O with NumPy, Indexing, Broadcasting, Byte-swapping, Structured arrays, Subclassing ndarray
* [Getting started](https://www.datacamp.com/community/tutorials/python-numpy-tutorial) - a little dive into the above mentioned basic concepts.
* [Arrays and Vectorized Computation](https://www.oreilly.com/library/view/python-for-data/9781449323592/ch04.html) - ndarrays, array & scalar operations, transposing arrays and swapping axes
* [Mathematical function](https://www.geeksforgeeks.org/numpy-mathematical-function/) - trigonometric, hyperbolic, exponents and logarithms, complex numeric functions
* [UFuncs - Universal Functions](https://jakevdp.github.io/PythonDataScienceHandbook/02.03-computation-on-arrays-ufuncs.html) - Introduction, expolaration, trigonometric functions, advanced ufuncs, special ufuncs
* [Array manipulation](https://docs.scipy.org/doc/numpy-1.13.0/reference/routines.array-manipulation.html) - changing shapes, transpose-like operations, changing number of dimensions, changing kind of array, joining-splitting-tilling of arrays, adding-removing & rearraning elements
* [Fancy Indexing](https://jakevdp.github.io/PythonDataScienceHandbook/02.07-fancy-indexing.html) - fancy indexing, combined indexing
* [Numpy  Cheatsheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)

<a name="libraries-alembic"></a>
#### Alembic - [pypi](https://pypi.org/project/alembic/)
Alembic is a database migrations tool written by the author of  [SQLAlchemy](http://www.sqlalchemy.org/). A migrations tool offers the following functionality:

 1. Can emit ALTER statements to a database in order to change the structure of tables and other constructs
 2. Provides a system whereby “migration scripts” may be constructed; each script indicates a particular series of steps that can “upgrade” a target database to a new version, and optionally a series of steps that can “downgrade” similarly, doing the same steps in reverse.
 3. Allows the scripts to execute in some sequential manner.

- [Homepage](https://alembic.sqlalchemy.org/)
- [Documentation](https://alembic.sqlalchemy.org/en/latest/)
- [Getting started](https://alembic.sqlalchemy.org/en/latest/tutorial.html) - Setting up alembic connection, running migrations, downgrading 
- [Auto-generate migrations](https://alembic.sqlalchemy.org/en/latest/autogenerate.html) - Alembic can view the status of the database and compare against the table metadata in the application, generating the “obvious” migrations based on a comparison.
- [Batch migratoins](https://alembic.sqlalchemy.org/en/latest/batch.html) - Runnign batch migrations
- [Working with branches](https://alembic.sqlalchemy.org/en/latest/branches.html) - merging two divergent source trees
-  [Alembic and Postgresql/](https://www.compose.com/articles/schema-migrations-with-alembic-python-and-postgresql/) - Running simple migrations on postgres using alembic.

<a name="tools"></a>
## Tools

<a name="tools-jupyterlab"></a>
#### JupyterLab
JupyterLab is the next-generation web-based user interface for Project Jupyter.

JupyterLab enables you to work with documents and activities such as [Jupyter notebooks](https://jupyterlab.readthedocs.io/en/latest/user/notebook.html#notebook), text editors, terminals, and custom components in a flexible, integrated, and extensible manner. You can[arrange](https://jupyterlab.readthedocs.io/en/latest/user/interface.html#interface) multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing.

* [Installation.html](https://jupyterlab.readthedocs.io/en/latest/getting_started/installation.html)
* [Documentation](https://jupyterlab.readthedocs.io/en/latest/index.html)
* [GitHub Repo](https://github.com/jupyterlab/jupyterlab)
* [Using Jupyter Notebook](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook) - explains how to install, run, and use Jupyter Notebooks for data science, including tips, best practices, and examples.
* [Jupyter notebook tips, tricks & shortcuts](https://www.dataquest.io/blog/jupyter-notebook-tips-tricks-shortcuts/) - keyboard shortcuts, IPython magic commands.
* [JupyterLab evolution of the jupyter notebook](https://towardsdatascience.com/jupyter-lab-evolution-of-the-jupyter-notebook-5297cacde6b) - An overview of JupyterLab, the next generation of the Jupyter Notebook.
* [Using notebook inside JupyterLab](https://jupyterlab.readthedocs.io/en/latest/user/notebook.html) - Using calssic jupyter notebooks inside jupyter lab.
* [Running PySpark in Jupyter notebook](https://blog.sicara.com/get-started-pyspark-jupyter-guide-tutorial-ae2fe84f594f) - PySpark installation, connection pyspark to notebook

<a name="tools-colab"></a>
#### Google Colab
Colaboratory is a free Jupyter notebook environment that requires no setup and runs entirely in the cloud.

With Colaboratory you can write and execute code, save and share your analyses, and access powerful computing resources, all for free from your browser.

* [Basic Features](https://colab.research.google.com/notebooks/basic_features_overview.ipynb)
* [Importing Libraries](https://colab.research.google.com/notebooks/snippets/importing_libraries.ipynb)
* [More resources](https://colab.research.google.com/notebooks/welcome.ipynb)
* [GPU Notebooks](https://colab.research.google.com/notebooks/gpu.ipynb)
* [Getting started](https://towardsdatascience.com/getting-started-with-google-colab-f2fff97f594c) -  a small dive into basic features
* [Running PySpark in colab](https://towardsdatascience.com/pyspark-in-google-colab-6821c2faf41c) - How to run Apache spark python api in google colab.
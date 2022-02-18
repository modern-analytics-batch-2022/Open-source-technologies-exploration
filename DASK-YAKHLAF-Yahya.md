![dask_horizontal_white_no_pad_dark_bg](https://user-images.githubusercontent.com/98273912/154573224-02aaf15a-494a-4923-990e-128d4c0b5c14.png)

# DASK (Dask natively scales Python)


## Brief description  

![Capture d’écran 2022-02-16 173549](https://user-images.githubusercontent.com/98273912/154596700-4a0bdc4e-5363-40e0-8dfb-42455889f817.png)


Dask is a flexible library for parallel computing in Python.

Dask is a framework to build distributed applications that has since been used with dozens of other systems like XGBoost, PyTorch, Prefect, Airflow, RAPIDS, and more. It’s a full distributed computing toolbox that fits comfortably in our hands.

Dask is composed of two parts:

1. Dynamic task scheduling optimized for computation. This is similar to Airflow, Luigi, Celery, or Make, but optimized for interactive computational workloads.

2. “Big Data” collections like parallel arrays, dataframes, and lists that extend common interfaces like NumPy, Pandas, or Python iterators to larger-than-memory or distributed environments. These parallel collections run on top of dynamic task schedulers.

## General information
* Creation year :

### initial release : 2015.01.08 / January 8, 2015

### stable release : 2021.09.01 / September 1, 2021

* Website : https://dask.org/

* dask documentation : https://docs.dask.org/en/latest/

* Github repository : https://github.com/dask/dask

* Community channel : https://docs.dask.org/en/latest/support.html

* Founders :  

 Dask is an open source library for parallel computing written in Python. Originally developed by Matthew Rocklin
 
 ![matthew-rocklin](https://user-images.githubusercontent.com/98273912/154576946-6d414b93-67e9-46b1-8f24-2729f4495503.png)
   
## Main capabilities  
Dask emphasizes the following virtues:

* Familiar: Provides parallelized NumPy array and Pandas DataFrame objects

* Flexible: Provides a task scheduling interface for more custom workloads and integration with other projects.

* Native: Enables distributed computing in pure Python with access to the PyData stack.

* Fast: Operates with low overhead, low latency, and minimal serialization necessary for fast numerical algorithms

* Scales up: Runs resiliently on clusters with 1000s of cores

* Scales down: Trivial to set up and run on a laptop in a single process

* Responsive: Designed with interactive computing in mind, it provides rapid feedback and diagnostics to aid humans



## Available connectors / integrations  

* These software projects are well-integrated with Dask, or use Dask to power components of their infrastructure.

![Capture d’écran 2022-02-18 012912](https://user-images.githubusercontent.com/98273912/154594562-a0daff61-935c-446b-8a5f-37b5888bd56e.png)

![Capture d’écran 2022-02-18 013312](https://user-images.githubusercontent.com/98273912/154594955-993cba99-ae7e-4154-9270-eb5fe00dc41c.png)

![Capture d’écran 2022-02-18 013804](https://user-images.githubusercontent.com/98273912/154595425-a3c4c02d-8b30-4f27-ae5c-0c0a42ce4a3e.png)

![Capture d’écran 2022-02-18 013911](https://user-images.githubusercontent.com/98273912/154595480-354181f8-aa56-48c8-abf1-7c3fbd56e5d6.png)


## Ways to deploy it :

* Cloud

There are a variety of ways to deploy Dask on cloud providers. Cloud providers provide managed services, like VMs, Kubernetes, Yarn, or custom APIs with which Dask can connect easily. You may want to consider the following options:

1. A managed Kubernetes service and Dask’s Kubernetes integration.

2. A managed Yarn service, like Amazon EMR or Google Cloud DataProc and Dask-Yarn.

Specific documentation for the popular Amazon EMR service can be found here

3. Directly launching cloud resources such as VMs or containers via a cluster manager with Dask Cloud Provider

* Data Access

You may want to install additional libraries in your Jupyter and worker images to access the object stores of each cloud:

1. s3fs for Amazon’s S3

2. gcsfs for Google’s GCS

3. adlfs for Microsoft’s ADL

* Historical Libraries

Dask previously maintained libraries for deploying Dask on Amazon’s EC2 and Google GKE. Due to sporadic interest, and churn both within the Dask library and EC2 itself, these were not well maintained. They have since been deprecated in favor of the Kubernetes and Helm solution.


## Reviews
* Good reviews  

Dask is lighter weight and is easier to integrate into existing code and hardware. If your problems vary beyond typical ETL + SQL and you want to add flexible parallelism to existing solutions, then Dask may be a good fit, especially if you are already using Python and associated libraries like NumPy and Pandas.

* Bad reviews   

1. The central scheduler spends a few hundred microseconds on every task. For optimal performance, task durations should be greater than 10-100ms.

2. Dask can not parallelize within individual tasks. Individual tasks should be a comfortable size so as not to overwhelm any particular worker.

3. Dask assigns tasks to workers heuristically. It usually makes the right decision, but non-optimal situations do occur.

4. The workers are just Python processes, and inherit all capabilities and limitations of Python. They do not bound or limit themselves in any way. In production you may wish to run dask-workers within containers.


## Roadmap  

![Capture d’écran 2022-02-18 015255](https://user-images.githubusercontent.com/98273912/154596642-12fcb178-676e-4611-b8b8-fe0bddae58fa.png)

## references

* http://distributed.dask.org/en/stable
* https://docs.dask.org/en/stable/
* https://dask.org/



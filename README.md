# Scraping Craigslist Housing


https://github.com/angelicadietzel/scraping-craigslist-housing

https://betterprogramming.pub/the-only-step-by-step-guide-youll-need-to-build-a-web-scraper-with-python-e79066bd895a

## Table of Contents
* [Objective](#objective)
* [Technologies](#technologies)
* [Data Sets](#data-sets)

## Objective
The purpose of this project is to teach you how to scrape housing data from Craigslist.

## Technologies
- Jupyter Notebook
- pandas
- NumPy
- Python
- BeautifulSoup

## Data Sets
- A [data set](https://github.com/angelicadietzel/scraping-craigslist-housing/blob/main/scraping_craigslist_housing/phx_apts.csv) containing the data that I scraped from Phoenix area housing posts on Craigslist. 

## Installing Beautiful Soup

https://www.crummy.com/software/BeautifulSoup/bs4/doc/#installing-beautiful-soup

```java
sudo apt-get update -y

sudo apt-get install python3-bs4

sudo pip install numpy

sudo pip install pandas

sudo apt-get install -y ipython3

```


## Installing Python Dependencies locally in project

https://stackoverflow.com/questions/53925660/installing-python-dependencies-locally-in-project

The recommended way to do this is by using a virtual environment. You can install virtualenv via pip with

```java
pip install virtualenv
```

Then create a virtual environment in your project directory:

```java
python3 -m venv env # previously: `virtualenv env`
```

Which will create a directory called env (you can call it anything you like though) which will mirror your global python installation. Inside env/ there will be a directory called lib which will contain Python and will store your dependencies.

Then activate the environment with:

```java
source env/bin/activate
```

Then install your dependencies with pip and they will be installed in the virtual environment env/:

```java
pip install -r requirements.txt
```

Then any time you return to the project, run source env/bin/activate again so that the dependencies can be found.

When you deploy your program, if the deployed environment is a physical server, or a virtual machine, you can follow the same process on the production machine. If the deployment environment is one of a few serverless environments (e.g. GCP App Engine), supplying a requirements.txt file will be sufficient. For some other serverless environments (e.g. AWS Lambda) the dependencies will need to be included in the root directory of the project. In that case, you should use 

```java
pip install -r requirements.txt -t ./.
```


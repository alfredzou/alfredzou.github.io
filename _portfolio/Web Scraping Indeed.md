---
title: "Web Scraping Indeed"
excerpt: "Web scraper to extract job title, salary, company, location, employment type and description from data related jobs on Indeed.<br/><img src='/user_images/indeed_logo.png' width='500px'>"
collection: portfolio
---

### Links
* Find the code [here](https://github.com/alfredzou/Web-Scraping-Indeed)

### Aim
Data is an emerging field that has been gaining popularity due to a few main factors, in my opinion: firstly the amount of data in the eco system has been greatly increased by the advent of the internet; second, the advancements in computing power has made data easier to process, especially making machine learning through deep neural networks feasible; finally, companies have realised the power of data for data analytics, or machine learning through data science.

Due to the relatively new nature of the data field, data job positions haven't been concretely defined. To me there are a few stand out divisions. Namely `data engineer`, `data analyst`, `data scientist` and `business analyst`. To test this theory, I want to scrape these roles from Indeed and try see if I can differentiate them based on requirements.

To achieve this, I will use logistic regression on the scraped descriptions to predict the associated job title. After using feature selection, I will be able to determine the respective role responsibilities.

### Web scraping introduction
Websites are constructed with 3 main components: html, which contains the content of the website; css, which contains the styling of the website; and javascript, which contains elements that update themselves without refreshing the page or can be interacted with like a drop-down menu.

Scraping involves using two tools: the crawler that navigates around the website to extract the page's html; and the parser that locates the html tag within the page's html to extract the relevant information. In this case we are trying to scrape the job title, salary, location, job type and description of data related job adverts.

Below is an example of some html. Notice how URLs and the text are wrapped around <a> and </a> tags. Say we wanted to extract the URLs of the search engines; we could use the `search_engine` class attribute to differentiate it from the wikipedia link. The parser uses tags and attributes to locate the necessary information to scrape.

```html
<a class="information" href="https://en.wikipedia.org/">Wikipedia</a>
<a class="search_engine" href="https://www.google.com/">Google</a>
<a class="search_engine" href="https://www.bing.com/">Bing</a>
```

From this process, you can see how each web scraper must be custom built for the website and can break easily if the website's html is changed. Essentially, we are at the mercies of the web developers.

### Developing a robust web scraper
I initially used Selenium as a crawler. Selenium creates a chrome browser than can be controlled through Python code. The main advantage of Selenium is that you can watch it crawl through the website, and it can handle javascript. Although this is fun to watch, Selenium is extremely slow, and prone to failure with javascript. An extremely common error I encountered with Selenium and javascript was being unable to locate an element. You can imagine how frustrating this would be, as the whole scraping process would both be unreliable and would need to be rerun. 

The lesson I've learned is to build a **robust** web scraper by reducing unnecessary complexity and improving visibility during the scraping. This means avoiding javascript if possible and printing out the data being extracted. 

I ended up using requests.get as the crawler, and XPath as the parser.

Here is my web scraper in action:

<img src='/user_images/Web Scraping Indeed.gif'>

### Determining Role Requirements
The next step is to use the scraped job descriptions to predict the job title as either a `data engineer`, `data analyst`, `data scientist` or `business analyst`. The job descriptions need to be preprocessed via count vectorisation. Count vectorisation involves breaking down each description into words and then counting how many times a specific unique word appears in that description. So if `python` appeared twice in a job advertisement, it would have a value of 2.

If `python` appeared more frequently in `data scientist` adverts than `business analyst` adverts, we could easily infer that `python` is an important role requirement for `data scientists` but not `business analysts`. Likewise, we can repeat that for other role requirements such as `tableau`, `sql`, `reporting`, etc.

To determine this information, we will look at the feature importance for determining each job title from a logistic regression model.

### Results

The initial results from the logistic regression have a lot of noise:

<img src='/user_images/noise.JPG'>

This can also be seen in an example job advertisement, where only a few parts of the advertisement are actually relevant:

<img src='/user_images/job advert.JPG'>

By manually selecting features from my knowledge of data role requirements, we can compare the role requirements between jobs:

<img src='/user_images/data engineer.JPG'>

As expected, data engineers require a skill set focused on databases and cloud computing with Google Cloud Platform, AWS or Azure.

<img src='/user_images/data analyst.JPG'>

Data analysts have a focus on reporting and creating visualisations. 

<img src='/user_images/data scientist.JPG'>

Data scientists have a focus on python and machine learning.

<img src='/user_images/business analyst.JPG'>

Business analysts have a similar skill set to data analysts. From my understanding business analysts are more management facing with a focus on business intelligence or company direction, while data analysts are more technical with a focus on deriving insights from data. My findings seem to confirm this.

### Limitations and Opportunities
There are multiple limitations involved with this analysis:
* I am using only data from Indeed about data jobs in Australia
* Small data source makes it hard to confirm the viability the model
* I have assumed there are only 4 main types of data jobs, there could be more such as data steward. This hypothesis could be tested using a clustering analysis
* The analysis does not determine the true skills required for the job, but the skills asked for by advertisements. This is especially true as advertisements are written by HR and not data professionals, who may not know the true role requirements. A solution could be surveying data professionals and/or conducting an analysis on data professionals on LinkedIn
* Job descriptions could be cleaned to only include relevant skill sets before count vectorisation
* Words such as `reporting` can be ambiguous depending on context. It could mean `reporting to` or `reporting` by itself. This might be solvable using lemmatisation 


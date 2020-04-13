---
title: "COVID-19 Dashboard"
excerpt: "Visualise the spread of COVID-19 and compare the responses between countries<br/><img src='/user_images/COVID-19 map.jpg' width='300px'>"
collection: portfolio
---

### Links
* View the dashboard [here](https://public.tableau.com/profile/alfred.zou#!/vizhome/COVID-19_15852011851070/COVID-19)
* Find the code [here](https://github.com/alfredzou/COVID-19-Dashboard)

### Introduction
Amidst a global pandemic, I wanted to create a Tableau dashboard to help visualise and compare the COVID-19 responses between countries. Specifically, I wanted to recreate the 

### Disclaimer
I am not an epidemiologist or a doctor. Please take my findings with a grain of salt and only follow medical advice from [NSW Health](https://www.health.nsw.gov.au/Infectious/diseases/Pages/coronavirus.aspx).

### General Findings
#### Act Early
At the start of the COVID-19 pandemic, there was a lot of wishful thinking that the virus would be contained in China and would not spread to the rest of the world. Governments were placed into a difficult situation on whether or not to enforce preventative policies at the risk of massive economic damage. Early actions implemented by governments are often met by questions of overreaction. The problem is that pandemics are not an immediate or a visible threat. Psychologically this doesn't feel real to us, unless we are personally affected. Personally, COVID-19 only started to feel real when General Assembly's Sydney campus was closed and moved to online lessons. To make this invisible threat visible, it important for governments to test for COVID-19. When there is a 



On a psychological 


#### Number of True Cases
The Johns Hopkins University's GitHub Repo reports the number of confirmed COVID-19 cases in each country. However, one must keep in mind that there is a big difference between confirmed and true cases. Firstly, I want to stress that its impossible to accurately determine the number of true cases. No medical test can provide a 100% accurate prediction. COVID-19 test kits may have around a 30% false negative rate, this means 30% of the time people test negative despite having COVID-19. One COVID-19 test kit involves taking a nasal and throat swab for COVID-19 pathogens. If 

E




<img src='/user_images/COVID-19 map blog post.JPG'>

#### Flattern the Curve




* There are two possible types of pandemics: a tall one and a short one. 
* There is also a horizontal line representing the total hospital capacity
* Flattening the curve means taking preventative measures to slow down the spread
* These could be government policies such as testing and lockdowns 
* Or hand washing, social distancing, remote work and reducing unnecessary trips
* Essentially squishing the tall curve below the hospital capacity line, relieving pressure off our medical system

<img src="/user_images/COVID-19.png"/>

Approximately 5% of COVID-19 cases are critical and require treatment in an ICU ward with a ventilator.

<img src="/user_images/Severe.png"/>





### Good sources to learn more about COVID-19
* [Our World in Data](https://ourworldindata.org/coronavirus)
* [Coronavirus: Why You Must Act Now by Tomas Pueyo](https://medium.com/@tomaspueyo/coronavirus-act-today-or-people-will-die-f4d3d9cd99ca)
* [The Science Paper That Has Changed US and UK Covid-19 Policy by Noel Plum](https://www.youtube.com/watch?v=JbQ3oLvvecM)
* [How To Tell If We're Beating COVID-19 by Minute Physics](https://www.youtube.com/watch?v=54XLXg4fYsc)
* [The Coronavirus Explained & What You Should Do by Kurzgesagt](https://www.youtube.com/watch?v=BtN-goy9VOY)
* [Estimating actual COVID 19 cases (novel corona virus infections) in an area based on deaths by Khan Academy](https://www.youtube.com/watch?v=mCa0JXEwDEk)
* [Even if you test negative for COVID-19, assume you have it, experts say](https://www.livescience.com/covid19-coronavirus-tests-false-negatives.html)
* [How Coronavirus Test Kits Work | WSJ](https://www.youtube.com/watch?v=tgyzdgf66eM)
* [Taiwan has only 77 coronavirus cases. Its response to the crisis shows that swift action and widespread healthcare can prevent an outbreak.](https://www.businessinsider.com.au/coronavirus-taiwan-case-study-rapid-response-containment-2020-3?r=US&IR=T)

### Data Sources
* Data on coronavirus cases from Johns Hopkins University's [githup repo](https://github.com/CSSEGISandData)
* Population estimates from [worldometers](https://www.worldometers.info/world-population/population-by-country/)
* US ICU beds estimate from [AHA 2015 Annual Survey](https://www.sccm.org/Communications/Critical-Care-Statistics)
* Mexico ICU beds estimate from [apnews](https://apnews.com/ff99a460e304ffc67ab03d8a57b2e1ef)
* Australia and NZ ICU beds estimate from [ANZICS 2018 report](https://www.anzics.com.au/wp-content/uploads/2019/10/2018-ANZICS-CORE-Report.pdf)
* ICU beds estimate from 2012 academic paper ['The variability of critical care bed numbers in Europe'](https://link.springer.com/article/10.1007/s00134-012-2627-) by Rhodes et al. 8/tables/2
* ICU beds estimate from 2020 academic paper ['Critical Care Bed Capacity in Asian Countries and Regions'](https://www.researchgate.net/figure/Number-of-Critical-Care-Beds_tbl1_338520008) by Phua et al.
* % Populations over 65 per country (2019) from [worldbank](https://data.worldbank.org/indicator/SP.POP.65UP.TO.ZS)
* Number of Doctors and Nurses per 10,000 people per country from 2015 [WHO's World Health Stasticis report]( https://apps.who.int/iris/bitstream/handle/10665/170250/9789240694439_eng.pdf;jsessionid=FC99DC52822E45FBA833E47587CB567E?sequence=1)
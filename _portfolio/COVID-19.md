---
title: "COVID-19 Dashboard"
excerpt: "Visualise the spread of COVID-19 and compare the responses between countries<br/><img src='/user_images/COVID-19 map.jpg' width='300px'>"
collection: portfolio
---

### Links
* View the dashboard [here](https://public.tableau.com/profile/alfred.zou#!/vizhome/COVID-19_15852011851070/COVID-19)
* Find the code [here](https://github.com/alfredzou/COVID-19-Dashboard)

### Introduction
Amidst the COVID-19 global pandemic, I wanted to create a Tableau dashboard to help visualise and compare the responses between countries. Specifically, I wanted to recreate the popular **flatten the curve** image for each country, but with actual data.

<img src="/user_images/COVID-19.png"/>

### Disclaimer
I am not an epidemiologist or a doctor. Please take my thoughts with a grain of salt and only follow medical advice from [your local health authority, NSW Health in my case](https://www.health.nsw.gov.au/Infectious/diseases/Pages/coronavirus.aspx). There is a lot of panic and misinformation out there, so I encourage a healthy amount of skepticism.

### General Findings
#### Act Early
At the start of the COVID-19 pandemic, there was a lot of wishful thinking that the virus would be contained within China and would not spread to the rest of the world. Governments were placed into a difficult situation on whether or not to enforce preventative policies at the risk of massive economic damage. Early actions implemented by governments were first perceived by the general public as both a nuisance and an overreaction. After the number of cases grew, governments were then blamed for taking actions too slowly.

The problem with pandemics is that they are not an immediate or a visible threat, especially when compared to natural disasters like bushfires, earthquakes, etc. Psychologically this doesn't feel real to us, unless we become personally affected. To make this invisible threat visible, it's important for governments to implement screening at airports and testing for COVID-19. Only when there is transparency on the severity of the issue, will the public start taking the 'invisible' threat seriously and start cooperating socially. The issue lies with governments that have failed to test and have down played the threat of COVID-19.

The second issue with pandemics is that their rate of spread is based on the number of infected people, which causes exponential growth. Exponential growth isn't very intuitive, which is explained very well in this [video by It's Ok To Be Smart](https://www.youtube.com/watch?v=fgBla7RepXU&feature=youtu.be&t=132). Hence, if their spread isn't kept in check during the early stages, their explosive growth can often surprise us and our governments.

Lastly, there is a significant lag time between the implementation of government policies and its effects. If the incubation period of COVID-19 is between 1-14 days, it can take up to two weeks before we see any significant effects from government policies. This suggests that proactive actions are more effective than reactive actions. Tomas Pueyo's analysis of COVID-19 cases in Wuhan is a good representation of this.

<img src='/user_images/hubei lockdown.JPG'>

#### Number of True Cases
The Johns Hopkins University's COVID-19 GitHub repository reports the number of confirmed COVID-19 cases in each country. However, one must keep in mind that there is a big difference between confirmed and true cases. 

Firstly, I want to stress that its impossible to accurately determine the number of true cases. No medical test can provide a 100% accurate prediction. The most common COVID-19 testing kits are PCR tests that involve taking nasal and throat swabs for COVID-19 pathogens. [COVID-19 test kits may have around a 30% false negative rate](https://www.livescience.com/covid19-coronavirus-tests-false-negatives.html), this means 30% of the time people test negative despite having COVID-19. [Reasons for this include](https://youtu.be/tgyzdgf66eM?t=114) testing too early and not capturing enough pathogens on the swab; and degradation of pathogens during transport. Therefore even if you test negative, you'll still be advised to stay home and self isolate. So essentially, there is an inherent measurement error with the testing kits. Even if we test every single person, its impossible to determine the true number of cases.

Secondly, countries being unable to test due to resource limitations or failing to test, will also hide the true number of cases. Countries with large populations with low amount of tests performed or countries with high mortality rates suggest that true cases are much larger than confirmed cases. The most comprehensive collection of testing data I have found is from [Our World In Data](https://ourworldindata.org/covid-testing).

<img src="/user_images/COVID-19 map blog post.JPG"/>

Additionally, not all asymptomatic or mild carriers will be tested and could recover by themselves.

<img src="/user_images/critical.png"/>

In conclusion, the true cases of COVID-19 are underestimated and probably much larger than the confirmed cases.

#### Flatten the Curve
The popular flatten the curve illustration shows two types of pandemics: the first type of pandemic is a sharp and concentrated curve, where no government policies or preventative measures are taken; the second type of pandemic is distributed over a long period of time, so it stays below the horizontal dashed line. The horizontal dashed line is a representation of a country's medical capacity. The aim of 'flatten the curve' is to reduce the strain on the medical system, which will in return prevent deaths.

<img src="/user_images/COVID-19.png"/>

 Approximately 5% of COVID-19 cases are critical and require treatment in an intensive care unit (ICU) ward with a ventilator. However, each country only has a limited amount of ICU beds. Australia has about 93,000 hospital beds but only around 2229 ICU beds (2.4%). In most countries 1-3% of total hospital beds are ICU beds. To make matters worse, the average occupancy rate for ICU beds is around 75%. 
 
 In my dashboard, I have modelled the number of critical active cases for each country against its medical capacity, represented by available ICU beds.

<img src="/user_images/critical.png"/>

### The Future
I hope I've convinced you of the gravity of the current situation. Everyone needs to do their part to help contain the spread of COVID-19 through hand washing, social distancing, remote work and reducing unnecessary trips. I want to encourage everyone that staying at home and self isolating is necessary in reducing the impact of COVID-19.

Unfortunately, I don't think there will be a light at the end of the tunnel until a vaccine has been developed. I'm also expecting the relaxation of government polices and reduction of new cases may trigger social complacency and future outbreaks.

### Good sources to learn more about COVID-19
* [Our World in Data](https://ourworldindata.org/coronavirus)
* [Coronavirus: Why You Must Act Now by Tomas Pueyo](https://medium.com/@tomaspueyo/coronavirus-act-today-or-people-will-die-f4d3d9cd99ca)
* [The Science Paper That Has Changed US and UK Covid-19 Policy by Noel Plum](https://www.youtube.com/watch?v=JbQ3oLvvecM)
* [How To Tell If We're Beating COVID-19 by Minute Physics](https://www.youtube.com/watch?v=54XLXg4fYsc)
* [The Coronavirus Explained & What You Should Do by Kurzgesagt](https://www.youtube.com/watch?v=BtN-goy9VOY)
* [Estimating actual COVID 19 cases (novel corona virus infections) in an area based on deaths by Khan Academy](https://www.youtube.com/watch?v=mCa0JXEwDEk)
* [Even if you test negative for COVID-19, assume you have it, experts say](https://www.livescience.com/covid19-coronavirus-tests-false-negatives.html)
* [How Coronavirus Test Kits Work WSJ](https://www.youtube.com/watch?v=tgyzdgf66eM)
* [Taiwan has only 77 coronavirus cases. Its response to the crisis shows that swift action and widespread healthcare can prevent an outbreak.](https://www.businessinsider.com.au/coronavirus-taiwan-case-study-rapid-response-containment-2020-3?r=US&IR=T)
* [What This Chart Actually Means for COVID-19](https://www.youtube.com/watch?v=fgBla7RepXU)

### Data Sources
* Data on coronavirus cases from Johns Hopkins University's [githup repo](https://github.com/CSSEGISandData)
* Population estimates from [worldometers](https://www.worldometers.info/world-population/population-by-country/)
* US ICU beds estimate from [AHA 2015 Annual Survey](https://www.sccm.org/Communications/Critical-Care-Statistics)
* Mexico ICU beds estimate from [apnews](https://apnews.com/ff99a460e304ffc67ab03d8a57b2e1ef)
* Australia and NZ ICU beds estimate from [ANZICS 2018 report](https://www.anzics.com.au/wp-content/uploads/2019/10/2018-ANZICS-CORE-Report.pdf)
* ICU beds estimate from 2012 academic paper ['The variability of critical care bed numbers in Europe'](https://link.springer.com/article/10.1007/s00134-012-2627-8/tables/2) by Rhodes et al. 
* ICU beds estimate from 2020 academic paper ['Critical Care Bed Capacity in Asian Countries and Regions'](https://www.researchgate.net/figure/Number-of-Critical-Care-Beds_tbl1_338520008) by Phua et al.
* % Populations over 65 per country (2019) from [worldbank](https://data.worldbank.org/indicator/SP.POP.65UP.TO.ZS)
* Number of Doctors and Nurses per 10,000 people per country from 2015 [WHO's World Health Stasticis report]( https://apps.who.int/iris/bitstream/handle/10665/170250/9789240694439_eng.pdf;jsessionid=FC99DC52822E45FBA833E47587CB567E?sequence=1)
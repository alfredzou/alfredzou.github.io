---
title: "COVID-19 Dashboard"
excerpt: "Visualise the spread of COVID-19 and compare the responses between countries<br/><img src='/user_images/COVID-19 map.jpg' width='500px'>"
collection: portfolio
---

### Links
* View the dashboard [here](https://public.tableau.com/profile/alfred.zou#!/vizhome/COVID-19_15852011851070/COVID-19)
* Find the code [here](https://github.com/alfredzou/COVID-19-Dashboard)

### Introduction
Amidst the COVID-19 global pandemic, I wanted to create a Tableau dashboard to help visualise and compare the responses between countries. Specifically, I wanted to recreate the popular **flatten the curve** image for each country, but with actual data. Below I have provide some social commentary on my thoughts regarding COVID-19.

<img src="/user_images/COVID-19.png"/>

### Disclaimer
I am not an epidemiologist or a doctor. Just someone curious about the whole situation. Please take my thoughts with a grain of salt and only follow medical advice from your local health authority, [NSW Health in my case](https://www.health.nsw.gov.au/Infectious/diseases/Pages/coronavirus.aspx). There is a lot of panic and misinformation out there, so I encourage a healthy amount of skepticism. [Sympathies to my 5G telco planning friends.](https://www.abc.net.au/news/science/2020-04-15/coronavirus-5g-vitamin-c-anti-vaccine-conspiracy-theories-spread/12145096)

### General Findings
#### Act Early
At the start of the COVID-19 pandemic, there was a lot of wishful thinking that the virus would be contained within China and would not spread to the rest of the world. Governments were placed into a difficult situation on whether or not to enforce preventative policies at the risk of massive economic damage. Early actions implemented by governments were first perceived by the general public as both a nuisance and an overreaction. However after the number of cases grew, governments were then blamed for taking actions too slowly. Why did the attitude towards government policies shift so quickly?

**The problem with pandemics is that they are invisible, which makes their severity hard to gauge, especially when compared to natural disasters like bushfires, earthquakes, etc.** A typical government response to a bushfire maybe to pump more money into fire fighting services and to deploy more fire fighters and trucks. If you watch the news and see fire fighters battling a bushfire, I think its very easy to support this government response. Especially when this response doesn't directly affect or require you to do anything. This is in contrast to pandemics, where at the core of the solution is policies on social behaviour. This directly affects every person, by limiting their freedom of movement, and requires their cooperation. For governments to justify its policies and convince the public to cooperate, they need to make this invisible threat visible. Great ways to achieve this include mass testing for COVID-19, screening at airports and contact tracing. Only when there is transparency on the severity of the issue, for example the number of cases and deaths, will the public start taking this 'invisible' threat seriously and start cooperating socially. If you see only 5 cases in your state, you might carry on as normal; if there are 100 cases, you might become more cautious and begin reducing social contact. The issue lies with governments that have failed to test and have down played the threat of COVID-19, which leads to both a false sense of security and social complacency. 

Countries like the US and [Brazil](https://www.latimes.com/world-nation/story/2020-04-09/brazils-president-refuses-to-admit-that-coronavirus-poses-a-real-threat-hes), who have down played the threat of COVID-19, are now facing the consequences of an explosive growth of cases and deaths.

Where as [Taiwan's speedy response and testing](https://www.businessinsider.com.au/coronavirus-taiwan-case-study-rapid-response-containment-2020-3?r=US&IR=T) has become the gold standard for epidemic response.

**The second issue with pandemics is that their rate of spread is based on the number of infected people, which causes exponential growth.** [Exponential growth isn't very intuitive and can quickly swing from no one having the virus to everyone suddenly everyone having it.](https://www.youtube.com/watch?v=fgBla7RepXU&feature=youtu.be&t=132) If there is no visibility on the spread of COVID-19 and hence lack of preventative policies, the unchecked exponential growth will lead to dire consequences.

<img src="/user_images/exponential growth.gif"/>

Source: [What we can learn from the countries winning the coronavirus fight by ABC](https://www.abc.net.au/news/2020-03-26/coronavirus-covid19-global-spread-data-explained/12089028)

**Lastly, there is a significant lag time between the implementation of government policies and its effects.** If the incubation period of COVID-19 is between 1-14 days, it can take up to two weeks before we see any significant effects from government policies. If a country only begins taking action only after a high spike in cases or deaths, its a signal that their response has been too slow. This heavily suggests that proactive actions are much more effective than reactive actions. Tomas Pueyo's analysis of COVID-19 cases in Wuhan is a good representation of this.

<img src='/user_images/hubei lockdown.JPG'>

#### Number of True Cases
The Johns Hopkins University's COVID-19 GitHub repository reports the number of confirmed COVID-19 cases in each country. However, one must keep in mind that there is a big difference between confirmed and true cases. 

Firstly, I want to stress that its impossible to accurately determine the number of true cases. No medical test can provide a 100% accurate prediction. The most common COVID-19 testing kits are PCR tests that involve taking nasal and throat swabs for COVID-19 pathogens. [COVID-19 test kits may have around a 30% false negative rate](https://www.livescience.com/covid19-coronavirus-tests-false-negatives.html), this means 30% of the time people test negative despite having COVID-19. [Reasons for this include](https://youtu.be/tgyzdgf66eM?t=114) testing too early and not capturing enough pathogens on the swab; and degradation of pathogens during transport. Therefore even if you test negative, you'll still be advised to stay home and self isolate. **Regardless of test results, everyone should assume they have COVID-19 and act accordingly.** So essentially, there is an inherent measurement error with the testing kits. Even if we test every single person, its impossible to determine the true number of cases.

Secondly, countries being unable to test due to resource limitations or failing to test, will also hide the true number of cases. Countries with large populations with low amount of tests performed or countries with high mortality rates suggest that true cases are much larger than confirmed cases. The most comprehensive collection of testing data I have found is from [Our World In Data](https://ourworldindata.org/covid-testing).

South Korea, despite a large outbreak from a religious cult, has managed to contain the virus through an aggressive testing scheme.

The Japanese government has been heavily criticised for its lack of testing.

<img src="/user_images/testing.JPG"/>

Additionally, not all asymptomatic or mild carriers will be tested and could recover by themselves.

<img src="/user_images/critical.png" width="500px"/>

In conclusion, the true cases of COVID-19 are heavily underestimated and probably much larger than the confirmed cases.

#### Flatten the Curve
The popular flatten the curve illustration shows two types of pandemics: the first type of pandemic is a sharp and concentrated curve, where no government policies or preventative social measures are taken; the second type of pandemic is distributed over a long period of time, so it stays below the horizontal dashed line. The horizontal dashed line is a representation of a country's medical capacity. The aim of 'flatten the curve' is to reduce the strain on the medical system, which will in return prevent deaths.

<img src="/user_images/COVID-19.png" width="500px"/>

 Approximately 5% of COVID-19 cases are critical and require treatment in an intensive care unit (ICU) ward with a ventilator. However, each country only has a limited amount of ICU beds. Australia has about 93,000 hospital beds but only around 2229 ICU beds (2.4%). In most countries 1-3% of total hospital beds are ICU beds. To make matters worse, the normal average occupancy rate for ICU beds is around 75%. 
 
 In my dashboard, I have modelled the number of critical active cases for each country against its medical capacity, which I have represented by available ICU beds. This is an extremely simple model that doesn't take into account lots of factors like number of ventilators, nurses, doctors, etc. It also doesn't account for changing medical capacity from ICU surge capacity, production of new ventilators and medical staff needing to self isolate.

<img src="/user_images/Active and Severe Cases AU.JPG" width="500px"/>

There are catastrophic consequences when a country's medical capacity is overwhelmed.

<img src="/user_images/Active and Severe Cases US.JPG" width="500px"/>

### The Future
I hope I've conveyed the gravity of the current situation. Everyone needs to do their part to help contain the spread of COVID-19 through hand washing, social distancing, remote work and reducing unnecessary trips. I want to encourage everyone that staying at home and self isolating is extremely important and vital in slowing the spread of COVID-19. This in turns reduces the stress on medical systems and saves lives. My greatest appreciation to all the medical staff and anyone else combating COVID-19.

For everyone staying at home, please look after yourselves and especially your sanity. Thankfully in the digital age, we can still combat loneliness by keeping in touch with our friends and family. For someone who loves staying at home, even I'm starting to become a little bit crazy. I can only imagine how bad it is for people who love going outside. Instead of going out on the weekends, it's a great opportunity to start a new hobby or learn some new skills.

Unfortunately, I don't think there will be a light at the end of the tunnel until a vaccine has been developed. With uncertainties on how long a vaccine could take, 2020 could definitely be the year of remote work and staying at home. However, how realistic is it for countries to stay in lock down, both in an economic and mental health sense? Without a vaccine, maybe some sort of slow and controlled herd immunity approach may work. Countries have been considering some sort of [immunity passport](https://www.france24.com/en/20200416-grave-concerns-about-covid-19-immunity-passports) to let those with detected antibodies leave lock down earlier. However, there are concerns regarding their accuracy and how they may trigger social unrest between those who have and don't have the passport. There doesn't seem to be any obvious golden bullet solution. [Additionally, I'm afraid that social complacency and relaxation of government policies may trigger a 2nd wave of outbreaks.](https://www.abc.net.au/news/2020-04-03/coronavirus-data-modelling-covid19-stay-home/12114978)

### Good sources to learn more about COVID-19
* [What we can learn from the countries winning the coronavirus fight by ABC](https://www.abc.net.au/news/2020-03-26/coronavirus-covid19-global-spread-data-explained/12089028)
* [Our World in Data](https://ourworldindata.org/coronavirus)
* [Coronavirus: Why You Must Act Now by Tomas Pueyo](https://medium.com/@tomaspueyo/coronavirus-act-today-or-people-will-die-f4d3d9cd99ca)
* [The Science Paper That Has Changed US and UK Covid-19 Policy by Noel Plum](https://www.youtube.com/watch?v=JbQ3oLvvecM)
* [How To Tell If We're Beating COVID-19 by Minute Physics](https://www.youtube.com/watch?v=54XLXg4fYsc)
* [The Coronavirus Explained & What You Should Do by Kurzgesagt](https://www.youtube.com/watch?v=BtN-goy9VOY)
* [Estimating actual COVID 19 cases (novel corona virus infections) in an area based on deaths by Khan Academy](https://www.youtube.com/watch?v=mCa0JXEwDEk)
* [Even if you test negative for COVID-19, assume you have it, experts say](https://www.livescience.com/covid19-coronavirus-tests-false-negatives.html)
* [How Coronavirus Test Kits Work WSJ](https://www.youtube.com/watch?v=tgyzdgf66eM)
* [What This Chart Actually Means for COVID-19](https://www.youtube.com/watch?v=fgBla7RepXU)

### Data Sources
* Data on coronavirus cases from Johns Hopkins University's [GitHup repository](https://github.com/CSSEGISandData)
* Population estimates from [Worldometers.info](https://www.worldometers.info/world-population/population-by-country/)
* US ICU beds estimate from [AHA 2015 Annual Survey](https://www.sccm.org/Communications/Critical-Care-Statistics)
* Mexico ICU beds estimate from [Apnews](https://apnews.com/ff99a460e304ffc67ab03d8a57b2e1ef)
* Australia and NZ ICU beds estimate from [ANZICS 2018 report](https://www.anzics.com.au/wp-content/uploads/2019/10/2018-ANZICS-CORE-Report.pdf)
* ICU beds estimate from 2012 academic paper ['The variability of critical care bed numbers in Europe'](https://link.springer.com/article/10.1007/s00134-012-2627-8/tables/2) by Rhodes et al. 
* ICU beds estimate from 2020 academic paper ['Critical Care Bed Capacity in Asian Countries and Regions'](https://www.researchgate.net/figure/Number-of-Critical-Care-Beds_tbl1_338520008) by Phua et al.
* % Populations over 65 per country (2019) from [Worldbank.org](https://data.worldbank.org/indicator/SP.POP.65UP.TO.ZS)
* Number of Doctors and Nurses per 10,000 people per country from 2015 [WHO's World Health Statistics report](https://apps.who.int/iris/bitstream/handle/10665/170250/9789240694439_eng.pdf;jsessionid=FC99DC52822E45FBA833E47587CB567E?sequence=1)
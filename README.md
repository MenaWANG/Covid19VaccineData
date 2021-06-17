# Covid-19 Vaccine Data

This repository shares the data wrangling process for a project on Covid-19 vaccines effectiveness. The purpose of the project is **to investigate the effects of vaccines on two key aspects of the pandemic**:  

* a) slowing down the **spread** and 
* b) reducing the **severity of illness** from Covid-19

The analysis was done using the **many-models approach**, where the same model was estimated among each entity then summarized to gain a comprehensive picture of vaccine effectiveness worldwide. 

**The full report is too big for GitHub to host. You can find it [here](https://rpubs.com/MenaWANG/COVID19Vaccines), or explore it through this [interactive dashboard](https://rstudioconnect-online.monash.edu/connect/#/apps/287/access).** This repository share the code used to prepare the data. You can also download these prepared data files directly from the **Data folder**: 

1. **VacccineAllVariables.csv**: Dataset with imputed vaccine numbers, smoothed case and deaths numbers, and a comprehensive list of other relevant variables.
2. **Vaccine.RDS**: Dataset with only the key variables in RDS format, used when deploying [this Dashboard]((https://rstudioconnect-online.monash.edu/connect/#/apps/287/access)) to boost performance.
3. **Entity.RDS**: List of all entities in the original dataset, categorized as included vs not-included in the analysis depending on its population. The population threshold is now set as 100K (i.e., only entities with population larger than 100K are included). You can adjust the value in the following code chunk; and the above two data files will change accordingly.
4. **BasicInfo.RDS**: Document basic information about the data files, including the population bar, last updated date, etc. for reference.


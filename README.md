# Prediction of Monthly Carbon Emissions and Discussion on the Impact of Volcanic Eruptions on Carbon Concentration in the Atmosphere
## Project information
- **Author**: Eddie Lin, Computation and Design major Computer Science track, 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**:  Submissions to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2022 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks to Prof. Luyao Zhang for her precious suggestions and teachings that made this project possible, and many thanks goes out to my classmates from Stats 201 for the productive discussions in class to perfect my hypothesis. Special thanks to Yiyang Zhang for peer reviewing my report and providing meaningful and impactful comments.
- **Project Summary**: 
In 1985, a major volcanic eruption occured in Columbia, the Nevado Del Ruiz volcano erupted in November, devastating the city of Armero, killing more than 20,000 people(Schuster and Highland 2001). The annual release of Carbon Dioxide from Volcanic activitites is 0.28-0.36 gigatons(Collins 2019). It would be enlightening to see how much impact this number of carbon emission actually has on the global scale of carbon emissions. Because the Carbon concentration measured is in the global scale, a major volcanic eruption is preferred to be studied so that its effects may be more obvious than an average-sized eruption or minor volcanic activities. The Armero tragedy was one of the biggest volcanic eruptions in the recent decades that has data on carbon concentration, thus we select to study this particular eruption. The study will analyze monthly data of carbon concentration in the atmosphere from the past few decades. We will apply causal inference to the major volcanic eruption of Nevada Del Ruiz in 1945. In hopes of acquiring a deeper understanding of the relationship between the variable and the potential impact of volcanic eruptions 

## Table of Contents
| File | Content |
| :---         |:---|
| [Data](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/tree/main/data) | [Data](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/edit/main/README.md#data)|
| [Code](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/tree/main/code) | [Code](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/edit/main/README.md#code)|
| [Spotlight](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/tree/main/spotlight) |[Spotlight](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/edit/main/README.md#spotlight)|



## Data
### Meta Data Information
| Data Files| Data Content | Data Type|
| :---         |     :---     | :---: |
|co2_mm_mlo.csv| data of monthly global carbon emissions | Queried |
|Cited.csv | literatures collected for the explanation task of the problem set | Queried |
|Regression_Test.csv| Test data for regression task| Processed |
|Regression_Train.csv| Train data for regression task| Processed |

### Data Dictionary 
| File of Data| variable name | description | frequency     |  unit. |    type|
|:---| :---         |     :---     |   :---: |  :---:   | :---: |  
|   co2_mm_mlo.csv    |      average     |    monthly average of global carbon concentration in the atmosphere  |   monthly    |   parts per million    |    float64   |
|   co2_mm_mlo.csv    |      deseasonalized     |    monthly average of global carbon concentration in the atmosphere removing the possible interference of the current season |   monthly    |   parts per million    |    float64   |
|Cited.csv | title| title of each collected literature | \ | \ | String |
|Cited.csv | abstract| abstract of each collected literature | \ | \ | String |
|Regression_Test.csv| average|  monthly average of global carbon dioxide emissions | monthly | parts per million | float64|
|Regression_Test.csv| average_past|  average of global carbon dioxide emissions of the past month | monthly | parts per million | float64|
|Regression_Train.csv| average|  monthly average of global carbon dioxide emissions | monthly | parts per million | float64|
|Regression_Train.csv| average_past|  average of global carbon dioxide emissions of the past month | monthly | parts per million | float64|


## Code
- [Explanation Code](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/code/Explanation.ipynb)
- [Prediction Code](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/code/Prediction.ipynb)
- [Causal Inference Code](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/code/Causal_Inference.ipynb)
### Table of Code
| File| Description |
| :---         |     :---:     |
| Prediction.ipynb  | Code that carries out the prediction task |
| Explanation.ipynb | Code that carries out the explanation task |
| Causual Inference.ipynb | Code that carries out the causal inference task |


## Spotlight
![Poster](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/Poster%20updated.png)
*Figure 1. Project Poster*

![linear regression](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/linear%20regression.png)

*Figure 2.  histogram graph of true and predicted value generated by linear regression algorithm*
Description: Figure 2 compares the predicted data and true data using histograms to represent each set's value. We can see that the data overlaps quiet perfectly. The R2 score for the regressor is 0.9915539790301517. Because an R2 score being closer to 1 means the data is better fitted. We can see that the regressor is in high accuracy in predicting the future month's carbon emissions.

![wordcloud](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/wordcloud.png)
*Figure 3. wordcloud of high frequency words in research titles*
Description: Figure 3 shows the high frequency phrases used in NFT-related literatures. With the help of natural language processing, it is easy to spot that market, Ethereum, and networks are mentioned more than the other phrases, which can bring insight to research on which of the aspects of NFT is currently focused on.

![Causal Inference](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/Causal%20Inference.png)

*Figure 4. Regression Discontinuity applied to the monthly data of carbon concentration in the atmosphere
Description: From figure 4 we can see that the carbon concentration does not present sudden change after the cutoff event. In contrast, the actual Carbon dioxide concentration actually dropped below the hypothesized regression line if the cutoff event did not happen

## References

### Data Source
- Data Source Title and URL
### Code Source
- Code Source Title and URL
### Articles
- Article Source Title and URL
### Literature
- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```


# Prediction of Monthly Carbon Emissions and Discussion on the Impact of Volcanic Eruptions on Carbon Concentration in the Atmosphere
## Project information
- **Author**: Eddie Lin, Computation and Design major Computer Science track, 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**:  Submissions to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2022 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks to Prof. Luyao Zhang for her precious suggestions and teachings that made this project possible, and many thanks goes out to my classmates from Stats 201 for the productive discussions in class to perfect my hypothesis. Special thanks to Yiyang Zhang for peer reviewing my report and providing meaningful and impactful comments.
- **Project Summary**: 
The annual release of Carbon Dioxide from Volcanic activitites is 0.28-0.36 gigatons(Collins 2019). It would be enlightening to see how much impact this number of carbon emission actually has on the global scale of carbon emissions. Because the Carbon concentration measured is in the global scale, a major volcanic eruption is preferred to be studied so that its effects may be more obvious than an average-sized eruption or minor volcanic activities. In 1985, a major volcanic eruption occured in Columbia, the Nevado Del Ruiz volcano erupted in November, devastating the city of Armero, killing more than 20,000 people(Schuster and Highland 2001). The Armero tragedy was one of the biggest volcanic eruptions in the recent decades that has data on carbon concentration, thus we select to study this particular eruption. The study will analyze monthly data of carbon concentration in the atmosphere that ranges from 1958 to January 2023(Tans and Global Monitoring Laboratory, n.d.). We will apply causal inference, specifically the technique of regression discontinuity, to the major volcanic eruption of Nevada Del Ruiz in 1945. In hopes of acquiring a deeper understanding of the relationship between the variable and the potential impact of volcanic eruptions. The results were contrary to the hypothesis that the volcanic eruption will have an obvious, direct, positive impact on the concentration of carbon dioxide in the atmosphere. Instead, after applying regression discontinuity, the results show that the trend line still roughly follows the regression line of the data before the cutoff event, which implies the event was not as influencial to the Carbon concentration in the atmosphere as previously hypothesized. The practical impact of this research is meaningful in being used as a counterargument to influential climate change deniers. Said deniers have been purposefully use volcanic eruptions as the scapegoats for carbon emissions instead of human activities such as fossil fuel burning in many medias(Schmidt 2016). The findings of this research puts forward the fact that a volcanic eruption as major as the Armero tragedy does not lead to a change in the carbon concentration, meaning natural factors are significantly outweighed by human factors in producing carbon dioxide.


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
![Poster](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/poster.png)
*Figure 1. Project Poster*

![linear regression](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/linear%20regression.png)

*Figure 2.  histogram graph of true and predicted value generated by linear regression algorithm*

Description: Figure 2 compares the predicted data and true data using histograms to represent each set's value. We can see that the data overlaps quiet perfectly. The R2 score for the regressor is 0.9915539790301517. Because an R2 score being closer to 1 means the data is better fitted. We can see that the regressor is in high accuracy in predicting the future month's carbon emissions.

![wordcloud](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/wordcloud.png)
*Figure 3. wordcloud of high frequency words in research titles*

Description: Figure 3 shows the high frequency phrases used in NFT-related literatures. With the help of natural language processing, it is easy to spot that market, Ethereum, and networks are mentioned more than the other phrases, which can bring insight to research on which of the aspects of NFT is currently focused on.

![Causal Inference](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/figures/Causal%20Inference.png)

*Figure 4. Regression Discontinuity applied to the monthly data of carbon concentration in the atmosphere

Description: From figure 4 we can see that the carbon concentration does not present sudden change after the cutoff event. In contrast, the actual Carbon dioxide concentration actually dropped below the hypothesized regression line if the cutoff event did not happen*

## More About the Author
![headshot](https://github.com/Rising-Stars-by-Sunshine/stats201-Final-Project-Eddie/blob/main/spotlight/image.png)
### Introduction
Eddie Lin is currently a sophomore student in Duke Kunshan University studying under the Computation and Design major. He has experience in working in programming languages such a Python and Java, he has also learned about using Structured Query Language(SQL).

### Final Reflections
This course has taught me much about what machine learning can do in the social science fields. I learned to use prediction models, explanation models, and causal inference models to solve problems that I have encountered in this course. I also learned about the other capabilities of machine learning such as optimization and made attempts at implementing optimization to social science problems. This course was taught in an interdisciplinary way, where students who are experienced in social science but not that much in computer science can learn more about the capabilities of machine learning and actually implement algorithms to their research, and students who know computer science well but not social science can use their knowledges in machine learning to solve social science and economical issues. Personally, I benefited hugely from the way this course was taught as I can actually use my coding experience to take a shot in solving social science problems that I was interested in. 
In the professional research aspect, the course teaches us from the very basics, from creating our own github page, to formulating a research topic and goes on to finishing the research, being peer-reviewed, and responding to the peer review. The process of research is helpful for me in the future to proceed on my own research topics since I have already experienced much of the process of research in this class.
This course has inspired me to continue to use machine learning on societal, economical, and even environmental issues in the future!

## References

### Data Source
- [Global Monitoring Laboratory-Carbon Cycle Greenhouse Gases](https://gml.noaa.gov/webdata/ccgg/trends/co2/co2_mm_mlo.txt)
### Code Source
- [stats201-tutorial-prediction](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction/tree/main/code)
- [sunshineluyao/design-principle-blockchain](https://github.com/sunshineluyao/design-principle-blockchain/tree/main/code)

### Literature
- Ante, Lennart. 2021. “Non-Fungible Token (NFT) Markets on the Ethereum Blockchain: Temporal Development, Cointegration and Interrelations.” SSRN Electronic Journal. https://doi.org/10.2139/ssrn.3904683.
- Collins, Terry. 2019. “Scientists Quantify Global Volcanic CO2 Venting; Estimate Total Carbon on Earth.” EurekAlert! October 1, 2019. https://www.eurekalert.org/news-releases/736161.
- Das, Dipanjan, Priyanka Bose, Nicola Ruaro, Christopher Kruegel, and Giovanni Vigna. 2021. “Understanding Security Issues in the NFT Ecosystem.” ArXiv:2111.08893 [Cs], November. https://arxiv.org/abs/2111.08893.
- Fowler, Allan, and Johanna Pirker. 2021. “Tokenfication - the Potential of Non-Fungible Tokens (NFT) for Game Development.” Extended Abstracts of the 2021 Annual Symposium on Computer-Human Interaction in Play, October. https://doi.org/10.1145/3450337.3483501.
- Ghelani, Diptiben. 2022. “What Is Non-Fungible Token (NFT)? A Short Discussion about NFT Terms Used in NFT.” Authorea. October 4, 2022. https://www.authorea.com/doi/full/10.22541/au.166490992.24247550.
- Hwang, Yohan. 2023. “When Makers Meet the Metaverse: Effects of Creating NFT Metaverse Exhibition in Maker Education.” Computers & Education 194 (March): 104693. https://doi.org/10.1016/j.compedu.2022.104693.
- Kapoor, Arnav, Dipanwita Guhathakurta, Mehul Mathur, Rupanshu Yadav, Manish Gupta, and Ponnurungam Kumaraguru. 2022. “TweetBoost: Influence of Social Media on NFT Valuation.” ArXiv:2201.08373 [Cs], January. https://arxiv.org/abs/2201.08373.
- Mazur, Mieszko. 2021. “Non-Fungible Tokens (NFT). The Analysis of Risk and Return.” SSRN Electronic Journal. https://doi.org/10.2139/ssrn.3953535.
- Muthe, Koushik Bhargav, Khushboo Sharma, and Karthik Epperla Nagendra Sri. 2020. “A Blockchain Based Decentralized Computing and NFT Infrastructure for Game Networks.” 2020 Second International Conference on Blockchain Computing and Applications (BCCA), November. https://doi.org/10.1109/bcca50787.2020.9274085.
- Nadini, Matthieu, Laura Alessandretti, Flavio Di Giacinto, Mauro Martino, Luca Maria Aiello, and Andrea Baronchelli. 2021. “Mapping the NFT Revolution: Market Trends, Trade Networks, and Visual Features.” Scientific Reports 11 (1). https://doi.org/10.1038/s41598-021-00053-8.
- NASA. 2019. “What Do Volcanoes Have to Do with Climate Change? – Climate Change: Vital Signs of the Planet.” Climate Change: Vital Signs of the Planet. 2019. https://climate.nasa.gov/faq/42/what-do-volcanoes-have-to-do-with-climate-change/.
- Okonkwo, Ifeanyi E. 2021. “NFT, Copyright; and Intellectual Property Commercialisation.” SSRN Electronic Journal. https://doi.org/10.2139/ssrn.3856154.
- Oppenheimer, C., D. M. Pyle, and J. Barclay. 2003. Volcanic Degassing. Pubs.geoscienceworld.org. Geological Society of London. https://pubs.geoscienceworld.org/gsl/books/book/1592/Volcanic-Degassing.
- Park, Andrew, Jan Kietzmann, Leyland Pitt, Amir Dabirian, and Amir Dabirian. 2022. “The Evolution of Nonfungible Tokens: Complexity and Novelty of NFT Use-Cases.” IT Professional 24 (1): 9–14. https://doi.org/10.1109/mitp.2021.3136055.
- Pinto-Gutiérrez, Christian, Sandra Gaitán, Diego Jaramillo, and Simón Velasquez. 2022. “The NFT Hype: What Draws Attention to Non-Fungible Tokens?” Mathematics 10 (3): 335. https://doi.org/10.3390/math10030335.
- Popescu, Andrei-Dragos. 2021. “Non-Fungible Tokens (NFT) - Innovation beyond the Craze.” ResearchGate. unknown. August 18, 2021. https://www.researchgate.net/publication/353973149_Non-Fungible_Tokens_NFT_-_Innovation_beyond_the_craze.
- Schmidt, Gavin. 2016. “RealClimate: The Volcano Gambit.” Www.realclimate.org. April 9, 2016. https://www.realclimate.org/index.php/archives/2016/04/the-volcano-gambit/.
- Schuster, Robert, and Lynn Highland. 2001. “Open-File Report 01-0276; Socioeconomic and Environmental Impacts of Landslides.” Pubs.usgs.gov. 2001. https://pubs.usgs.gov/of/2001/ofr-01-0276/.
- Tans, Pieter, and Global Monitoring Laboratory. n.d. “Global Monitoring Laboratory - Carbon Cycle Greenhouse Gases.” Gml.noaa.gov. https://gml.noaa.gov/ccgg/trends/data.html.
- Vasan, Kishore, Milán Janosov, and Albert-László Barabási. 2022. “Quantifying NFT-Driven Networks in Crypto Art.” Scientific Reports 12 (1). https://doi.org/10.1038/s41598-022-05146-6.
- Wachter, Victor von, Johannes Rude Jensen, Ferdinand Regner, and Omri Ross. 2021. “NFT Wash Trading: Quantifying Suspicious Behaviour in NFT Markets.” SSRN Electronic Journal. https://doi.org/10.2139/ssrn.4037143.
- Wang, Qin, Rujia Li, Qi Wang, and Shiping Chen. 2021. “(PDF) Non-Fungible Token (NFT): Overview, Evaluation, Opportunities and Challenges.” ResearchGate. May 2021. https://www.researchgate.net/publication/351656444_Non-Fungible_Token_NFT_Overview_Evaluation_Opportunities_and_Challenges.
- Zhang, Luyao (Sunshine). 2022. “Machine Learning for Causal Inference.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/causal-inference/release/8.
- Zhang, Luyao (Sunshine), Zesen Zhuang, and Xinyu (Michelle) Tian. 2022. “Machine Learning for Predictions.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/ml-prediction/release/4.


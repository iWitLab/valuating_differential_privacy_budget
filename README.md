# valuating_differential_privacy_budget
Code to analyze the responses to a conjoint analysis survey on trade-offs between differential privacy valuation and contextual properties.

The code accompanies our paper, _"Valuating the Differential Privacy Budget in Data Sharing: A Conjoint Analysis"_, submitted to [the 17th IFIP International Summer School on Privacy and Identity Management, 2022](https://ifip-summerschool.github.io/archive/2022).

### Conjoint analysis
Conjoint analysis is a common research method typically employed for product and pricing research and frequently used across different industries. It enables researchers to review the decision-making process of users who are requested to choose a preferred item (such as product, setting, scenario and etc.) based on a set of attributes.

#### Use case
We consider a use case of a two-sided data market where individuals trade their personal data with a data collector, who in turn aggregates the data to perform a statistical data analysis that satisfies differential privacy.

A choice-based conjoint analysis with N=139 participants was performed to investigate the decision-making process of individuals under a differentially private data sharing scenario.

In our experiments, participants were asked to perform several choice-based tasks, where they select the most preferred description of a scenario, described by a set of attributes, in the context of different data sharing scenarios.


#### Questionnaire
The file `Qualtrics Conjoint Analysis Questionnaire.pdf` includes the survey protocol and its questions.
The survey was generated in the [Qualtrics](https://www.qualtrics.com/uk/) platform and distributed using the [Amazon Mechanical Turk (MTurk)](https://www.mturk.com/) platform.

#### Data
The file `DP_Conjoint_Analysis_Project_responses.csv` includes the raw responses of participants to the survey's questionnaire.

### Evaluation
* The code at the Jupyter notebook `qualtrics_conjoint_analysis.ipynb` loads the raw responses, processes them and calculates attribute importance of each attribute in the analysis, along with its part-worth utilities.
  * Change the path to your local downloaded data files.

**Note:** Code was tested and executed in `Python 3.8`.

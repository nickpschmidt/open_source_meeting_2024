# Open Source De-Biasing Discussion
By Nicholas Schmidt, SolasAI and BLDS, LLC


## Overview

This repository contains the code and data used to discuss open-source debiasing tools. My goal in these meetings is to provide regulators with an overview of some open source tools and libraries available for de-biasing machine learning models, and to discuss how these tools can be used to help the regulators in their mission to protect consumers from unfair, deceptive, or abusive practices in the financial marketplace.


## Data

The data used in this meeting comes from a processed version of a random sample of publicly available 2017 HMDA dataset. We use the variables in HMDA to predict whether an applicant is likely to receive a "low-priced loan."


## Creating the Environment

```
conda env create --file environment.yml --name [CHOSEN ENV NAME]
conda activate [CHOSEN ENV NAME]
pip install xgboost solas-ai aequitas fairlearn aif360[AdversarialDebiasing]
```

If you are on Windows, and you have issues with plotly plotting (this is an issue with the SolasAI library) you may need to run the following line after the prior lines. (This is as of July 2024. Hopefully, Kaleido will be fixed soon and this will not be necessary.)
```
pip install --force-reinstall kaleido==0.1.*
```


## Contact

For more information, please contact [Nicholas Schmidt](https://www.linkedin.com/in/nickpschmidt/).


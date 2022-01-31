# whale_analysis
Daily returns analysis from source csv file including performance, volatility, risk, risk-return profile and diversification
[![LinkedIn][linkedin-shield]][linkedin-url]
<!-- [![License][license-shield]][license-url] -->

<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="https://github.com/evianap/whale_analysis/blob/main/Images/Risk.jpeg" alt="Risk Analysis"" width="700" height="300">
  </a>

  <h3 align="center">whale_analysis_</h3>

  <p align="center">
    Evaluating Risk of Funds
    <br />
    <a href="https://github.com/evianap/whale_analysis"><strong>Go to documents »</strong></a>
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

<p>This project is designed to download data series from a csv file with historic market information from the S$&P 500 (used as benchmark) and 4 different funds. Ris is assessed and determinations are made on the most convenient fund depending on the risk apetite of the user<p/>

```
whale_df = whale_Dataframe =pd.read_csv(
    Path("./Resources/whale_navs.csv"), 
    index_col="date", 
    parse_dates=True, 
    infer_datetime_format=True
)
whale_df.head()
```
<p align="center"><img src="https://github.com/evianap/whale_analysis/blob/main/Images/Daily_Return.png" alt="series_screenshot" width="450" height="650"><p/>

<p>Standard deviation for all funds is calculated<p/>

```
standard_deviation = whale_daily_return.std()

standard_deviation.sort_values()
```


<p align="center"><img src="https://github.com/evianap/whale_analysis/blob/main/Images/Std_Dev.png" alt="screenshot_error_" width="550" height="200"><p/>
<p align="center"><img src="https://github.com/evianap/whale_analysis/blob/main/Images/Sharpe_Ratios.png" alt="screenshot_error_" width="550" height="200"><p/>

### Built With

<!-- This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples. -->

* [Python](https://www.python.org/)
* [Jupyter Lab](https://jupyter.org/install)

### Prerequisites

<!-- This is an example of how to list things you need to use the software and how to install them. -->
A variety of libraries were used and are needed for this program. They can be added using the below commands in terminal:

``` 
import numpy as np
import pandas as pd
from pathlib import Path
%matplotlib inline
```



<!-- CONTACT -->
## Contact

Enrique Viana - [@evianap][linkedin-url] - j.enrique.viana@gmail.com

Project Link: [https://github.com/evianap/whale_analysis](https://github.com/evianap/whale_analysis)

<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* [Kevin Lee](https://github.com/kevinclee26/)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

<!-- [license-shield]: 
[license-url]:  -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/enriqueviana/
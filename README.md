# AI-Generated-Text-Detector









<h3 align="center">Gitcoin-Beta-Grants-analysis-during-GR15</h3>

  <p align="center">
   This project aims to identify and flag potentially fraudulent projects during the Gitcoin Grant Round (GR) 15, which focuses on funding promising open source projects in the web 3 space. The GR is hosted by Gitcoin using the quadratic funding system to create a fair voting ecosystem for all projects. However, malicious actors known as SYBILS utilize fraudulent methods to vote for undeserving projects during the funding rounds.
    <br />
   
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
  </ol>
</details>



## ABOUT THE PROJECT

 This project is an analysis of the projects during the Gitcoin Grant Beta Grant Round (GR) 15. The aim of each GR which is held quaterly is to fund promising open source 
 projects mainly in the web 3 space. The GR is hosted by Gitcoin using the quadratic funding system. The use of the quadratic funding system was to create a free and fair voting 
 ecosystem for all projects irrespective of thier fudning power. Ditto to this innovation, criminal mastermind know as SYBILS use fraudulent methods to vote for undeserving projects 
 during the funding/ grant rounds. A sybil in lame man term is an attacker who creates multipe identities (wallet address) simultaneously within a peer-to network.
 So the main aim of this project is to identify and flag out fraudulent projects during the GR15 beta.


 For this project I modified and made use of the Website Vaalidation Lego from the Grants Review Dashboard Legos. I also built a Github Lego for checking grants Githubs.
 




<!-- GETTING STARTED -->
## Getting Started

To get started with this project, the installation of some python packages are required.

### Prerequisites

* os
  ```sh
  !pip install os
  ```
  
* request
  ```sh
  !pip install request
  ```
  
* validators
  ```sh
  !pip install validators
  ```
  
* pandas
  ```sh
  !pip install pandas
  ```
  
 * beautifulsoup4
  ```sh
  !pip install beautifulsoup4
  ```



<!-- USAGE EXAMPLES -->
## Methodology

I built off from the Website Validation lego created by the Open Data Community: _[Grant Review Snadbox Proj](https://github.com/OpenDataforWeb3-sandbox/Grant-Review-Dashboard/tree/main/LEGOS)_. For the first phase of the analysis, I passedeach website provided by
each grants through the lego to determine their validity. If the  response after running the lego was a 200 status code it would be grouped as True and if it return another 
status code for example 404, it would be grouped as False. But when running he code I encountered an error which was some website didn't return an error code which might be due to 
a down server or other reasons. In response to this challenge I created another output called "no_connection". Grants with this attribute were also channel through for further invetigations through other legos.
After I was able to draw out grants with fraudulent symptoms, I also inspected each of the owners address for fraudulent traits on etherscan. 




<!-- ROADMAP -->
## Roadmap

- [ ] Website Validation
- [ ] Github Validation (This package is still under development and susceptible to some slight errors and adjustmnts.) This packag was used to cross validate the result from (1)
- [ ] Etherscan Inspection
   


## Conclusion.

1.  40--50% of suspecious projects were identied by  the use of invallid website url  and github url. 
2.  A twittter lego to check feature like followers, tweets,  creation date  would also  be another effective tool.
3. This analysis continues  and the full report would be submitted on theh  13th may.
  I  will be using the GrantDNA lego to check for possible sybil activities in each grants.





# Ngram AdWords Analysis
### A Shiny app built for analyzing the Search Terms report from AdWords.

![preview](https://i.imgur.com/1gCVfoW.jpg)

---
### Data Cleaning  

- Export Search Terms Report as CSV from AdWords  
&nbsp;  
- Delete first and last two rows from CSV  
&nbsp;  
![first two](https://i.imgur.com/gwV5DOF.png)
&nbsp;
![last two](https://i.imgur.com/8yENiAQ.png)
&nbsp;
- Make sure numeric columns are formatted as numbers
  - exact to two decimal points
  - include no comma separators  
&nbsp;
- Your CSV has these columns
  - Clicks
  - Cost
  - Ctr
  - Conversions
  - Impressions
  - Avg. CPC

---
### Get Up & Running  

To run locally, clone the repo.
```bash
git clone https://github.com/beigebrucewayne/NgramShinyApp.git
```

Then, make sure you have R installed. The easiest way, if you have a Mac, is to use homebrew. Alternatively, you can always download from [CRAN](https://cran.r-project.org/).
```bash
brew tap homebrew/science
brew install Caskroom/cask/xquartz
brew install r
```

Finally, start R in the project directory and invoke the Shiny library.
```r
library(shiny)
shiny::runApp()
```

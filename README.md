# Do Left-Handed People Really Die Young? 

Welcome! This is a Python project intended to help you practice using Python for data science. 
The content of this project is nearly identical to the DataCamp project I created at the end of 2018, but this version is free!

## What is this project about?

![Barack Obama signs the Patient Protection and Affordable Care Act at the White House, March 23, 2010](img/Obama_signs_health_care-20100323.jpg)

Barack Obama is left-handed. So are Bill Gates and Oprah Winfrey; so were Babe Ruth and Marie Curie. A [1991 study](https://www.nejm.org/doi/full/10.1056/NEJM199104043241418) reported that left-handed people die on average nine years earlier than right-handed people. Nine years! Could this really be true? 

In this project, we will explore this phenomenon using age distribution data to see if we can reproduce a difference in average age at death purely from the changing rates of left-handedness over time, refuting the claim of early death for left-handers. This project uses `pandas` and Bayesian statistics to analyze the probability of being a certain age at death given that you are reported as left-handed or right-handed.

A National Geographic survey in 1986 resulted in over a million responses that included age, sex, and hand preference for throwing and writing. Researchers Avery Gilbert and Charles Wysocki analyzed this data and noticed that rates of left-handedness were around 13% for people younger than 40 but decreased with age to about 5% by the age of 80. They concluded based on analysis of a subgroup of people who throw left-handed but write right-handed that this age-dependence was primarily due to changing social acceptability of left-handedness. This means that the rates aren't a factor of *age* specifically but rather of the *year you were born*, and if the same study was done today, we should expect a shifted version of the same distribution as a function of age. 

This project uses two datasets: [death distribution data](https://www.cdc.gov/nchs/data/statab/vs00199_table310.pdf) for the United States from the year 1999 (source website [here](https://www.cdc.gov/nchs/nvss/mortality_tables.htm)) and rates of left-handedness digitized from a figure in this [1992 paper by Gilbert and Wysocki](https://www.ncbi.nlm.nih.gov/pubmed/1528408). 

## How to use this project

The Jupyter notebooks in this repo contain a series of cell blocks that fall into one of six types:

* **Context:** a text cell following a numbered title that contains background information about a task.
* **Instructions:** a text cell that contains the specific instructions for a task.
* **Hint:** a hint about how to accomplish the coding task.
* **Sample code:** scaffolding code to get you started on completing a task.
* **Solution:** my solution code for the task. This code will pass all the tests in the following cell.
* **Tests:** tests to check solutions for the task.

If you'd just like to see the entire project, you can read **[the full notebook](https://nbviewer.jupyter.org/github/mbonsma/lefty-longevity/blob/master/lefty_longevity_with_solutions.ipynb)** from top to bottom, glossing over the **hint**, **sample code**, and **tests** sections. 

If you'd like to work on this project as an exercise, download **[the workbook version](https://github.com/mbonsma/lefty-longevity/blob/master/lefty_longevity_workbook.ipynb)** of the notebook and follow the instructions in there. The instructions are also repeated below. If you have any issues at all getting set up, please let me know by opening an [Issue](https://github.com/mbonsma/lefty-longevity/issues) and I will be very happy to troubleshoot and make the instructions more clear. 

### Working through the exercises

#### Get set up with Jupyter and Python
1. Install [Jupyter notebook](https://jupyter.org/install) and Python. I recommend installing [Anaconda](https://www.anaconda.com/distribution/#download-section), which comes with both Jupyter and Python (and lots of other useful stuff). 
2. Download this notebook onto your computer. You can download the entire GitHub repository or just this notebook, your choice.
3. Run Jupyter Notebook: 
  * Open Anaconda Navigator and select Jupyter Notebook, or
  * Open a terminal window or anaconda prompt and type `jupyter notebook`. Jupyter Notebook will launch in your default browser.
4. In the Jupyter Notebook interface, navigate to the folder in which you saved this notebook, and click on it (`lefty_longevity_workbook.ipynb`) to open the notebook.

#### Using the notebook
1. Run the first cell below to load the testing module (optional)
2. Read the **context** and **instructions** cells below each numbered heading.
3. In the **sample code** cell, try coding your solution and running the cell. (To run a cell, click `Run` in the top menu or hit `SHIFT-ENTER`.)
4. To test your solution for each task, run the **tests** cell that directly follows the **sample code** cell.

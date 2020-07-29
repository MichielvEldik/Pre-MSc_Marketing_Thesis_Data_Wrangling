# Pre-MSc-Marketing-Thesis-Data-Wrangling

## Set-up of the experiment

I completed my thesis research by means of a between-subjects experimental design with two tasks using the online survey tool Qualtrics (N = 188).
One group was triggered to rely on their feelings whilst the other was conditioned to rely on logic and reasoning throughout these experiments.

The first task required participants to determine whether or not they saw a pattern for a series of twelve pictures on a scale from 1 to 9.
The mean score for all pictures in which no pattern was present is to be aggregated and compared across the experimental groups.

The second task required participants to come up with as many associations as possible for two common household objects within a timeframe of 2 minutes.
For the experiment, the contents of these answers didn't matter so much as the number of answers per individual. 

## Goal of the data wrangling program
The main purpose of this short program was to set up the dataset imported from Qualtrics to smoothly work in SPSS for analyses. Although SPSS offers great features to wrangle data, I found that certain things were simply much easier in Python and Pandas. 

### (1) 
Qualtrics was set up with three randomized series for the Snowy Picture Task. This means that an answer for a question may be found in 1 of 3 places in the dataset. Step 1 is to organize the dataset so that each question - regardless of in which series it appeared - is assigned to the same variable.

### (2)
Create a dummy variable based on the 'submit page' data for either of manipulation pages on Qualtrics. This dummy variable is necessary to distinguish between the two experimental groups (emotional and reasoned).

### (3)
Return a numerical variable that represents how many associations an individual case came up with for both tasks.

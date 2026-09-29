<<<<<<< HEAD
# QMEE
Bio 708

Assignment 7:
Making a GLM for my distance travelled data. 

## Assignment 5 (JD comments)

A good attempt to deal with difficult questions. Your beginning is not promising: “what are the differences” and “what genes are” different? These are not sharp questions: technically the answer would be everything changes, although you wouldn't see most of it without a giant sample size. But you do much better after that. You need to think more about Ucrit thresholds, but you are thinking in the right direction. For deseq, I'm not sure why you want to think separately about significance and size (or why you should be more conservative with a small sample size, the statistics should handle that for you in theory). You can combine ideas (here and maybe for Ucrit) by looking for things whose CI does not overlap the small-effect region (iow, you are confident effect is large).

Grade: 2.1/3

## Assignment 3

JD: Not sure why your third and fourth graphs have the gray background; the fifth graph looks much better without it. You should think about the advantages and disadvantages of including 0 on your vertical scales. I kind of like the fourth figure (except for the gray) and it doesn't bother me that much that I can't exactly tell where the CIs are, I feel like I get the sense of how much they overlap. I liked the discussion and the way you used color to indicate similarity. Grade: 2.1/3

Assignment 3:
I have plotted two concepts, firstly the maximum velocity following a startle, and secondly the distance travelled over time in the 200s following the startle. 

Firstly, maximum velocity. I plotted this as a boxplot and a violin plot. A benefit of the violin plot is that the reader can see every point on the graph and visually assess the data(works because it is a small dataset). In particular, because one hypothesis was that SETBP1 mutant fish would show particularly high and particularly low responses (hyper responsive and hypo responsive neurological defects) this graph does a good job of showing distribution. The violin plot is more exploratory, and useful for me as the researcher to assess my data. The boxplot is very clean, and looks more like a publication style plot (which is something that I wanted to practice). Both of these plots are position on a common scale, the highest ranked encoding in the cleveland hierarchy. The groups are ordered in a biological sense (rather than greatest to least for example). This is because I want my graph to reflect my research question, which asks if there is a difference between controls and SETBP1 mutant fish.

Secondly, graphing distance travelled over time. I plotted this as a few different styles of line graphs. The first one is what I would think of as a publication style graph. The second graph is anchored closer to the data points to look more closely at the data (data does not fit a log scale well), however this is a bit misleading of a scale so is only useful to explore the data and confidence intervals, not appropriate for a paper due to the overlapping CI's and scale. For these two graphs I had the categorical variable in a legend rather than as an axis to maximize the information that can be included in the plot. The genotype can be distinguehed by both shape and colour, this is because colour is low in the cleveland hierarchy, so I wanted to add another aspect to make the lines stand out more. Following a principle of comparison I made wildtype groups blue and knockout groups red because I do not need the reader to distinguish between different wildtype groups. The main comparison I want them to make is wildtype vs knockout, not specifically which wildtype or which knockout. 
In my final graph I made 4 different panels for each genotype. This graph is the most clear because the lines and confidence intervals do not overlap. This allows for confidence intervals to be viewed better. While this is lower in the cleveland hierarchy than position along a common scale, I think that the inclusion of confidence intervals is important in this case, so it is best to prioritize the confidence intervals being comprehensible than it is to prioritize being on a common scale. 

Assignment 2:
My first script reads a csv of startle response assay data. I checked and corrected the R classes of my variables, then plotted the total distance travelled, and max velocity in the first 20s as histograms to visualize the data and determine if there were any errors. The data showed all positive values (as expected), and the only NAs found were the expected blanks before the first measurement, so they were removed from analysis.  Because my variables of interest are maximum velocity in the first 20s of the assay, and total distance over the whole assay time, i made seperate dataframes for each of these variables, and saved them as rds. I set up these rds files to go to my gitignore. 
My second script reads in my two rds files, and confirms that they are dataframes. Then I calculate mean, standard deviation, and standard error by genotpe for maximum velocity for the first 20s and total distance travelled. I don't really know what statistical tests are most appropriate for this type of data, so i hope to increase the complexity of analysis in future assignments as we learn about statistical tests. I didn't have the chance to update my code to reflect the cleaner pipes and groupings we learned in class, but will modify for next assignment and future coding!
The directory that the first file should be run from QMEE/Assignment2_File1_Bio708.Rmd and the second file should be run from QMEE/Assignment2_File2_Bio708.Rmd



Assignment 1:
SETBP1-HD is a genetic disorder in humans caused by a knockout of the SETBP1 gene. SETBP1-HD currently has no treatment. This project aims to test if zebrafish are a good model for SETBP1-HD by inducing the same genetic mutation (SETBP1 knockout) in zebrafish. If zebrafish are a good biomedical model, they can be used to test theraputics for SETBP1-HD in high-throughput. 
SETBP1-HD causes neurodevelopmental disorders in humans, impacting behaviour. Thus, if zebrafish are a good biomedical model for SETBP1-HD, we would expect to see modified behaviour in SETBP1 knockout fish relative to wildtype fish. This is measured through a startle response assay. 
The startle response behavioural assay aims to measure the response of animals to a sudden stimulus (similar to a startle response to a predator).  I want to determine if SETBP1 knockout zebrafish display a "hyperactive" response to startle stimulus. To do so I ask, do SETBP1 knockout zebrafish display a greater distance moved in response to a startle than wildtype fish do? I also ask do SETBP1 knockout fish display a higher maximum velocity swim in response to startle stimulus than wildtype fish (immediately following startle)? Finally, I ask if a hemizygous knockout of SETBP1 has the impacts on velocity and distance travelled as a homozygous knockout does?
This dataset contains four groups of zebrafish, who have been subjected to an auditory startle response stimulus. The first two groups of fish are control fish, one is wildtype ("WT") , and one is another group of wildtype control with a different parent backgroud ("WTSK"). The next group is an experimental group, SETBP1 hemizygous knockouts (KO). The final group is also an experimental group, SETBP1 homozygous knockouts ("KOKO"). 
This makes a boxplot of the total distance travelled during the assay by each of these four groups, with the median noted on the plot.
This also makes a boxplot of the maximum velocity immediately following the startle(first 20s) for each of the groups, with the median value noted on the boxplot. 

In the future I hope to complete statistical tests to identify if differences between any of the groups are statistically significant - but maybe I can do that later in the course once we have learned when to do different tests!
=======
Critical swim capacity test of adult fish with a SETBP1 mutation
>>>>>>> 7aca7c299d610c669ee238d88c4bf63a06ff8322
# SETBP1-HD

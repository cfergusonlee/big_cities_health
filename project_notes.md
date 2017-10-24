## Plan

Now that we have a better idea of the overall data structure, we can better formulate a plan as to what to do with the data. We have reshaped it so that we can document interactions between variables. There are many avenues to explore in regards to visualizations, variable interactions, and modeling. What might be important to an insurance company or hospital looking at this data? There are both visualizations and models that they are probably interested in.

### Vizualiations

For visualizations, let's throw a few in here but also try a few out in Tableau. Tableau will be quicker and because we can just drag and drop. If we need to do any major reshaping, that can easily be done in Python before porting back into Tableau.

Let's create the visualizations we have in our list above, then dive into Tableau to look at what else can be made.

1. Plan which features you want to explore
  1. Can't do all 53, untenable
  2. Can do overview and automate certain parts to accomplish more
  3. Choose some that are interesting to you and some that may be of interest to organizations. Not carving out of marble. It's always possible to come back for more later
    1. Chronic Disease
    2. Infectious disease
    3. Behavioral health/substance abuse
    4. Life expectancy / death rate
2. Create visualizations in list
3. Create more in Tableau

### Models

For models, we need to think carefully about what insights might be important:
- Mortality rates?
- Cancer rates?
- Separate classifiers by gender and ethnicity?

Before we can create our models, however; we need to research what we can do with all the missing data points. Just about every row has missing data and I don't believe our algorithms can work with them in that form. Do we need imputation? Should we delete columns with mostly sparse data? If there are rows that are mostly complete, should we just use those? Let's take another look at the missing data now that the data has been reshaped. Then we'll research what can be done for the remaining data.

1. Visualize missing data with msno
2. Research missing workarounds: 
  1. Titanic
  2. Look for others
3. Decide whether we can continue with models or we need to just stick to visualizations
4. Choose appropriate algorithms for the data
5. Model a handful
6. Tune algorithms
7. Share insights
8. Move on

## Feature Engineering

Need to figure out what you want to predict. Look at all features and decide what might be most useful to a hospital or healthcare provider. Then look at features and decide:

1. Which ones might be useful
2. Whether they require scaling
3. Transform necessary categorical variables

## Modeling

Use a variety of algorithms, pick the best one or two and tune those parameters.


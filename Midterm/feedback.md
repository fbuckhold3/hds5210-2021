Score: 50/50

Nice work on all the calculation functions.

In the last part, just a couple of notes:

When you want to change the column names in a pandas dataframe, the quickest way to do that is `data.columns = ['a','b','c','d'...]`

Also, it's generally not best practice to use `iterrows()` with dataframes, because it can get slow when the dataframes get very large.  It's better to use dataframe.apply(...).



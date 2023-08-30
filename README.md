# Data Visualization

## The project is to analyze the housing rental market data for San Francisco by using professionally styled and formatted interactive visualizations.

1. Calculate and plot the housing units per year:
   * Use the `groupby` function to group the data by year. Aggregate the results by the `mean` of the groups.
   * Use the `hvplot` function to plot the `housing_units_by_year` DataFrame as a `bar chart`. Make the `x-axis` represent the year and the `y-axis` represent the housing_units.
   * Style and format the `line plot` to ensure a professionally styled visualization.

2. Calculate and plot the average prices per square foot:
   * Group the data by year, and then average the results.
   * Create a new DataFrame named `prices_square_foot_by_year` by filtering out the “housing_units” column.
   * Use `hvPlot` to plot the `prices_square_foot_by_year` DataFrame as a `line plot`.
   * Style and format the `line plot` to ensure a professionally styled visualization.

3. Compare the average prices by neighborhood:
   * Create a new DataFrame that groups the original DataFrame by `year` and `neighborhood`. Aggregate the results by the `mean` of the groups.
   * Filter out the “housing_units” column to create a DataFrame that includes only the `sale_price_sqr_foot` and `gross_rent averages per year`.
   * Create an interactive `line plot` with `hvPlo`t that visualizes both `sale_price_sqr_foo`t and `gross_rent`. Set the `x-axis` parameter to the year (x="year"). Use the groupby parameter to create an interactive widget for neighborhood.
   * Style and format the `line plot` to ensure a professionally styled visualization.

4. Build an interactive neighborhood map:
   * Read the `neighborhood_coordinates`.csv file from the Resources folder into the notebook, and create a DataFrame named `neighborhood_locations_df`. Be sure to set the `index_col` of the DataFrame as “Neighborhood”.
   * Using the original `sfo_data_df` Dataframe, create a DataFrame named `all_neighborhood_info_df` that groups the data by neighborhood. Aggregate the results by the `mean` of the group.
   * Review the two code cells that concatenate the `neighborhood_locations_df DataFrame` with the `all_neighborhood_info_df DataFrame`. 
   * Using `hvPlot` with GeoViews enabled, create a `points plot` for the `all_neighborhoods_df`DataFrame.
  

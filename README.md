#About the Project :
This data is related with direct marketing campaign by a Portuguese Banking Institution (Dataset, 2024). The Goal of the Campaign was to classify weather the client will subscribe a term deposit or not. This dataset contains 16 features which affect the Term Deposit Classification. The dataset contains 768587 Data with 0 null values in any of the columns. Our Aim is to find when the Campaign is Successful which is when the client aggresses to make a Term Deposit and try to find the factors affecting it.

#Columns in the Data:

age	->	Age			
job	->	type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')		
marital	->	Marital Status	marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)		
education	->	Education Level	(categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')		
default	->		has credit in default?		
balance		->	average yearly balance	euros	
housing	->		has housing loan?		
loan	->		has personal loan?		
contact	->		contact communication type (categorical: 'cellular','telephone')		
day_of_week	->		last contact day of the week
month	->		last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')		
duration	->		last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.		
campaign	->		number of contacts performed during this campaign and for this client (numeric, includes last contact)
pdays	->	number of days that passed by after the client was last contacted from a previous campaign (numeric; -1 means client was not previously contacted)		
previous	->		number of contacts performed before this campaign and for this client		
poutcome	->	outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')		
y	Target	->		has the client subscribed a term deposit?

#Functions Used
#Histogram Function:
 
    
    Creates a Histogram for the given Data 

    Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - x_var (list or a array) : The data to plot.
    - title (str, optional) : The title of the plot.
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - bins (int ,optional) : The number of bins to divide the data into (Default is 5).
    - color (str, optional) : THe color of the bars (Default is lightblue).
    - edgecolour (str, optional) : The color of the bar edges (Default is black).
    - alpha (float,optional)The transparency of the bars, from 0 (transparent) to 1 (opaque) (default is 0.8).

    Returns:
    - None: The function will display a Histogram
  

  #Bar Chart Function:

  Creates a Bar Chart for the given Data 

    Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - column_name (list or a array) : The data to plot.
    - title (str, optional) : The title of the plot.
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.

    Returns:
    - None: The function will display a Bar Chart

  
#Scatter Plot :

    Creates a Scatter Plot for the given Data 

    Parameters:
    - xaxis (str) : The Column name to plot on x axis 
    - yaxis (str) : The column name to plot on y axis .
    - title (str, optional) : The title of the plot.
    - hue (str or list) : Grouping variable that will produce points with different colors. Default is None
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - palette (str or list): Colors to use for different levels of the hue. 
    - alpha (float): Transparency of the points, between 0(fully transparent) and 1(fully opaque).
    - fontsize (int, optional) : Fontsize of the legend (Default is 14)

    Returns:
    - None: The function will display a Scatter Plot
    
#Heat MAP
    
    Creates a Heat Map for the given Data 

    Parameters:
    - Dataset : The dataset name

    Returns:
    - None: The function will display a Heat Map

Fitting Function

 
Function for fitting a straight line, for curve_fit
        x: independent variable
        a, b: parameters to be fitted

        Returns :  y value
one_silhouette for data 

    Calculates the silhouette score for n clusters.

    - n (int) - Number of Clusters
    - xy -  dataset containing the 2 columns for the clustering to be done on 

    Returns : The score for each cluster

    

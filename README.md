# Road Accident Analysis (India)

Road accidents resulting in fatalities, injuries have evolved as a major issue across the world. According to the Global Status Report on Road Safety 2018 published by World Health Organization (WHO), the burden of road traffic injuries and deaths is borne by vulnerable road users living in low and middle income countries where deaths are increasing due to abrupt growth of motorized transport. Road accident injuries are the leading cause of death for children and young adults aged 5-29 years. Road injuries cause considerable economic losses to individuals, their families, and to nations as a whole. These losses arise from the cost of treatment as well as lost productivity for those killed or disabled by their injuries, and for family members who need to take time off work or school to care for the injured. It is estimated that road crashes alone are responsible for 3 to 4 percent of GDP loss in most of the countries including India. Considering the severity of the above issue it is very much essential to identify the underlying factors of road crashes in order to control the destruction caused to human lives as well as the national asset.  

Hence as a Countermove, We have gathered the past data, precisely of 2018 data from the Following Website https://data.gov.in/

# PreProcessing

The data set from the above website was available in chunks. So we merged the individual chunks into a single main dataset. You can find the merged Dataset in the DataSet Folder. we have shared both the XLS and CSV Format.

For Analysis, the counts of the Accidents are required where in the dataset has got few Strings (NR) which were removed. You can find those steps in the "Road Accident Data Analysis" Jupyter Notebook in Analysis Fold

For Prediction: 
  - We calculated Mean for each attribute, if the corresponding value for each state is greater than mean then it is replaced with 'Yes' otherwise 'No'.
  - Another Dataset is prepared manually which has individual categorical attributes set for every state. You can check Road Accident Labelled Data (csv or xsl).
  - Now, these categorical attribute values are replaced with 'Yes' or 'No' with the initial dataset help.
  - We created a new column 'ACCIDENT OCCURRENCE'
  - 'ACCIDENT OCCURRENCE' column is replaced with 'Yes' if it has more than 7 yes values in the row, otherwise 'No'
  - After adding a new column we have finally converted into 'Final Road Accident Dataset.csv'   

All the code for the Pre Processing Steps for Prediction can found in Prediction Folder. You can check "Road-Accident Prediction - Pre Processing" Jupyter Notebook.

# Analysis

We have used Pie Charts and Bar Graphs for Representing and also for Analysis the data. You can go to Analysis Folder and check the "Road Accident Data Analysis" Jupyter Notebook for the same.

# Prediction
We have opted for AdaBoostClassifier for the prediction of occurence of Road Accidents. You can go to Prediction Folder and check the "Road-Accident Prediction" Jupyter Notebook for the same.

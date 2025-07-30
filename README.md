
 [Definition of EDA](#EDA)
- [OBJECTIVES](#objectives)
- [IMPORTING](#import)
- [Steps of EDA](#StepsofEDA)
- [practical_implementation_of_stepsofEDA](#[practical_implementation_of_stepsofEDA)

## What is EDA:
It is simply the exploration of data to know about different aspects of data 
There are different techniques 
We need to make sure data is clean ,contain no redundancies ,null values, identifying important variables,removal of noise, relationship of variables through EDA

## Objectives of EDA:
EDA helps to find out faulty points 
Relationship between variables

## Steps of EDA
Firstly, we upload the required datasheet
Inorder to perfrom EDA we need to take 3 steps 

## Understanding the data
knowing about columns,unique values in columns by using 
df['nameofcolumn'].unique()
df.nunique()
df.shape(knowing about size of data i.e rows and columns)


## Cleaning the data 
This can be done by removing redundancies,null values (NaN),removing noise incase of audio data,removing duplicated data
then if there is any data like the address,phone number,date ,years etc that feels scattered then fix it 
(in my assignment i have used AI for this becasue I was bit confused how to do that)
while cleaning data the data I checked for rows if they need to be removed as my data was too large with 9998 rows and 9 columns which was reduced to 968 rows and 8 columns 
after performing the above operations
inorder to check if we need to remove rows or not incase of large data 5000,9000 etc the number of rows containing empty spaces i.e I had checked there were more than
1000 empty spaces so in this case it is better to fill these spaces using median mode mean 
i checked mean ,median if mean was> median so i used median and vice verse
mean_value = df['RATING'].mean()
df['RATING'].fillna(mean_value) used this approach to find mean,median and fill the data 

## Analysis (relationship between variables)
This is done by scatter plot,catplot,replot and some these are somewhat related 
a)relplot 
b)catplot
c)displot(cretaed a graph like histo)
d)scatter plot (creates scatter plot
e)pair plot
these plots are used to give a visulaization to user
## tale of contents

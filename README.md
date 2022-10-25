# Assignment-Due-DATE-25oct
#line chart,CGPA of all male students,(csv file),colors of male vs female......

  #Print the percentage of students who have a CGPA of 3.0 or above.
x=0
b=0
df2 = df['CGPA']
for i in df2:
    x+=1
print(x)                   
for i in df2:
    if i>=3:
        b+=1
#       print(i)

#Plot a pie chart to show the ratio of male and female students.

for_labal = newdf.gender_types
for_value = newdf.total

fig = plt.figure()
ax = fig.add_axes([0,0,1,1])
ax.axis('equal')

ax.pie(for_value, labels = for_labal, autopct='%1.2f%%')

  #Create a correlation matrix between HSSC-1 and HSSC-2 marks and then plot on a heatmap.
  
import seaborn as sns
calls = df[['HSSC-1','HSSC-2']]
matrix=nums.corr()

plt.figure(figsize=(8,5))
plot = sns.heatmap(calls.corr()
  
  #Load the dataset (csv file) into a Pandas DataFrame.
  
import pandas as pd

url = 'https://drive.google.com/file/d/1xpPrW3ivqQPm029cr0KccSbWUAPiPF6S/view?usp=sharing.csv'
df = pd.read_csv(url,index_col=0)
#df = pd.read_csv(url)

print(df.head(5))

  # Plot line chart of students and their birth months
plt.figure(figsize=(18,35))
plt.plot(df['BirthMonth'],df['Name'])
plt.ylabel('Students')
plt.xlabel('Birth Month')
plt.show()

  #Plot the favorite colors of male vs female students on a bar chart.
sns.countplot(x='FavoriteColor',hue='Gender',data=df)
sns.set(rc={'figure.figsize':(20,20)})
plt.title("Bar Chart of favorite colors of male vs female students")
plt.show()
  # Plot the CGPA of all male students on a histogram with intervals 2.0-2.5, 2.6-3.0, 3.1-3.5, 3.6-4.0.
  
df['CGPA'].plot(kind='hist');
plt.xlabel("CGPA Interval", labelpad=14)

plt.ylabel("Male Students", labelpad=14)

plt.title("CGPA of All Male Students are there", y=1.015, fontsize=22);
# ring from 2.0 - 4.0
plt.xlim([2.0,4.0])

  #Bonus points: What other things (insights) you can get from the dataset?
Data analytics is a process that allows you to extract insights from data sets that could otherwise be either too big or complex to analyze on your own.
--->Tracking competitors’ keyword rankings to get a better understanding of keywords that work for your company

--->Predictive analytics to help you avoid customer churn, optimize your marketing budget, and identify potential up

  #Print the list of all students whose first name starts with letter the 'H'.
 # Words starting with specific letter
 
# initializing list
test_list = ['Hkash', 'Hikhil', 'Hanjeet', 'akshat']
 
# initializing check letter
check = 'H'
 
# printing original list
print("The original list : " + str(test_list))
 
# Words starting with specific letter
res=[]
for i in test_list:
    if(i.find(check)==0 or i.find(check.lower())==0):
        res.append(i)
# print result
print("The list of matching first letter : " + str(res))

# Print the total number of students who have a three words name (first-middle-surname).
class PassportController {
  constructor() {
    this.details = {};
    // English letters, spaces and the following symbols ' - . are allowed
    // Max length determined by ng-maxlength for better error messaging
    this.nameRegex = /^[a-zA-Z '.-]*$/;
  }
}

angular.module('akyc', ['ngMessages'])
  .controller('PassportController', PassportController);

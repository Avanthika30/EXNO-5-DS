# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
<img width="714" height="533" alt="image" src="https://github.com/user-attachments/assets/7fc6ff13-d6de-4883-b7df-6320ef19b5b9" />

```
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/badff502-0d0d-4f93-9c72-2408ecfc5074" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
plt.show()
```
<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/68f97e1e-861d-4174-b66e-72617791a3ab" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue') # Added closing quote and a color 'blue'
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations')
plt.show()
```
<img width="558" height="453" alt="image" src="https://github.com/user-attachments/assets/437f05a6-7efe-4131-b776-220c47c40bc3" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
<img width="764" height="568" alt="image" src="https://github.com/user-attachments/assets/0eb4d2bc-98d9-470d-8a1d-abedd43964f3" />

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9375,0.895] 
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.895] 
plt.plot(years , apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="576" height="432" alt="image" src="https://github.com/user-attachments/assets/0288b35e-ed50-4bfe-93b0-383b7d9cfa78" />

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
plt.title("Crop yield in Kanto")
plt.legend(['Apples','Oranges'])
```
<img width="766" height="610" alt="image" src="https://github.com/user-attachments/assets/07cafb2f-c693-4ce2-82e6-b0d147c46988" />

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="585" height="432" alt="image" src="https://github.com/user-attachments/assets/2ea43859-d782-4f39-9ea8-7393cd9f1f17" />

```
plt.figure(figsize=(12,6))
years=range(2000,2012)
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (tons per hectare)");
```
<img width="990" height="526" alt="image" src="https://github.com/user-attachments/assets/109de88a-54f8-4b95-8b67-3cd67429911e" />

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in kanto")
plt.legend(['Apples','Oranges'])
```
<img width="760" height="605" alt="image" src="https://github.com/user-attachments/assets/e114f5dc-b535-4787-8be7-ecbefbbff657" />

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="red")
plt.show()
```
<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/b122a1ea-62f7-4433-9610-e624a1aaf16c" />

```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
<img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/05774ae2-b78d-4c99-8e8d-5a3131231f0e" />

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
<img width="554" height="453" alt="image" src="https://github.com/user-attachments/assets/941a82cf-c2de-4daa-a252-6694ca94d7b3" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="709" height="569" alt="image" src="https://github.com/user-attachments/assets/5cc0f0e2-6f05-4aa9-861b-3f614963f232" />

```
import numpy as np
np.pi
```
<img width="182" height="39" alt="image" src="https://github.com/user-attachments/assets/20f18d63-7e06-4bf5-a2d4-1b81e025bc82" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
<img width="568" height="433" alt="image" src="https://github.com/user-attachments/assets/f2860d7c-f013-4545-ab08-0d3ad53491d6" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="556" height="413" alt="image" src="https://github.com/user-attachments/assets/369f6c74-414e-48e7-9076-fbea9c9db108" />

```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='Spline')
plt.legend()
plt.show()
```
<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/0e3e9290-5927-4b82-9d77-0ce80547c459" />

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color="green")
plt.show()
```
<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/a53d7adc-ee7b-4a9f-9a5c-91631a1c4f77" />

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
<img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/4d7773e9-d436-41d6-b9de-f0c6e84c6dc7" />

```
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/9c4b8a89-e88b-41a0-92e9-dea0a517d671" />
# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.

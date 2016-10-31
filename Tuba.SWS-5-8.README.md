####Worksheet	5 - Do	chapter	3	of	online	R	tutorial	
http://tryr.codeschool.com/

1.	How	could	you	make	a	matrix	that	is	5	columns	wide	and	2	rows	deep	and	that	
has	the	value	1	in	each	cell?	

>``` matrix(1, 2, 5)```

2.How	could	you	make	a	matrix	that	is	2	wide	and	2	deep	and	that	has	the	values	
10,	14,	20	and	30	in	it?	
 
>```a<-c(10,14,20,30)```

>``` matrix(a, 2, 2)```

3.What	does	the	dim	assignment	function	do	to	a	vector?	

The dim assignment function sets dimensions for a matrix. It accepts a vector with the number of rows and the number of columns to assign.

4.This	chapter	is	about	matrices.	Can	you	think	of	data	that	would	come	in	the	form	
of	a	matrix?	Remember	that	in	a	matrix,	all	cells	have	the	same	datatype.	

No,we will need to have different data types in order to run the functions.We can combine different data matrix in a data frame in order to run the program.

5.You	learned	three	commands	to	plot	a	matrix.	Which	are	they?	Which	one	do	you	
think	would	be	most	useful?

Countour(),Presp(),image()

Depending on what we need to explore with a given data  we can use any of those commands.I think countour can be  most used commands since it gives the general view of vectors in a plot.

Let's say that x is a vector contains the height and the enlargement of a mountain.

```>a<-(matrix(1, 10, 10)```

spot where I dug down to ground level

```> a[4, 6] <-0```


Depending on the situation

``` >contour(a)```

countour can be helpful to see general format of the vectors in a plot.

```>persp(a)```

persp is helpful to see 3D formatted version of the vectors in plot.


``` >image(a)```

Image function is helpful to see heat map of the vectors that we are working on.
It was a volcano in the web-page.



###Worksheet	6:	Do	chapter	4	of	Try	R	codeschool	

1.You	used	about	5	functions	in	this	tutorial.		Write	down	the	functions	and	how	
they	work.	

Mean:A quick way to assess our battle-readiness.It gives us the average of  accounts appendage counts.
let's create a vector called limbs.
>```limbs <- c(4, 3, 4, 3, 2, 4, 4, 4)```

Now get the mean value of it.

> ```mean(limbs)```

Barplot:We can make a column plots of given vector.

```barplot(vectorname)```

Abline:In order to compare the various values to the average,we can draw a line on the plot representing the mean.The function takes an h parameter with a value at which to draw a horizontal line,or a v parameter for vertical line.
First we make a barplot of the vector 

>``` barplot(limbs)```

Then get the horizontal line across the plot at the mean with abline factor.

>```abline(h = mean(limbs))```

Median:The median is calculation of the average of middle values.

median function on the vector:

>``` median(limbs)```


Standard Deviation:st is used from the mean to describe the range of typical values for a data set. For a group of numbers, it shows how much they typically vary from the average value.Standard deviation is long calculation mathematically.R gives a simple usage for it. 

```> deviation <- sd(vector name)```

2.Several	objects	were	used	in	this	tutorial.	Two	of	them	are	vectors	- which	ones?	
Which	ones	were	simple	"numeric"s?	

Limbs and pounds were used.
Limbs and pounds both used in numbers,but limbs has the simple numeric.
Pound contains larger numbers in the tutorial as values of the hauls . 


3.How	would	you	use	the	function	abline	to	create	a	horizontal	line	that	crosses	the	
y-axis	at	10?	And	a	vertical	line	that	crosses	the	x-axis	at	10?
If	you	want	to	try	this	out (which	would	be	great!	use	Rstudio),	you	need	to	first	
create	a	plot	with	some	data,	for	example:
x<-1:12
y<-1:12
plot(x,y)
Now	you	can	play	with	the	abline()	function	to	add	horizontal	and	vertical	lines.	
```x<-1:12```
```y<-1:12```
```plot(x,y)```
Now	you	can	play	with	the	abline()	function	to	add	horizontal	and	vertical	lines.	

```>meanValue <- mean(x)```

6.5

```> abline(h=meanValue)```

```> meanValue<- mean(y)```

6.5

```> abline(v=meanValue)```

``> deviation <- sd (x) ``

3.5

```deviation <- sd (y)```

3.5

```abline(h = meanValue + deviation)```

6.5+3.5=10 line passes through 10 horizontally

```abline(v = meanValue + deviation)```

6.5+3.5=10 line passes through 10 vertically



###worksheet  7 
I watched the videos and checked out the web page in order to complete the task 6.

Task6.Create	a	new	R	script	in	Rstudio
Write	code	to	make	two	numeric	vectors of	equal	length,	and	plot	them	in	a	scatter	
plot.
Then	plot	one	of	them	in	a	barplot.	Make	the	barplot	horizontal.	
Create	a	matrix	that	combines	both	vectors	using	rbind(vector1,vector2)	and	create	
a	barplot	of	that	matrix.	

```>y<-c(1:10)```

```> x<-c(1:10)```

```>plot(x,y , main = "Scatter Plot Example", xlab= "weight of he mice" , ylab="Height of the mice")```

```>barplot(x,y , main = "Bar Plot Example", xlab= "weight of he mice" , ylab="Height of the mice")```

Simple Horizontal Bar Plot

```barplot(x,y , main = "H Plot Example", horiz =TRUE)
 
matrix

``> matrix(rbind(x,y))``


 ```>barplot(matrix(rbind(x,y)))```

####Worksheet 8

Task	1.	Come	up	with	at	least	4	examples	of	data	that	should	be	stored	as	factors.	
R has factor function to track the catagorized values.Factor function helpful to make data frames.
In these cace we can factor function as a 

1.Names(First Names,Last names)

2.Date of brith,death,graduation

3.Marial Status

4.Catogorize the data as(public or private or old and new etc...)

5.Insurance plans

Task2.	Explain	all	parts	of	the	command	

plot(weights, prices, pch=as.integer(types))

Plot the weights and prices for each type by converting the factor to integers and passing it to the pch argument of the plot.
It will then plot the each type of the data with different symbols on the graph to make the variables  clearly seen. 














	


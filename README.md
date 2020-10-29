# MLB-Championship-Team

MoneyBall 2.0
Examination of American' Past time

Purpose of Project

Extracted MLB data from (1969-Present)
Determined which statistical categories were relevant to our overall objective
Built models to predict WS winners by team and league from (’15 -’20)

Available Features 

Year, League, Total Games, Home Games, Wins, Losses, Winning %, Won World Series, Runs, At Bats, Hits, Doubles,  Triples, Homeruns, Base by Ball, strikeouts, complete games, Stolen Bases, ERA, Shutouts, Saves, name


![](Hitting.PNG)
![](Fielding.PNG)
![](League.PNG)
![](WL.PNG)



The Models

Neural Network Model

-	Feature selection –

'Wins', 'Losses', 'Winning %', 'Won World Series', 'Runs', 'Hits', 'Doubles',
      		 'Triples', 'Homeruns', 'Base by Balls', 'Stolen Bases', 'ERA', 'Shutouts', 'Saves', 'name'

-	Parameters

o	18 inputs, activation = ‘relu’
o	1 hidden layer (100 nodes)
o	36 outputs
o	Training accuracy – 0.51
o	Testing accuracy – 0.16

SVM

-	Feature selection –

'Wins', 'Losses', 'Winning %', 'Won World Series', 'Runs', ‘At Bats’, 'Hits', 'Doubles',  'Triples', 'Homeruns', 'Base by Balls', 'Stolen Bases', ‘Strikeouts’, 'ERA', 'Shutouts', 'Saves', 'name'

-	Parameter

o	Linear Kernel
o	‘C’ parameter - 500
o	‘gamma’ – 0.0001
o	Training accuracy – 0.13
o	Testing accuracy – 0.18




RandomForestClassifier

-	Feature selection 

'Wins', 'Losses', 'Winning %', 'Won World Series', 'Runs',  'Hits', 'Doubles',  'Triples',   'Homeruns', 'Base by Balls', 'Stolen Bases', ‘Strikeouts’, 'ERA', 'Shutouts', 'Saves', 'name'

-	Parameters

o	Linear Kernel
o	‘bootstrap’ - True
o	‘max depth’ – 40
o	‘n-estimator’ – 500
o	Testing accuracy – 0.20

![](Chart.PNG)


Lessons Learned

-	Could have used more inputs/features (increase accuracy)
-	Figured out how require less outputs
-	More data
-	Ensure outcomes are included in each year
-	Maybe look at individual games instead of seasons

Conclusion

-	Requiring 36 outputs yields 0.20 accuracy (2 outputs yield >0.70)
-	Neural Network appears to be the better model
-	2015 Neural Network accurately pick the World Series Champ and RandomForestClassifier picked the AL team the Royals beat.

Burning Questions

Why did neural network pick Montreal for 2020?
Why were most of the picks in the center of their division?
Why were last place teams picked?

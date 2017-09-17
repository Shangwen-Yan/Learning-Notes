Introduction to Machine Learning 

Homework 2: Multiple Linear Regression

Shangwen Yan | N17091204 | sy2160

=========================================================================================================================

1\. 
(a) past sales

(b) extract numeric score as vector $x_1$, frequency of occurence of words as vector $x_2$(positive when good, negative when bad, and assign weight towards different words), the model is like: $\hat{y}=\beta_0+\beta_1x_1+\beta_2x_2 $


(c) $\hat{y}=\beta_0+\beta_1(x_{11}+\frac{1}{2}x_{12})+\beta_2x_2 $, numeric score from 1 to 5 as $x_{11}$, numeric score from 1 to 10 as $x_{12}$

(d) score from 1 to 5 as $x_{11}$; rating as $x_{12}$, $x_{12}=5$ when good, $x_{12}=1$ when bad; no numeric rating as $x_{13}=2.5$; so, $x_{1}=x_{11}+x{12}+x{13}$ and the model is still: $\hat{y}=\beta_0+\beta_1x_1+\beta_2x_2 $

(e) I would suggest fraction of reviews with the word "good", but the total number of reviews also have significance(more popular, more reviews), so I would also suggest to add another predictor of the total number of reviews(both good and bad)

2\. (a)assume the model is: $\hat{y}=\beta_0+\beta_1x_1+\beta_2x_2 $(b) $\hat{y}=0.75+2.5x_1+3.5x_2 $3\.(a)
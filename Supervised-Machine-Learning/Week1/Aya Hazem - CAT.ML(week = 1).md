
## Machine Learning Questions
1. Define machine learning; what are the differences between machine learning and normal programming?

		A branch of AI and CS that uses data and learning algorithms to imitate the way humans learn, gradually improving its accuracy
		Feild of study that gives the computer the ability to learn by itself without being explicitly programmed
		A computer is said to learn from task T given some previous experience E with some performance measure P, if its performance P increases with experience E. 
		For example a ML programm to flag spam emails "task" that given example of spam and no spam emails also called training set "experience" can learn to flag spam and its performance improves with experience. Instead of writing expliced rules to detect patterns in spam emails using traditional programming, ML model can automatically detect patterns and udpate them given new data.



		Traditional programming takes input data and  a programm of well-defined instructions, excutes it on the input data and produces some output.
		ML takes the input and the output data puts them in a black box "model" and produces a program that can predict the output from input data


2. There're 4 types of machine learning:
	-   Supervised Learning.
	-   Unsupervised Learning.
	-   Semi-Supervised Learning.
	-   Reinforced Learning. 

	
	$\Rightarrow$ Compare two of them, at least, to each other.
	<br></br>

	<table style="width:100%">
	<tr>
		<th>Supervised Learning</th>
		<th>Unsupervised Learning</th>
		<th>Semi-Supervised Learning</th>
		<th>Reinforced Learning</th>
	</tr>
	<tr>
		<td style="width:25%">
			In supervised learning, the training set you feed the learnig algorithm have the disred output solutions "labels\targets" with the needed input data, the learning algorithm tries to predict the output labels given a new input data
		</td>
		<td style="width:25%">
			In unsupervised learning, the training set features isn't associated with any output labels, the learning algorithm tries to find some structure or patterns in the data.
		</td>
		<td style="width:25%">
			part of the training data set is labeled another is not labeled this could be helpful when working with larger data as labeling can be time consuming 
		</td>
		<td style="width:25%">
		<p> 
			branch of Machine Learning int whichtha agents or bots try to pick up actions that will maximize their rewards over time 
		</p>
		</td>
	</tr>
	<tr>
		<td>
			<ul style="list-style-type:disc;">
				<li>Classification</li> 
				<li>Regression</li>
			</ul>
		</td>
		<td>
			<ul style="list-style-type:disc;">
				<li>Clustering</li> 
				<li>Anomely dectection</li>
				<li>Dimensionality reduction</li>
			</ul>
		</td>
		<td>-</td>
		<td>-</td>
	</tr>
	<tr>
		<td>
			<ul style="list-style-type:disc;">
				<li>Spam filter given a labeled spam, non-spam emails </li> 
				<li>predicting a car's price given its attributes and price</li>
			</ul>
		</td>
		<td>
			<ul style="list-style-type:disc;">
				<li>Google news recommending similar articles to what you engage with</li> 
			</ul>
		</td>
		<td>-</td>
		<td>-</td>
	</tr>
	</table>


3. Clustering is _______________ , and Classification is _______________ :

	|    Clustering    |  Classification  |
	|------------------|:---------------:|
	| <input type="checkbox" /> Supervised   |<div style="text-align: left"> <input type="checkbox" checked /> Supervised </div> |
	|<input type="checkbox" checked/> Unsupervised |<div style="text-align: left"><input type="checkbox" /> Unsupervised</div> |
	| <input type="checkbox" /> Reinforced   | <div style="text-align: left"><input type="checkbox" /> Reinforced </div>  |

*note: Answers need to be `checked` in the `<input/>` tag in source code, just edit it to be `<input ... checked/>`*

4. What is Gradient Descent? Do you know any other thing similar to it?
- machine learning optimization algorithm for finding the local minimam value of a differentiable function moslty the error\cost function.
	<ul style="list-style-type:disc;">
		<li>Decision tree.</li> 
		<li>SVM algorithm.</li> 
		<li>Naive Bayes algorithm.</li> 
		<li>KNN algorithm.</li> 
		<li>K-means.</li> 
		<li>Random forest algorithm.</li> 
	</ul>

5. You're approximating a function $f(x) = wx+b$, you have the data points $\textbf{x}$.
	1. What is $w$?
		- $w$ is a parameter\coefficient\weight of the model, it's one of the values we adjust to find the best fit for the data.<br> its's the slop of the line the model is trying to fit to the data
	2. What is $x$?
		- $x$ is the input feature
	3. What is $b$?
		- $b$ is a parameter\coefficient\weight of the model, it's one of the values we adjust to find the best fit for the data.<br>it is the value of $f(x)$ when $x = 0$ 
	4. Why is $\textbf{x}$ written in bold-face in the question, what does it mean?
		- becouse it represents all data points of $x$
	5. How are you planning to get the values of $w, b$?
		- I'm going to compute a cost function Mean Square Error $MSE(w, b)$ to calculate the error in values of $f_{w, b}(x)$ <br><br>
			$MSE(w, b) = \frac{1}{2m}\sum_{i = 1}^{m}(f_{w, b}(x^{(i)})-y^{(i)})^2$
		<br><br> to find the perfect fit I need to minimize this cost function $MSE(w, b)$ to achieve that I'll use the Gradient Descent.
		<br>
<br> <br>

6. $w:=w - \alpha \frac{1}{m}\sum_{i =1}^{m}(f_{w, b}(x^{(i)} )- y^{(i)}) x^{(i)}$
	1. What is $\alpha$?
		- $\alpha$ is the learning rate of the model, it take a value between $0$ and $1$, it determines how big do we want to change the value of $w$.
	2. What is $m$?
		- $m$ is the number of training feature samples
	3. What is $y$?
		- $y$ is the target values from the training set
	4. What does the summation compute?
		- the derivatitve of the cost function $MSE_{w,b}(x)$


## *Bonus* NumPy Questions

1. What does `np.cumsum` calculate?

2. What do `np.argmin` and `np.argmax` calculate?

3. How to rotate a matrix $90 ^{\circ}$?

4. What do `np.arange` and `np.newaxis` do?
	```
	data = np.arange(0, 5)
	column = data[:, np.newaxis]
	```

5. What's the difference between `np.flatten` and `np.ravel`?

6. 
	```py
	 A = np.linspace(0, 1, 11)
	 A[[0, 2, 4]]
	```
	
	```py
	A = np.linspace(0, 1, 11)
	A[0: 2: 4]
	```
	$\Rightarrow$ What does each return? And why?
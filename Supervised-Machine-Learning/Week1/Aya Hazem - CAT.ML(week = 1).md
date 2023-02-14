
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

	<table style="width:80%">
	<tr>
		<th>Supervised Learning</th>
		<th>Unsupervised Learning</th>
		<th>Semi-Supervised Learning</th>
		<th>Reinforced Learning</th>
	</tr>
	<tr>
		<td>-</td>
		<td>-</td>
		<td>-</td>
		<td><p> branch of ML that agents or bots to pick up actions that will maximize their rewards over time </p></td>
	</tr>
	<tr>
		<td>-</td>
		<td>-</td>
		<td>-</td>
		<td>-</td>
	</tr>
	<tr>
		<td>-</td>
		<td>-</td>
		<td>-</td>
		<td>-</td>
	</tr>
	</table>


3. Clustering is _______________ , and Classification is _______________ :

	|    Clustering    |  Classification  |
	|------------------|:---------------:|
	| <input type="checkbox" /> Supervised   |<div style="text-align: left"> <input type="checkbox"/> Supervised </div> |
	|<input type="checkbox" /> Unsupervised |<div style="text-align: left"><input type="checkbox" /> Unsupervised</div> |
	| <input type="checkbox" /> Reinforced   | <div style="text-align: left"><input type="checkbox" /> Reinforced </div>  |

*note: Answers need to be `checked` in the `<input/>` tag in source code, just edit it to be `<input ... checked/>`*

4. What is Gradient Descent? Do you know any other thing similar to it?

5. You're approximating a function $f(x) = wx+b$, you have the data points $\textbf{x}$.
	1. What is $w$?
	2. What is $x$?
	3. What is $b$?
	4. Why is $\textbf{x}$ written in bold-face in the question, what does it mean?
	5. How are you planning to get the values of $w, b$?

6. $w:=w - \alpha \frac{1}{m}\sum_{i =1}^{m}(f_{w, b}(x^{(i)} )- y^{(i)}) x^{(i)}$
	1. What is $\alpha$?
	2. What is $m$?
	3. What is $y$?
	4. What does the summation compute?


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
	```
	 A = np.linspace(0, 1, 11)
	 A[[0, 2, 4]]
	```
	
	```
	A = np.linspace(0, 1, 11)
	A[0: 2: 4]
	```
	$\Rightarrow$ What does each return? And why?
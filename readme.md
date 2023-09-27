This repo contains code for the report [Reliable Offline Pricing in eCommerce Decision-Making: A Distributionally Robust Viewpoint](). 

> Please direct all inquiries to Jie Wang @ jwang3163@gatech.edu.

# Code structure 
The basic process of generating the figures in the report is to run the python jupyer notebook in each directory to get experiment results together with scientifc plots. In the following, we provide brief description of each directory.

### Figure\_3\_generation
The jupyer notebook in this folder first provides linear regression coefficient estimate for response variables "COG", "FBA", and "reffee".

Next, it provides code for cross-validation procedure of tuning hyper-parameters $\epsilon$ and $\sigma^2$.

Finally, it generates profit estimation for the last 30 days of the given dataset. Figure 3 compares the estimated robust/optimistic profit versus the true profit.

### Figure\_4\_generation
The jupyer notebook in this folder first provides the estimation of expected customer demand for different choices of price with fixed competitor price 22.99$. 

Next, it visualizes the probability distribution of customer demand for four different prices: 17.49$, 19.49$, 21.49$, 23.49$. 

### Figure\_5\_generation/Pricing\_Week1.ipynb
This notebook first generates estimated "ADSPEND" and "comp\_1\_price" using time series prediction.

Next, it generates the profit estimation for Week1 testing phase for different choices of price. This generates the plot of Figure 5(a).

### Figure\_5\_generation/Pricing\_Week2.ipynb
This notebook follows the similar structure as in Pricing\_Week1.ipynb. It generates the plot of Figure 5(b).

Besides, it also provide the estimated profit versus true profit for the Week1 and Week2 testing phase. This corresponds to the plot of Figure 5(c).




# Dependencies
### python 3.6.10
- numpy                     1.19.1
- scikit-learn              0.23.2
- scipy                     1.3.1
- pandas 					     2.1.1


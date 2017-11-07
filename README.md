# SAMPLE DATA ANALYSIS SCRIPTS
## Demonstration of a scalable multi-Cloud application. Which will compute Value at Risk (VAR) for some well-known companies listed on stock markets.

#### Value At Risk (VAR): VAR is the calculation of risk of an investment. Resultant computations show how a given investment will climb or fall over some time span, with some given market conditions. Using the three VAR methods namely, historical, covariance and Monte Carlo.

#### 1) Historical: This is calculated by finding the return series, using the adjacent close of a given company. The next step is to sort the values from largest profit to the largest loss, taking the total number of data points we calculate the 95 and 99 percentages to attain the VAR at 95 and 95 percentages 

#### 2) Covariance: We compute the mean and standard deviation (stdev) to fit   the give formula with a set investment, where D is 1.65 at 95 and 2.33 at 99: −(𝑚𝑒𝑎𝑛 +(𝐷) ∗𝜎))∗𝐼𝑛𝑣𝑒𝑠𝑡𝑚𝑒𝑛𝑡 
 
#### 3) Monte Carlo: Having the mean and stdev from the previous step, we use the python function “random. Gauss” to generate random number (q).  ‘q’ is then used together with the most recent price of the adjacent close from a given company (p) to fit the formula: 𝑛 = (1 +𝑞)∗𝑝 The resultant n produces a new price list, which is run through the historical step to attain VAR at 95 and 99 percentages. 

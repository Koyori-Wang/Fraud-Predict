<h1>Data Challenge: Credit Card Fraud Transaction Prediction</h1>
<li>Xiaoyi Wang
  
<h2>Step 1: Load the data</h2>
<h4>The structure of the data</h4>
<li>786363 records
<li>29 fields
<h4>Basic Cleaning</h4>
<li>Drop the columns where values are all null
<li>Drop one ‘accountNumber’ and ‘customerId’ because these two columns are just the same

<h2>Step 2: Plot</h2>
<li>The histogram of transaction amount
<li>The sum of transaction amount everyday
<li>The amount and time distribution of fraud transactions
<li>Correlation between features
<li>The number of transaction in each category

<h2>Step 3: Data Wrangling - Duplicate Transactions</h2>
<h4>Reversed type</h4>
<li>There are a pair of transaction. One of the transaction type is REVERSAL and the other is PURCHASE
<li>The purchase one occurred before the reversal one
<li>They have same customer id, transaction amount, merchant name, card last 4 digit
<h4>Multi-swipe type</h4>
<li>There are more than 1 transaction. The transaction type is all PURCHASE
<li>All transactions happen in 1 hour
<li>They have same customer id, merchant name, card last 4 digit

<h2>Step 4: Model</h2>
<h4>Data cleaning</h4>
<li>Convert the datetime columns to int
<li>Convert categorical columns to dummy variables
<li>Add some Columns may releted to the fraud transaction

<h4>Sampling</h4>
<li>Use Random Over Sampling to deal with the imbalance

<h4>Feature Selection based on feature importance</h4>
<li>Select the most important 25 features

<h4>Modeling</h4>
<li>Decision Tree
<li>Random Forest
<li>Gradient Boosting


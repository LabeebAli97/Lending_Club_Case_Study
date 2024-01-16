# Project Name
> Lending Club Case Study


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

### Project Information

> The project is a data science project that uses the lending club data set to predict whether a loan will be defaulted or not.

### Project Background

> This company is the largest **online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures**. Borrowers can easily access lower interest rate loans through a fast online interface. Like most other lending companies, lending loans to **‘risky’** applicants is the largest source of financial loss (called credit loss). **Credit loss** is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

### Project Statement

> The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

### Data Set

> The data set is a csv file with the loan data for the Lending Club.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Results from Univariate Analysis:
  
  1. Majority of the Loan Amount Requested/Sanctioned falls between 2500 - 10000 range.
  2. 85.4% of the loans approved was Fully Paid and a 14.6% of loans was defaulted.
  3. Around 22% of the total loan are taken by people who had 10+ Years of employee length, indicating that people tend to take loans more on a later stage of life.
  4. The loan issued increases drastically year by year, 2011 has over 50% of the all issued loans. This can be due to several reasons.
		- Life Getting Tougher Over Years
		- Recession in 2011
		- LC became popular over years
  6. dti vs loan_status --> 
	    - From dti vs Loan Status analysis, binned in 2 different methods Equal Width Binning and Quantile Binning show almost similar patterns, that as the dti increases chances of defaulting also increases
  7. funded_to_income vs loan_status -->
		- Similar analysis was made from the relationship btw funded_to_income vs loan_status, binned in 2 different methods Equal Width Binning and Quantile Binning.
		- From the analysis of 2 binning methods one can conclude that as the funded_to_income increases chances of defaulting also increases
		- From the plot generated using Equal Width Binning for funded_to_income vs loan_status, its clear that almost 31.1% of loans defaulted whose funded_to_income ratio was above 0.52
		- Loan Status vs Funded To Income Ratio, the Box plot gives a slight indication that most of the defaulters fall on a high f_to_i ratio value, whereas the majority of the Fully Paid is on the lower ratio end

- Results from Bivariate Analysis:
  
  1. Loan Status vs Interest Rate
		- Loan Status vs Interest Rate Box plot gives a strong indication that most of the defaulters tend to fall on higher interest rates when compared to non-defaulters.  
		- The Percentage of Defaulters Under Each Category WRT Grade bar plot gives a clear conclusion/insight that the higher the grade at which the loans are taken, the more the chance of defaulting. 
		- Around 36% of the loan takers under G category has defaulted
		- Grade/Sub Grade is linked to Interest rate, The Higher the grade higher the interest rate

  2. Term vs loan_status
		- People who opted for longer duration installments i.e. 60 months are going to default more, than people who opted for shorter duration i.e. 36 months
		- From Term vs Loan Status Analysis, it’s clear that out of 8722 who opted for 60 Months as term 2230 has defaulted, which means around 25.6 %, whereas, for those who opted 36 Months only 2966 out of 26953 defaulted, that’s just 11%

  3. Purpose vs loan_status
		- From Purpose vs Loan_status analysis, it’s clear that 27.8% of loans taken for small_business end up as defaulters. This might be because of the failure of the business.
		- Another insight is that loans taken under 60 months as term and purpose as educational and small_business show very high default rates of about 42%

  4. Annual Income vs Loans Defaulted In that segment in Percentage
		- From Annual Income vs Loan Status analysis, it was found that as annual_inc decreases chances of defaulting increases

  5. Funded Amount By Investors vs Loans Defaulted In that segment in Percentage
		- From Funded_amnt_inv vs loan_status analysis, it was found that as the funded amount by investors increases chances of defaulting increases

  6. Record of Bankruptcies vs Loans Defaulted In that segment in Percentage
		- pub_rec_bankruptcies vs percentage of defaulters shows an indication that people having previous records of bankruptcies tend to repeat that in the future.
		- Around 40% of those who take loans with a history of bankruptcies of 2 tend to default. 

  7. Difference of Funded Amount and Funded amount by investors vs Loans Defaulted In that segment in Percentage
		- Analyzing the relationship btw the difference of funded_amnt and funded_amnt_inv, and the Percentage of defaulters in each segment, binned using the Equal Width Binning technique shows a very interesting analysis.
		- So if the difference btw the approved amount from LC and the amount funded by investors increases, means the tendency for that loan to default is very high
		- For loans that had a difference in approved amount from LC and amount funded by investors greater than 21.6K, around 46.5% of such loans were defaulted


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Pandas - version 1.3.4
- NumPy - version 1.20.3
- Seaborn - version 0.11.2
- MatplotLib - version 3.4.3
- Plotly - version 5.7.0


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project was inspired by UpGrad IITB Programme as a case study for the Machine Learning and Artificial Intelligence course.

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->
<!-- You don't have to include all sections - just the one's relevant to your project -->

## Contributors:

* [Labeeb Ali Koleth](https://github.com/LabeebAli97)
* [Akankshya Abhilipsa](https://github.com/Aabhilipsa)

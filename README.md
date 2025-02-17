# DSN
<h3>Introduction</h3>

<h4>This is a competition hosted by Data Science Nigeria as part of prerequisite for it's all-expenses-paid learning bootcamp. 
<h4>Hosted on Zindi https://zindi.africa/hackathons/dsn-ai-bootcamp-qualification-hackathon/'
<h4>Competition Score: 0.844648358439733
<h3>Problem Statement</h3>
<p>Kowope Mart is a Nigerian-based retail company with a vision to provide quality goods, education and automobile services to its customers at affordable price and reduce if not eradicate charges on card payments and increase customer satisfaction with credit rewards that can be used within the Mall. To achieve this, the company has partnered with DSBank on co-branded credit card with additional functionality such that customers can request for loan, pay for goods even with zero-balance and then pay back within an agreed period of time. This innovative strategy has increased sales for the company. However, there has been recent cases of credit defaults and Kowope Mart will like to have a system that profiles customers who are worthy of the card with minimum if not zero risk of defaulting.</p>

<h4>Objective</h4> To predict customers who are likely to default or not.
<h4>Model Used</h4> Catboost classifier
<h4>Evauation Metric</h4> Area under the ROC Curve(AUC)

<h3>Variable Definitions</h3>
<ul>
    <li> Application_ID: Unique Customer Application Identification number </li>

<strong>Risk Scoring features:</strong>
    <li>form_field1: Customer Creditworthiness score based on historical data</li>
    <li>form_field2: A score that measures the number and riskiness of credit enquiries made by a borrower.</li>
    
<strong>Severity features:</strong> Severity is a function of amount, time since default, and number of defaults
    <li>form_field3: Severity of default by the borrower on any loan(s).</li>
    <li>form_field4: Severity of default by the borrower on auto loan(s).</li>
    <li>form_field5: Severity of default by the borrower on education loan(s).</li>

<strong>Credit features</strong>

   <li>form_field6: Minimum of credit available on all credit cards that is automatically renewed as debts are paid off on the
    customer’s cards (in NGN)</li>
    <li>form_field7: Maximum of credit available on customer’s active credit lines (in NGN)</li>
    <li>form_field8: Maximum of credit available on all active credit cards that is automatically renewed as debts are paid off
    on the customer’s cards (in NGN)</li>
    <li>form_field9: Sum of available credit on credit cards that the borrower has missed 1 payment (in NGN)</li>
    <li>form_field10: Total amount of credit available on accepted credit lines (in NGN)
    <li>form_field11: The amount of dues collected post-default where the due amount was more than 500 (in NGN)</li>
    <li>form_field12: Sum of the amount due on active credit cards (in NGN)</li>
    <li>form_field13: Annual amount paid towards all credit cards during the previous year (in NGN)</li>
    <li>form_field14: Annual income (in NGN)</li>
    <li>form_field15: The estimated market value of a property owned/used by the borrower (in NGN)</li>

<strong>Credit card features:</strong>
    <li>form_field16: Number of active credit card that is automatically renewed as debts are paid off on which full credit
    limit is utilized by the borrower</li>
    <li>form_field17: Number of active credit cards on which full credit limit is utilized by the borrower</li>
    <li>form_field18: Number of active credit lines on which full credit limit is utilized by the borrower</li>
    <li>form_field19: Number of active credit cards on which at least 75% credit limit is utilized by the borrower</li>
    <li>form_field20: Number of active credit lines on which at least 75% credit limit is utilized by the borrower</li>
    <li>form_field21: Average utilization of active revolving credit card loans (%)</li>
    <li>form_field22: Average utilization of line on all active credit lines activated in last 2 years (%)</li>
    <li>form_field23: Average utilization of line on all active credit cards activated in last 1 year (%)</li>
    <li>form_field24: Average utilization of line on credit cards on which the borrower has missed 1 payment during the last 6 months (%)</li>
    <li>form_field25: Average tenure of active revolving credit cards (in days)</li>
    <li>form_field26: Tenure of oldest credit card among all active credit cards (in days)</li>
    <li>form_field27: Tenure of oldest revolving credit card among all active revolving credit cards (in days)</li>

<strong>Time-related features</strong>
    <li>form_field28: Number of days since last missed payment on any credit line</li>
    <li>form_field29: Tenure of the oldest credit line (in days)</li>
    form_field30: Maximum tenure on all auto loans (in days)</li>
    <li>form_field31: Maximum tenure on all education loans (in days)</li>
    <li>form_field32: Sum of tenures (in months) of active credit cards</li>
    <li>form_field33: Sum of tenures (in months) of active credit cards</li>
    <li>form_field34: Number of active credit lines over the last 6 months on which the borrower has missed 1 payment</li>
    <li>form_field35: Number of revolving credit cards over the last 2 years on which the borrower has missed 1 payment</li>
    <li>form_field36: Number of active credit lines</li>
    <li>form_field37: Number of credit cards with an active tenure of at least 2 years</li>
    <li>form_field38: Number of credit lines activated in the last 2 years</li>
    <li>form_field39: Number of credit lines on which the borrower has current delinquency</li>

<strong>Percentage related features</strong>
    <li>form_field40: Utilization of line on active education loans (%)</li>
    <li>form_field41: Utilization of line on active auto loans (%)</li>

<strong>Other features</strong>
    <li>form_field42: Financial stress index of the borrower. This index is a function of collection trades, bankruptcies files, tax liens invoked, etc.</li>
    <li>form_field43: Number of credit lines on which the borrower has never missed a payment in the last 2 years, yet considered as high-risk loans based on the market prediction of the economic scenario</li>
    <li>form_field44: Ratio of the maximum amount due on all active credit lines and the sum of amounts due on all active credit lines</li>
    <li>form_field45: Number of mortgage loans on which the borrower has missed 2 payments</li>
    <li>form_field46: Number of auto loans on which the borrower has missed 2 payments</li>
    <li>form_field47: Type of product that the applicant applied for. (C = Charge; L = Lending)</li>
    <li>form_field48: Undefined Variable</li>
    <li>form_field49: Undefined Variable</li>
    <li>form_field50: Ratio of the minimum amount due on all active credit lines and the sum of amounts due on all active credit lines</li>

<strong>Target features</strong>
    <li>default_status: defaulted or not. (yes:1, no: 0)</li>
</ul>

# Market Analysis in Banking Domain

## Background & Objective

Your, client a portuguese banking institution, ran a marketing campaign to convince potential customers to invest in a back term deposit scheme.
The marketing campaigns were based on phone calls. Often, the same customers were contacted more that ones through phone, in order to assess if they would want to subscribe to the bank term deposit or not. You have to perform the market analysis of the data generated by this campaign.

## Domain

Banking (Market Analysis)

## Dataset description

1. **age:** age of potential customer (numeric)
2. **job:** type of job (categorical; admin, blue-collar, entrepreneur, housemaid, management, retired, self-employed, services, student, technician, unemployed, unknown)
3. **martial:** marital status (categorical; divorced, married, single, unknown; note: divorced -> divorced or widowed)
4. **education:** educational background (categorical; basic.4y, basic.6y, basic.9y, high.school, illiterate, professional.course, university.degree, unknown)
5. **default:** has credit in default? (categorical; no, yes, unknown)
6. **housing:** has housing loan? (categorical; no, yes, unknown)
7. **loan:** has personal loan? (categocial: no, yes, unknown)

**Related to last contact of current campaign**

8. **contact:** contact communication type (categorical; cellular, telephone)
9. **month:** month of last contact (categorical; jan, feb, mar, ..., dec)
10. **day_of_week:** last contact day of the week (categorical; mon, tue, wed, thu, fri)
11. **duration:** last contact duration in seconds (numeric; note: this attribute highly effects the output target (eg. if duration=0 then y='no'). Yet the duration is not known before a call is performed. Also, after the end of the call 'y' is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

**Other attributes**

12. **campaign:** number of times a customer was contacted during the campaign (numeric; note: includes last contact)
13. **pdays:** number of days passed after the customer was last contacted from a previous campaign (numeric; 999 means customer was not previously contacted)
14. **previous:** number of times the customer was contacted prior to or before this campaign (numeric)
15. **poutcome:** outcome of the previous marketing campaign (categorical; failure, nonexistent, success)

**Target variable**

16. **y:** has the customer subscribed a term deposit? (categorical; yes, no)

## Analysis tasks

1. Load the data and create a Spark data frame.
2. Give marketing success rate (No. of people subscribe / total no. of entries)
    - Give marketing failure rate
3. Give the maximum, minimum and average age of targeted customer.
4. Check the quality of customers by checking average balance, median balance of customers.
5. Check if age matters in marketing subscription for deposit.
6. Check if marital status mattered for a subscription to deposit scheme.
7. Check if age and marital status together mattered for a subscription to deposit scheme.
8. Do feature engineering for the back and find the right age effect on the campaign.

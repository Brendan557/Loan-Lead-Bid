# Loan-Lead-Bid

This project deals with leads and bids for loans. Each lead that is available can be bid in for $3, $35, $50, or $75. Bidding on a lead does not mean that the lead is won. The lower the bid price the less likely it is for the bid to be won. Once a lead is won it can be attempted to convert the lead into a loan.  I am going to use the lead data to develop a model for deciding which leads should be bid on and how much. The bid amounts again are limited to $3, $35, $50, or $75. 


Fields

BidPrice: If this is populated, then we bid this price for this lead
AcceptedBid: This will tell you if the bid was accepted (we “won” the bid)
ExpectedRevenue: This is the amount of revenue we expect to get from the lead if it turns into a
loan. 

Three things need to happen for us to get any revenue:
1. We need to bid
2. We need to win the bid
3. We need to convert the lead into a loan
ExpectedConversion: This is the expected conversion rate of lead into loan.

Example
Let’s say we bid on 20 leads. For simplicity, let’s say we bid $50 on each, and that all 20 are exactly the
same:
ExpectedRevenue: $150 
ExpectedConversion: 0.4

Let’s also say we win 10 of these bids and lose 10.
The 10 bids we lost have no revenue or costs.
The 10 bids we won cost $50 each – so $500 total cost.
They each have an expected revenue of $150, and they each have an expected conversion of 40%.
10 Leads * 40% Conversion = 4 Loans
4 Loans * $150 Revenue = $600 Total Revenue
So for this example, we have $600 in total revenue, and $500 in costs – so we have a net revenue of
$100.

# ETF Investing and Index Replication / Tracking

## Index Tracking with Optimization (Part 1) - The S&P 500 Constituents

__Objectives__:

1. Find a portfolio that tracks the S&P best with just 50 stocks.
   - The S&P has 500 stocks and we want to reduce trading costs.
  
2. Find the optimal number of stocks to track the S%P efficiently

Optimal will be around 100-150. Let's take 110! The less we track the lower our rebalancing costs!

  <img width="880" alt="image" src="https://github.com/user-attachments/assets/72be504b-5590-4d00-a899-719da4971e29">


__Method__:

1. Use Optimizer through making simulated portfolios
   - This optimization makes 1000 different, simulated portfolios using random 50 stocks from the S&P
   - These simulated portfolios are weighted by market cap.
   - We will use the portfolio that has the lowest tracking error

2. Chart out the average tracking error for each portfolio size (ranging from 0-500). The method of contructing these portfolios are the same as what was mentioned above!

Tracking error (In sample from 2019-2021 at 2.9%)

<img width="826" alt="image" src="https://github.com/user-attachments/assets/0782b084-6a41-4c14-8bd3-ade08bc57049">

Tracking error (Out sample from 2021-2023 at 3.9%)

<img width="872" alt="image" src="https://github.com/user-attachments/assets/bab41833-2a1e-407d-97fb-5f628286ba39">

   
__Key Learnings from this Project__:

1. Average tracking error for all 1000 simulations was at 7.57%. This was if we were to take just 50 stocks (from 2019 till date)
2. Marginal benefit significantly decreases past the 110 sample mark as could be seen in the graph. Therefore, we can optimally track the S&P500 with about 110 stocks, with an average tracking error of 3.67% (outsample), 2.9% for insample!

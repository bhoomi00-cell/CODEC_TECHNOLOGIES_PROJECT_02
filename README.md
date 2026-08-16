Market Basket Analysis

Goal: Identify product associations in transaction data to improve cross-selling opportunities.

Overview:-
This project analyzes 14,963 grocery shopping transactions to find which products are frequently bought together, using the Apriori algorithm. It goes beyond simple co-occurrence by using lift to distinguish genuine product associations from combinations that only look common because individual items are popular.

Approach:-
- Python: Converted raw purchase records into transaction baskets, applied Apriori to mine frequent itemsets, then generated association rules (support, confidence, lift)
- Visualization: Charted the most frequent items and the top product associations by lift

Key Findings:-
- Sausage and bottled beer show the strongest genuine association (lift 1.22) — the top cross-sell opportunity in the data
- Frankfurter and other vegetables (lift 1.12) and sausage and yogurt (lift 1.11) are the next strongest pairings
- Whole milk appears in nearly every basket due to sheer popularity, not because of a meaningful product relationship — high support alone doesn't mean a real association

Tech Stack:-
Python (pandas, mlxtend, matplotlib), Jupyter Notebook

Files:-
- Groceries_dataset.csv — raw transaction data
- market_basket_analysis.ipynb — full pipeline (transaction building, Apriori, association rules, visualization)
- Market_Basket_Insights.pptx — findings and recommendations

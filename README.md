📊 **Food Marketing Data Analysis — Full Project Description**

📘 **Project Overview** DONE

This project analyzes customer behavior for a food retail/marketing company using historical customer and campaign data. The goal is to understand who spends the most, who is most likely to accept marketing campaigns, and which channels (web, catalog, in-store) are most effective.
Using Python and exploratory data analysis, you engineered key features (e.g., Age_Group, Total_Children, Education_Status, Marital_Status_str, MntTotal) and visualized relationships between:
- Demographics (age, marital status, children, education) DONE
- Purchase behavior (web, catalog, store purchases) DONE
- Total spending (MntTotal) DONE
- Campaign response (Accepted_Campaigns) DONE

From these insights, you define practical customer segments and marketing recommendations to maximize revenue and campaign ROI.

🎯 **Business Problem** DONE

The business needs to answer:
- **Which customers generate the most revenue?**  
  (Middle-aged customers (around 31–70 years old), especially those with few or no children, generate the most revenue.)
- **Which customers are most likely to respond to marketing campaigns?**  
  (Younger adults (23–30) and older customers (71+) are the most likely to respond to campaigns.)
- **Which channels (web, catalog, store) should we prioritize for marketing efforts?**  
  (Campaign efforts should prioritize the catalog channel for higher acceptance and the store/web channels for higher spending volume.)
- **How should we segment customers to target campaigns more effectively?**  
  (Segment customers by age group, number of children, and shopping channel behavior to target high-spending clusters differently from high-response clusters.)

Essentially: How can we best allocate marketing budget across customer segments and channels to maximize profit and new spend?

🛠 **Tech Stack** DONE

- Language: Python
- Environment: Jupyter Notebook

**Libraries:** DONE

- pandas – data loading, cleaning, feature engineering
- seaborn – statistical visualizations (heatmaps, barplots, regplots, jointplots)
- matplotlib – plot formatting and titles

**Analysis & Insights by Graph** DONE

Below I walk through the graphs in the notebook and summarize what each one is telling you, plus likely cause–effect interpretations (with the caveat that the data is observational, so we’re inferring plausible business drivers, not proving strict causality).

1. Correlation Heatmaps DONE
- Insight: The full correlation heatmap shows how numerical variables move together (spending, purchases, demographics, campaign acceptance).
- Cause & Effect (interpretation): Higher purchase activity (more web/catalog/store purchases) likely contributes to higher total spend (MntTotal).Demographics alone are not strong direct drivers; instead, behavioral factors (how customers shop) better explain revenue and campaign response.

2. Barplot of percentage of accepted campaigns per age group. Age vs Campaign Acceptance DONE
- Core age audience (31–70): Represent a large share of customers. Less likely to accept campaigns compared to the very young and very old.
- Young adults (23–30) and older customers (71+): Higher campaign acceptance rates.

Insights: DONE
- Age is influencing both spend and willingness to engage:
  31–70 may already be loyal, habitual shoppers; campaigns may not significantly change their behavior (low marginal effect on acceptance).

- Younger (23–30) and older (71+) customers:  
  These groups might be more price-sensitive or more attentive to offers, so campaigns have a stronger impact on their behavior.
  
Business implication: DONE
- Use 31–70 as your core revenue base but recognize they are less responsive; think loyalty benefits and retention, not aggressive discounting.
- Provide tailored and persuasive promotions to customers aged 23–30 and 71+, as these segments are more responsive to marketing and can be more effectively encouraged to increase or resume spending.

3. Barplot of Age vs Spending (All Customers vs Campaign Acceptors) DONE

Insights: DONE
- 30–70 spend the most money overall.
- Among campaign acceptors, the spending pattern still favors the middle-aged groups.
- Younger and older groups accept campaigns more frequently, but their absolute spend level is lower.
- Being in the 30–70 range is causing higher baseline consumption (likely due to higher incomes, stable households).
- Campaigns do not dramatically increase acceptance rates in these high-spend groups but can nudge additional spend.
- For younger and older customers, campaigns are more effective in changing behavior, even if their base spend is smaller.

Business implication: DONE
- For growth and new spend, focus on high-acceptance age bands at the edges (23–30, 71+).














## Travel Insurances Prediction Model

This is a machine learning model to predict if a passenger will claim for travel insurance or not. 
Travel insurance is a type of insurance that provides protection as long as we travel both domestically and abroad. Several countries have even required travelers to have travel insurance, for example, countries in Europe and America. The amount of premium depends on the coverage desired, the length of the trip, and the purpose of the trip. A company engaged in travel insurance wants to know the policyholder who will submit an insurance claim for coverage. Policyholder data at insurance companies is historical data consisting of destinations, insurance products, and so on.

Contents:
1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

### **Business Problem Understanding**
Dataset https://drive.google.com/drive/folders/1iVx5k6tWglqfHb05o0DElg8JHg7VVG_J

**Context**

Travel insurance provides financial protection against unexpected events and losses that can occur while traveling. It can cover a range of scenarios, including medical emergencies, trip cancellations, lost or stolen belongings, and travel delays. Essentially, it helps mitigate financial risks associated with travel. 

A survey of 500 passengers in Singapore in 2023 (source: https://ancileo.com/singapore-consumers-travel-insurance-needs/) found that 68% of the 500 respondents are willing to purchase travel insurance plans for their trips in 2023.
Several factors that make them want to purchase travel insurance plans are: 

#1: Price And Ease Of Online Claims Emerge As Top Purchase Considerations
Pricing was identified as the most important consideration among travelers when purchasing travel insurance plans. Ease of online claims is also a crucial factor for many, as it enables them to make claims quickly and easily without the need for physical documents or lengthy processes. 

#2: Covid-19 Coverage Remains A Priority For Family Travelers
Although COVID-19 benefits were a significant consideration for trip insurance purchases in 2022, it is no longer a top priority for most travelers in 2023. However, family travelers still see it as a crucial factor, given that the pandemic has heightened awareness of the risks associated with travel and the necessity of having coverage for unforeseen circumstances. 

#3: Personalization Of Travel Insurance Plans Are More Important For Generation Y Travelers
Generation Y travelers (26-41 y/o) place more emphasis on personalization of travel insurance plans compared to other age groups. This could be due to their greater familiarity and comfort with technology, which has enabled them to access personalized insurance products and services.

#4: Price Sensitivity Higher Among Younger Travelers
Younger travelers (Generations Y and Z, 19-41 y/o) are more price sensitive than the rest of the age groups. This suggests that insurers may need to offer more affordable and flexible plans that cater to the needs and preferences of this demographic. By taking these factors into account, insurers can better meet the evolving needs and expectations of travelers and ensure that they have the right coverage for their travel plans.

This survey also shows some challenges in purchasing travel insurances, such as:
Challenge #1: Policy Exclusions
Policy exclusions are a common challenge for many travelers, especially for those in the Generation X age group (42-56 y/o). They highlighted limitations in policy coverage the most compared to other age groups.

Challenge #2: Lack Of Transparency
Another notable challenge is insurers’ lack of transparency, making it difficult for travelers to understand their coverage. This can lead to confusion and frustration, especially for those prioritizing trip interruption coverage who often struggle to obtain necessary information.

Challenge #3: Difficulty In Filing Online Claims
Travelers who prioritize ease of online claims service, as well as those who prioritize trip cancellation coverage, face limitations in policy coverage and difficulty in filing online claims. This highlights the need for insurers to provide more comprehensive and transparent coverage and make their claim management system more user-friendly and streamlined to reduce the burden on travelers.

**Problem Statement**

One of the biggest challenge for travel insurances company is the claiming process of travel insurance. Most of the consumer don't read the term and conditions, what is covered and what is not. The other problem is the claiming process that too long can make consumer angry and disatisfied. 

**Benefits of Analysis**
1. reduce financial risk
2. determine which products are most popular
3. increase customer satisfaction
4. determine promotional targets

**Goals**
Generating ML models to predict whether consumers will make a claim or not so as to speed up the claims process and increase consumer satisfaction.

**Analytic Approach**
Claim Prediction (Binary Classification) to predict if a policy will result in a claim (Yes/No).

**Metric Evaluation**
The evaluation metrics to be used are Precission, Recall, F1 Score and AUC-ROC. Precission is to measures false claim alerts (costly for insurers). Recall is to captures actual claims missed (risky if underpredicted). F1 Score is to balances precision/recall (which is critical for imbalanced data). AUC-ROC is to evaluates model’s ranking ability (higher = better discrimination).

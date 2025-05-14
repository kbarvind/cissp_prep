# Six Elements of Quantitative Risk Analysis

1. **Asset Value (AV)**  
   - The monetary value of an asset (e.g., data, hardware, intellectual property).  
   - Represents what you're trying to protect.

2. **Exposure Factor (EF)**  
   - The percentage of asset loss if a specific threat occurs.  
   - Expressed as a decimal (e.g., 0.4 for 40%).

3. **Single Loss Expectancy (SLE)**  
   - The expected monetary loss every time a risk event occurs once.  
   - **Formula:** `SLE = AV × EF`

4. **Annualized Rate of Occurrence (ARO)**  
   - The estimated frequency with which a threat is expected to occur annually.  
   - Based on historical data, expert judgment, or statistics.

5. **Annualized Loss Expectancy (ALE)**  
   - The expected yearly loss from a specific risk.  
   - **Formula:** `ALE = SLE × ARO`

6. **Cost-Benefit Analysis (CBA)**  
   - Compares the cost of implementing a security control with the expected reduction in risk.  
   - Helps determine if a control is worth the investment.  
   - **Formula:** `CBA = (ALE before - ALE after) - Cost of control`


## **Risk Formula**
   `ALE = SLE (AV x EF) x ARO`

**Key points**:
- EF should be in decimals
- ARO should be converted to 1 year

---
**Problem**

Office Building = $1,000,000

Hurricane damage estimate = 50% = 0.5

SLE = AV x EF = $1,000,000 x 0.5 = 5,00,000

Hurricane probability is once in 10 years = 1 time/ 10 years =0.1

possible questions:
 - if hurricane occurs 2 times in 1 year = 2/1 = 2

Company buys an $50000 insurance policy to cover risk of loss. The policy has $7500 dedcuctible 

The insurance policy costs $10000 per year

```
AV = $1,00,000
EF = 0.5
SLE = AV x EF = 500000
ARO = (1/10) = 0.1
ALE = SLE x ARO = 500000 x 0.1 = $50000
```

`Total Risk(ALE) - Control gap = Residual Risk`

Control gap = Insurance - deductible = $50000-$7500=$42500

$50000 - $42500 = $7500(Residual Risk)


```Safegaurd Evaluation = (ALE1(Before) - ALE2(After)) - Annaul Cost of Safegaurd(ACS)```

ALE1 = $50000

ALE2 = $7500

ACS(Insuarance policy) = $10,000

Safeguard Evaluation = $50,000 - $7500 - $10,000 = $32,500

SE > $0 for good financial decision


---
You are evaluating the benefit of a safeguard to a specific threat. The asset is a customer database, which is estimated to be worth $10 million. The threat is an intrusion that could cause a 50 percent value loss. The attack has already been attempted three times in the last 6 months. The best countermeasure would be able to reduce the success rate to only once per year, but the cost of the protection is $350,000.

What is the benefit of this countermeasure?


The benefit of this countermeasure is $24,650,000. 

This is calculated by first establishing the pre-countermeasure annualized loss expectancy (ALE1). 
From the scenario, we know that the asset value (AV) =$10,000,000 and the exposure factor (EF) = 50%, so the single loss expectancy (SLE) = AV * EF = $5,000,000. The ARO = 6/year (3 times in six months is 6 times per year). Thus, ALE1 = SLE * ARO = $30,000,000. The post-countermeasure ARO=1/year, so the ALE2 is = $5,000,000. The annual cost of the countermeasure/safeguard (ACS) is $350,000. Thus, the cost benefit is [ALE1 – ALE2] – ACS = $24,650,000. 

---

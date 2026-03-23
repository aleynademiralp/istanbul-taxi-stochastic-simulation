# Istanbul Taxi Distribution: A Stochastic Simulation Analysis

## Objective
This project models the imbalances in Istanbul's taxi distribution using stochastic processes, Markov Chains, and Monte Carlo simulations in **Julia**. The goal is to mathematically prove why certain districts suffer from taxi shortages and how urban traffic crises affect long-term mobility.

## Tools & Technologies
* **Language:** Julia
* **Methods:** Monte Carlo Simulation, Inverse Transform Method, Transition Matrices, Stationary Distribution Calculation

## Hypotheses Tested
1. **Unbalanced Accumulation:** Do taxis naturally pool in central districts (e.g., Şişli, Beşiktaş) while leaving distant districts (e.g., Beylikdüzü) empty due to transition probabilities?
2. **Return Time (The "Black Hole" Effect):** How many trips does it take on average for a taxi to return to a distant district like Beylikdüzü once it leaves?
3. **Traffic Trap (Crisis Scenario):** If cross-continent bridge traffic reduces transition probabilities between Europe and Asia by 80%, how does the stationary distribution of taxis change?

## Key Findings
* **Severe Imbalance:** The simulation proved that without external intervention, taxis naturally accumulate in Şişli and Beşiktaş (over 30% supply vs. 20% demand), leaving Beylikdüzü in a "Crisis" state with near-zero availability (3% supply vs. 25% demand).
* **The Transit Desert:** A taxi leaving Beylikdüzü takes an average of **27.0 trips** to return, mathematically confirming the district's severe shortage.
* **Bridge Traffic Impact:** Imposing an 80% penalty on cross-continent transitions acts as a "Traffic Trap," effectively trapping taxis on the European side and starving the Asian side (Kadıköy, Ümraniye).

# Introduction

> **Part:** Introduction · **Status:** Not started
>
> [Read the introduction online](https://mlsysbook.ai/vol1/introduction/introduction.html)

## Key ideas
Based on The Bitter Lesson (Sutton 2019), using more computing is more effective than relying on humans for improving the system.

Machine learning system is about data + algorithm + machine (DAM)
![[img/Pasted image 20260921114853.png]]

Time and energy are factors to consider for training systems. Minimising avoidable data movement can improve both speed and energy efficiency.

It is about balancing edge + cloud computing.
Depends on how it is served, based on strictly set requirements.

 The architectural foundation of ML systems engineering organized into five core disciplines: Data Engineering, Training Systems (Model Training), Deployment Infrastructure (Model Deployment), Operations & Monitoring (Operation & Maintenance), and Ethics & Governance, supported by foundational efficiency, evaluation, and reliability practices.
## Mental models / intuition
A frequent misconception is that AI engineering is just “software engineering for ML.” The system specification is instead probabilistic. An ML system’s output is statistically valid or invalid relative to a shifting distribution, not correct or incorrect relative to a fixed deterministic contract.

## Important equations
$T = \underbrace{\frac{D_{\text{vol}}}{\text{BW}}}_{\text{The Data Term}} + \underbrace{\frac{O}{R_{\text{peak}} \cdot \eta_{\text{hw}}}}_{\text{The Compute Term}} + \underbrace{L_{\text{lat}}}_{\text{The Latency Term}}$
The iron law

$\text{Accuracy}(t) \approx \text{Accuracy}_0 - \lambda \cdot \mathcal{D}(P_t \lVert P_0)$
Degration equation

$\text{RoC} = \frac{\Delta \text{Accuracy}}{\Delta \text{Compute Cost}}$
**Return on compute (RoC)** measures the incremental accuracy gain per added dollar of infrastructure investmentIf the RoC is negative or negligible, the system is over-engineered, regardless of its technical sophistication. This economic lens transforms “accuracy” from a research target into an engineering budget.

## Trade-offs
### Roofline model: Tradeoff between compute and bandwidth
Helps when considering batch size
![[img/Pasted image 20260914143627.png|610]]

## Things I don't understand yet

## Review questions
1. A medical-imaging team has severely limited access to labeled data (a few thousand radiographs per class) but adequate GPU capacity. According to the efficiency framework, which dimension should they prioritize first?
    1. Compute efficiency, because better accelerator utilization indirectly produces more labels
    2. Latency optimization, because lower inference latency reduces distribution drift
    3. Serving optimization, because efficient serving removes the need for more training data
    4. Data selection, because it extracts more learning value from each scarce labeled sample
	A medical-imaging team has severely limited access to labeled data (a few thousand radiographs per class) but adequate GPU capacity. According to the efficiency framework, which dimension should they prioritize first?



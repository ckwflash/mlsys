# Introduction

> **Part:** Introduction · **Status:** Not started
>
> [Read the introduction online](https://mlsysbook.ai/vol1/introduction/introduction.html)

## Key ideas
Based on The Bitter Lesson (Sutton 2019), using more computing is more effective than relying on humans for improving the system.

Machine learning system is about data + algorithm + machine (DAM)
![[Pasted image 20260907174519.png|566]]

Time and energy are factors to consider for training systems. Minimising avoidable data movement can improve both speed and energy efficiency.
## Mental models / intuition


## Important equations
$\text{RoC} = \frac{\Delta \text{Accuracy}}{\Delta \text{Compute Cost}}$
**Return on compute (RoC)** measures the incremental accuracy gain per added dollar of infrastructure investmentIf the RoC is negative or negligible, the system is over-engineered, regardless of its technical sophistication. This economic lens transforms “accuracy” from a research target into an engineering budget.

## Trade-offs
### Roofline model: Tradeoff between compute and bandwidth
Helps when considering batch size
![[Pasted image 20260914143627.png|610]]

## Things I don't understand yet

## Review questions


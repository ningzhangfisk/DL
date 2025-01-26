+ Why optimization fails?
  - local optimal
  - saddle point
+ Solution 1: adjust learning rate
  - adaptive learning rate
  - scheduled learning rate
+ Solution 2: Batch Norm

# 1. local optimal and saddle point
## 1.1 critical points
+ both are called critical points
+ derivates are 0.

![](https://www.offconvex.org/assets/saddle/minmaxsaddle.png)

+ When reaching a local optimal, it is already the lowest point in that area, we can not move.
+ But when reaching a saddle point, we can still go some direction to get a lower cost.

## 1.2 how to find the critical point is local optimal or saddle point?
+ Plotting, but impossible due to the complexity of the loss function/model
+ Tayler series approximation

$
L(\theta)  \approx L(\theta^\prime)  + (\theta - \theta^\prime)^Tg + \dfrac{1}{2}(\theta - \theta^\prime)^T H (\theta - \theta^\prime)
$
+ 

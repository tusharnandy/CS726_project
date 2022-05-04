# CS726_project

## Progress

1. The code of independent cascade model is in model-independent-cascade/src/influence.py; the model is not perfect yet. Look at line number 49 and the comment above it.
2. The probability of a node being able to activate its neighbor depends on the edge features, which consists of alpha and beta. I've not been able to understand the dimensions of each of them. All I know is that under the setting of our problem, we have to "learn" the edge features simultaneously.
3. But we also need "ground-truth" values of alpha and beta so that we can run the cascade model. 
4. There are hints about contructing the ground-truth edge features in the 1st paragraph starting _"Since the  ground-truth diffusion probabilities..."_ right column on page 5 of our paper.
5. Coming to the ORACLE. The code is in notebook.ipynb, under the function __degdisIC.__ The pseudocode is as follows:

    <img src="/model-independent-cascade/imgs/DegreeDiscountIC.png" alt="Degree Discount Method" width="600">

    Notice the value _p_ on line 12. I am not sure as yet whether this is a fixed parameter or the $\hat p$ that our code is calculating.

---
## References
[1] [cbhua/model-independent-cascade](https://github.com/cbhua/model-independent-cascade)

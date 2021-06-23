# Simulation to evaluate different approaches for risk-based benefit assessment

![front](https://github.com/rekkasA/arekkas_HteSimulation_XXXX_2021/blob/master/extras/figures/front.png)

## Summary
## 
**Objective:** Compare risk-based methods for individualizing treatment effects
with simulations in the RCT setting. **Study Design and Setting:** We predicted
absolute benefit based on an available prognostic index (PI) using: a model with
the PI and a constant relative treatment effect; a model including an
interaction of treatment with the PI; 4 quarters of the PI; nonlinear
transformations of the PI (restricted cubic splines with 3, 4 and 5 knots); an
adaptive model selection method using Akaike’s Information Criterion. Starting
from a base case scenario (sample size 4,250, constant odds ratio 0.8, AUC of
the PI 0.75), we considered diverse assumptions by introducing linear and
quadratic interactions of the PI with treatment and varying sample size and
discriminative ability of the PI. We evaluated performance using root mean
squared error, discrimination and calibration for benefit. **Results:** Models
including a linear interaction of the PI with treatment had adequate performance
that was robust under most simulation scenarios. Restricted cubic splines
required larger sample sizes and higher AUC of the PI to achieve adequate
performance. The adaptive approach performed equivalently to the best-performing
method in each scenario. **Conclusion:** Usually, models with just a linear
interaction of the PI with treatment adequately predict absolute benefit.

## Replication

To rerun the simulation study and regenerate the report run:

```bash
git clone https://github.com/rekkasa/arekkas_HteSimulation_XXXX_2021.git
cd arekkas_HteSimulation_XXXX_2021
make clean
make submission/manuscript.pdf
```
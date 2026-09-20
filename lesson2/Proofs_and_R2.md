### 1. 代数证明题 

最小二乘法（OLS）旨在最小化残差平方和： $$ RSS = \sum (y_i - \beta_0 - \beta_1 x_i)^2 $$ 

对参数求偏导并令其为 0： 

1. 对 $\beta_0$ 求导：$\frac{\partial RSS}{\partial \beta_0} = -2 \sum e_i = 0 \implies \sum e_i = 0$ 
1. 2. 对 $\beta_1$ 求导：$\frac{\partial RSS}{\partial \beta_1} = -2 \sum x_i e_i = 0 \implies \sum x_i e_i = 0$ 

### 2. 理解思考题 

 **$R^2$ 上升**：$R^2 = 1 - RSS/TSS$。增加变量必然使残差平方和 ($RSS$) 减小或不变（$TSS$ 固定），因此 $R^2$ 必然上升。 -

**$R^2_{adj}$ 下降**：$R^2_{adj} = 1 - \frac{RSS/(n-p-1)}{TSS/(n-1)}$。加入无关特征时，$RSS$ 下降极微，不足以抵消自由度惩罚项（分母 $n-p-1$ 减小）带来的影响，导致 $R^2_{adj}$ 下降。
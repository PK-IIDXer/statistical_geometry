パラメトリックモデル$(\Theta,(\Omega,\mathcal{F},\mu),\{P_\theta\}_{\theta\in\Theta})$を以下で定義する。
- $(\Omega,\mathcal{F},\mu)$: 測度空間で、$\mu$は$\sigma$有限
- $\Theta$: 有限次元$C^\infty$多様体
- $P_\theta$: 確率測度
- $P_\theta\ll\mu$
- 任意の$\omega\in\Omega$に対して、確率密度関数$$p(\omega;\cdot):\Theta\to\mathbb{R};\theta\mapsto p(\omega;\theta):=\frac{dP_\theta(\omega)}{d\mu}$$は正値をとり、かつ$C^\infty$級
- 任意の$\theta\in\Theta$と$v\in T_\theta\Theta$に対して、$$\int_\Omega v(p(\omega;\cdot))d\mu(\omega)=v\left(\int_\Omega p(\omega;\cdot)d\mu(\omega)\right)$$
- 任意の$\theta\in\Theta$に対して、線形写像$$T_\theta\Theta\otimes T_\theta\Theta\ni(u,v)\mapsto\int_\Omega u(l(\omega;\cdot)) \; v(l(\omega;\cdot))\; p(\omega;\theta)d\mu(\omega)$$は正定値非退化。ここで$l(\omega;\theta):=\log p(\omega;\theta)$

$M_i=(\Theta_i,(\Omega_i,\mathcal{F}_i,\mu_i),\{P_{i,\theta_i}\}_{\theta_i\in\Theta_i})$を二つのパラメトリックモデルとする($i=1,2$)。$C^\infty$写像$\varphi:\Theta_1\to\Theta_2$とマルコフ核$K:\Omega_1\times\mathcal{F}_2\to[0,1]$の組$(\varphi,K)$であって、$$P_{2,\varphi(\theta_1)}(A)=\int_{\Omega_1}K(\omega,A)dP_{1,\theta_1}(\omega)$$を満たすものを、$M_1$から$M_2$へのパラメトリックモデルの射とよぶ。
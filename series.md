# 十二章 无穷级数
## 第一节 常数项级数的概念和性质
### 一、常数项级数的概念
- 数列：$u_1,u_2,u_3,...,u_n,...,$  
- 级数（常数项无穷级数）：$\sum\limits_{n=1}^{\infty}u_n =u_1+u_2+u_3+...+u_n+...,$  
- 一般项：$u_n$  
- 部分和：$s_n=u_1+u_2+...+u_n=\sum\limits_{i=1}^{n}u_i$  
- 部分和数列：$\{s_n\}$
- 收敛：如果级数$\sum\limits_{n=1}^{\infty}u_n$的部分和数列$\{s_n\}$有极限，即

    $$
    \lim_{x \to + \infty}s_n=s,
    $$
    此时，$s$ 叫级数的和。  
- 余项：$r_n=s-s_n=u_{n+1}+u_{n+2}+...$  
- 误差：余项的绝对值$\left| r_n \right|$

### 二、收敛级数的基本性质
- 性质1：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛于 $s$ ，则级数 $\sum\limits_{n=1}^{\infty}ku_n$ 也收敛，其和为 $ks$ 。
- 性质2：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 、 $\sum\limits_{n=1}^{\infty}v_n$ 分别收敛于和 $s$ 、 $\sigma$ ，则级数 $\sum\limits_{n=1}^{\infty}(u_n \pm v_n)$ 也收敛，且其和为 $s \pm \sigma$ 。
- 性质3：在级数中去掉、加上或改变有限项，不会改变级数的收敛性。
- 性质4：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛，则这对级数的项任意加括号后所成的级数

    $$
    (u_1+...+ u_{n_{1}})+(u_{n_{1}+1}+...+u_{n_{2}})+(u_{n_{k-1}+1}+...+u_{n_{k}})+...
    $$
    仍然收敛，且其和不变。
- 性质5（级数收敛的必要条件）：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛，则它的一般项 $u_n$ 趋于零，

    $$
    \lim_{n \to \infty} u_n = 0.
    $$

### 三、柯西审敛原理
判断一个级数的收敛性质。
 - 定理（`柯西审敛原理`）：级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛的充分必要条件为：对于任意给定的正数 $\varepsilon$，总存在正整数 $N$，使得当 $n>N$时，对于任意的正整数 $p$，都有

    $$
    \left| u_{n+1}+u_{n+2}+...+u_{n+p} \right| < \varepsilon 
    $$
    成立。  
    证：$\left| u_{n+1}+u_{n+2}+...+u_{n+p} \right|=\left| s_{n+p}-s_n \right|$。$\varepsilon-N$ 语言是指的：$\varepsilon$ 是误差，只要想，就能小于给定的误差 $\varepsilon$。

## 第二节 常数项级数的审敛法
### 一、正项级数及其审敛法
许多级数的收敛性问题可以归结为正项级数的收敛性问题。  
级数 $u_1+u_2+...+u_n+...$ 是正项级数 ($u_n\ge0$) ，它的部分和为 $s_n$ 。显然，数列 $\{s_n\}$ 是一个单调增加数列。若数列 $\left| s_n \right|$ 有界，根据单调有界必有极限：知级数必收敛于  $\lim\limits_{n \to \infty}s_n=s$ 。
- 定理1：正项级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛的充分必要条件是：它的部分和数列 $\{s_n\}$ 有界。
- 定理2（`比较审敛法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 和 $\sum\limits_{n=1}^{\infty}v_n$ 都是正项级数，且 $u_n \le v_n(n=1,2,...)$ 。若级数 $\sum\limits_{n=1}^{\infty}v_n$ 收敛，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛；反之，若级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散，则级数 $\sum\limits_{n=1}^{\infty}v_n$ 发散。
    - 推论：$u_n \le kv_n(k>0)$
- 定理3（`比较审敛法的极限形式`）：设$\sum\limits_{n=1}^{\infty}u_n$和$\sum\limits_{n=1}^{\infty}v_n$都是正项级数，
    - （1）如果 $\lim\limits_{n \to \infty}{\frac{u_n}{v_n}}=l (0 \le l < +\infty)$ ，且级数 $\sum\limits_{n=1}^{\infty}v_n$ 收敛，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛；
    - （2）如果 $\lim\limits_{n \to \infty}{\frac{u_n}{v_n}}=l > 0$ 或 $\lim\limits_{n \to \infty}{\frac{u_n}{v_n}}=+\infty$ ，且级数 $\sum\limits_{n=1}^{\infty}v_n$ 发散，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散。

- 定理4（`比值审敛法`，`达朗贝尔(d'Alembert)判别法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，如果

    $$
    \lim_{n \to \infty} \frac{u_{n+1}}{u_n}= \rho，
    $$
    则当 $\rho < 1$ 时级数收敛； $\rho>1$ （或 $\lim\limits_{n \to \infty} \frac{u_{n+1}}{u_n}= \infty$ ）时级数发散； $\rho=1$ 级数可能收敛可能发散。
- 定理5（`根值审敛法`，`柯西判别法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，如果

    $$
    \lim_{n \to \infty} \sqrt[n]{u_n} = \rho，
    $$
    则当 $\rho<1$ 时收敛，  $\rho >1$（或 $\lim\limits_{n \to \infty} \sqrt[n]{u_n}=+ \infty$ ）时级数发散， $\rho=1$ 时级数可能收敛也可能发散。

- 定理6（`极限审敛法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，
    - （1）如果 $\lim\limits_{n \to \infty}nu_n=l>0$ 或 $\lim\limits_{n \to \infty}nu_n=+\infty$，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散；
    - （2）如果 $p>1$，而 $\lim\limits_{n \to \infty} n^p u_n=l (0 \le l < +\infty)$ ，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛。  
    证明：用极限形式的比较审敛法，分别取 $v_n=\frac{1}{n}$ 和 $v_n=\frac{1}{n^p}$ 。

### 二、交错级数及其审敛法
所谓交错级数：

$$
u_1-u_2+u_3-u_4+...,
$$
其中 $u_n$ 都是正数。
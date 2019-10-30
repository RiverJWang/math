# 十二章 无穷级数
## 第一节 常数项级数的概念和性质
### 一、常数项级数的概念
- 数列：$u_1,u_2,u_3,\dotsc,u_n,\dotsc,$ 。
- 级数（常数项无穷级数）：$\sum\limits_{n=1}^{\infty}u_n =u_1+u_2+u_3+\dotsb+u_n+\dotsb,$ 。
- 一般项：$u_n$ 。
- 部分和：$s_n=u_1+u_2+\dotsb+u_n=\sum\limits_{i=1}^{n}u_i$ 。 
- 部分和数列：$\{s_n\}$ 。
- 收敛：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 的部分和数列 $\{s_n\}$ 有极限，即

    $$
    \lim_{x \to + \infty}s_n=s,
    $$
    此时，$s$ 叫级数的和。  
- 余项：$r_n=s-s_n=u_{n+1}+u_{n+2}+\dotsb$ 。
- 误差：余项的绝对值 $\left| r_n \right|$ 。

### 二、收敛级数的基本性质
- 性质1：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛于 $s$ ，则级数 $\sum\limits_{n=1}^{\infty}ku_n$ 也收敛，其和为 $ks$ 。
- 性质2：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 、 $\sum\limits_{n=1}^{\infty}v_n$ 分别收敛于和 $s$ 、 $\sigma$ ，则级数 $\sum\limits_{n=1}^{\infty}(u_n \pm v_n)$ 也收敛，且其和为 $s \pm \sigma$ 。
- 性质3：在级数中去掉、加上或改变有限项，不会改变级数的收敛性。
- 性质4：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛，则这对级数的项任意加括号后所成的级数

    $$
    (u_1+\dotsb+ u_{n_{1}})+(u_{n_{1}+1}+\dotsb+u_{n_{2}})+(u_{n_{k-1}+1}+\dotsb+u_{n_{k}})+\dotsb
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
    \left| u_{n+1}+u_{n+2}+\dotsb+u_{n+p} \right| < \varepsilon 
    $$
    成立。  
    证：$\left| u_{n+1}+u_{n+2}+\dotsb+u_{n+p} \right|=\left| s_{n+p}-s_n \right|$。$\varepsilon-N$ 语言是指的：$\varepsilon$ 是误差，只要想，就能小于给定的误差 $\varepsilon$。

## 第二节 常数项级数的审敛法
### 一、正项级数及其审敛法
许多级数的收敛性问题可以归结为正项级数的收敛性问题。  
级数 $u_1+u_2+\dotsb+u_n+\dotsb$ 是正项级数 ($u_n\ge0$) ，它的部分和为 $s_n$ 。显然，数列 $\{s_n\}$ 是一个单调增加数列。若数列 $\left| s_n \right|$ 有界，根据单调有界必有极限：知级数必收敛于  $\lim\limits_{n \to \infty}s_n=s$ 。
- 定理1：正项级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛的充分必要条件是：它的部分和数列 $\{s_n\}$ 有界。
- 定理2（`比较审敛法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 和 $\sum\limits_{n=1}^{\infty}v_n$ 都是正项级数，且 $u_n \le v_n(n=1,2,\dotsc)$ 。若级数 $\sum\limits_{n=1}^{\infty}v_n$ 收敛，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛；反之，若级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散，则级数 $\sum\limits_{n=1}^{\infty}v_n$ 发散。
    - 推论：$u_n \le kv_n(k>0)$
- 定理3（`比较审敛法的极限形式`）：设$\sum\limits_{n=1}^{\infty}u_n$和$\sum\limits_{n=1}^{\infty}v_n$都是正项级数，
    - （1）如果 $\lim\limits_{n \to \infty}{\dfrac{u_n}{v_n}}=l (0 \le l < +\infty)$ ，且级数 $\sum\limits_{n=1}^{\infty}v_n$ 收敛，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛；
    - （2）如果 $\lim\limits_{n \to \infty}{\dfrac{u_n}{v_n}}=l > 0$ 或 $\lim\limits_{n \to \infty}{\dfrac{u_n}{v_n}}=+\infty$ ，且级数 $\sum\limits_{n=1}^{\infty}v_n$ 发散，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散。

- 定理4（`比值审敛法`，`达朗贝尔(d'Alembert)判别法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，如果

    $$
    \lim_{n \to \infty} \dfrac{u_{n+1}}{u_n}= \rho，
    $$
    则当 $\rho < 1$ 时级数收敛； $\rho>1$ （或 $\lim\limits_{n \to \infty} \dfrac{u_{n+1}}{u_n}= \infty$ ）时级数发散； $\rho=1$ 级数可能收敛可能发散。
- 定理5（`根值审敛法`，`柯西判别法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，如果

    $$
    \lim_{n \to \infty} \sqrt[n]{u_n} = \rho，
    $$
    则当 $\rho<1$ 时收敛，  $\rho >1$（或 $\lim\limits_{n \to \infty} \sqrt[n]{u_n}=+ \infty$ ）时级数发散， $\rho=1$ 时级数可能收敛也可能发散。

- 定理6（`极限审敛法`）：设 $\sum\limits_{n=1}^{\infty}u_n$ 为正项级数，
    - （1）如果 $\lim\limits_{n \to \infty}nu_n=l>0$ 或 $\lim\limits_{n \to \infty}nu_n=+\infty$，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 发散；
    - （2）如果 $p>1$，而 $\lim\limits_{n \to \infty} n^p u_n=l (0 \le l < +\infty)$ ，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛。  
    证明：用极限形式的比较审敛法，分别取 $v_n=\dfrac{1}{n}$ 和 $v_n=\dfrac{1}{n^p}$ 。

### 二、交错级数及其审敛法
所谓交错级数：

$$
u_1-u_2+u_3-u_4+\dotsb,
$$
其中 $u_n$ 都是正数。
- 定理7（莱布尼兹定理）：如果交错级数 $\sum\limits_{n=1}^{\infty}(-1)^{n-1} u_n$ 满足条件：  
    （1） $u_n \ge u_{n+1}(n=1,2,3,\dotsc)$ ；  
    （2） $\lim\limits_{n \to \infty} u_n =0$,  
    则级数收敛，且其和 $s \le u_1$ ，其 余项 $r_n$ 的绝对值 $|r_n| \le u_{n+1}$。

### 三、绝对收敛和条件收敛
- 绝对收敛：如果实数级数 $\sum\limits_{n=1}^{\infty}u_n$ 各项的绝对值所构成的正项级数 $\sum\limits_{n=1}^{\infty}|u_n|$ 收敛，称级数 $\sum\limits_{n=1}^{\infty}u_n$ 绝对收敛。
- 条件收敛：如果实数级数 $\sum\limits_{n=1}^{\infty}u_n$ 收敛， 而级数 $\sum\limits_{n=1}^{\infty}|u_n|$ 发散，则称级数 $\sum\limits_{n=1}^{\infty}u_n$ 条件收敛。
- 定理8：如果级数 $\sum\limits_{n=1}^{\infty}u_n$ 绝对收敛，则级数 $\sum\limits_{n=1}^{\infty}u_n$ 必定收敛。 

### * 四、绝对收敛级数的性质
- 定理9：绝对收敛级数经改变项的位置后构成的级数也收敛，且与原级数有相同的和（即绝对收敛级数具有可交换性）。
- 定理10（绝对收敛级数的乘法）：设级数 $\sum\limits_{n=1}^{\infty}u_n$ 和级数 $\sum\limits_{n=1}^{\infty}u_n$ 都绝对收敛，其和分别为 $s$ 和 $\sigma$，则它们的柯西乘积

    $$
    u_1v_1+(u_1v_2+u_2v_1)+\dotsb+(u_1v_n+u_2v_{n-1}+..+u_nv_1)+\dotsb
    $$
    也是绝对收敛的，且其和为 $s \cdot \sigma$。

## 第三节 幂级数
### 一、函数项级数的概念
- 给定一个定义在区间 $I$ 上的函数列 $u_1(x),u_2(x),u_3(x),\dotsc,u_n(x),\dotsc,$ 则由着函数列构成的表达式

    $$
    \tag{1}
    u_1(x)+u_2(x)+u_3(x)+\dotsb+u_n(x)+\dotsb
    $$
    称为定义在区间 $I$ 上的（函数项）无穷级数或（函数项）级数。
    对于每一个确定的值 $x_0 \in I$ ，函数项级数（1）成为常数项级数
    
    $$
    \tag{2}
    u_1(x_0)+u_2(x_0)+u_3(x_0)+\dotsb+u_n(x_0)+\dotsb
    $$
- 收敛点：若（2）在 $x_0$ 处收敛，称 $x_0$ 是函数项级数（1）的收敛点。
- 发散点同理。
- 收敛域：函数项级数（1）的收敛点的全体称为它的收敛域，发散点的全体称为它的发散域。
- 和函数：在收敛域上，函数项级数的和是 $x$ 的函数 $s(x)$ ，通常称 $s(x)$ 为函数项级数的和函数，定义域是级数的收敛域。写成

    $$
    s(x)=u_1(x)+u_2(x)+u_3(x)+\dotsb+u_n(x)+\dotsb
    $$
- 函数项级数`部分和`：把函数项级数的前 $n$ 项的部分和记作 $s_n(x)$。
- 函数项级数`和函数`：把函数项级数的前 $n$ 项的部分和记作 $s_n(x)$ ，则在收敛域上有$\lim\limits_{n\to\infty}s_n(x)=s(x)$。
- 函数项级数余项：记 $r_n(x)=s(x)-s_n(x)$，$r_n(x)$叫函数项余数的余项（在收敛域），并有$\lim\limits_{n\to\infty}r_n(x)=0$。

### 二、幂级数及其收敛性
- 幂级数：函数项级数中各项都是幂函数，它的形式是
 
    $$
    \tag{3}
    \sum_{n=0}^{\infty}a_nx^n=a_0+a_1x+a_2x^2+\dotsb+a_nx^n+\dotsb
    $$
    其中，常数 $a_0,a_1,a_2,\dotsc,a_n,\dotsc$ 叫做幂级数的系数。
- 定理1（`阿贝尔（Abel）定理`）：如果级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 当 $x=x_0(x_0 \ne 0)$ 时收敛，则适合不等式 $|x|<|x_0|$ 时的一切 $x$ 使这幂级数绝对收敛。反之，如果级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 当 $x=x_0$ 时发散，则适合不等式 $|x|>|x_0|$ 的一切 $x$ 使这幂级数发散。
    - 推论：如果幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 不是仅在 $x=0$ 一点收敛，也不是在整个数轴上都收敛，则必有一个确定的正数 $R$ 存在，使得当 $|x|<R$ 时，幂级数绝对收敛；当 $|x|>R$ 时，幂级数发散；当 $x=R$ 与 $x=-R$ 时，幂级数可能收敛也可能发散。
    - 收敛半径：正数 $R$ 通常叫做幂级数（3）的收敛半径。
    - 开区间 $(-R,R)$ 叫做幂级数（3）的收敛区间。
- 定理2（幂级数的收敛半径求法）：如果 $\lim\limits_{n\to\infty}\left| \dfrac{a_{n+1}}{a_n} \right|=\rho$，其中 $a_n、a_{n+1}$ 是幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 的相邻两项的系数，则这个幂级数的收敛半径

$$
 R =
  \begin{cases}
    1/\rho    & \quad \rho \ne 0,  \\  
    +\infty   & \quad \rho = 0,  \\  
    0    & \quad \rho = +\infty. \\  
  \end{cases}
$$

### 三、幂函数的运算
设幂函数 

$$
\sum_{n=0}^{\infty}a_nx^n=a_0+a_1x+a_2x^2+\dotsb+a_nx^n+\dotsb 
$$ 
$$
\sum_{n=0}^{\infty}b_nx^n=b_0+b_1x+b_2x^2+\dotsb+b_nx^n+\dotsb 
$$
分别在区间 $(-R,R)$ 及 $(-R',R')$内收敛，对于这两个幂级数，可以进行加减乘除，在较小的区间内成立。

`和函数性质`
- 性质1：幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 的和函数 $s(x)$ 在其收敛域 $I$ 上连续。
- 性质2：幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 的和函数 $s(x)$ 在其收敛域 $I$ 上可积，并有逐项积分公式

    $$
    \tag{5}
    \int_0^x s(x)\,\mathrm{d}x = \int_0^x\left[\sum_{n=0}^{\infty}a_nx^n\right]\mathrm{d}x=\sum_{n=0}^{\infty} \int_0^x a_nx^n \mathrm{d}x  \\
    =\sum_{n=0}^{\infty} \dfrac{a_n}{n+1}x^{n+1} \quad (x \in I),
    $$
    逐项积分后所得到的幂级数和原级数有相同的收敛半径。
- 性质3：幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 的和函数 $s(x)$ 在其收敛区间 $(-R,R)$ 内可导，且有逐项求导公式

    $$
    \tag{6}
    s'(x)=\left(\sum_{n=0}^{\infty}a_nx^n \right)'= \sum\limits_{n=0}^{\infty}\left(a_nx^n \right)'= \sum\limits_{n=0}^{\infty}n a_nx^{n-1} \quad(|x|< R)
    $$
    逐项求导后所得到的的幂级数和原级数有相同的收敛半径。
    - 反复应用上述结论，幂级数 $\sum\limits_{n=0}^{\infty}a_nx^n$ 的和函数 $s(x)$ 在其收敛区间 $(-R,R)$ 内具有任意阶导数。

### 四、函数展开成幂级数
- 换句话说，也就是：能否找到这样一个幂级数，它在某区间内收敛，且其和恰好就是给定的函数 $f(x)$。如果能找到这样的幂级数，就说，函数 $f(x)$ 在该区间内能展开成幂级数。
- 假设函数 $f(x)$ 在点 $x_0$ 的某领域 $U(x_0)$ 内能展开成幂级数，即有：

    $$
    \tag{1}
    f(x) =a_0+a_1(x-x_0)+a_2(x-x_0)^2+\dotsb+a_n(x-x_0)^n+\dotsb, \, x \in U(x_0)
    $$
    根据和函数性质，可知 $f(x)$ 在 $U(x_0)$ 内应具有任意阶导数，且

    $$
    f^{(n)}(x) = n!a_n + (n+1)!a_{n+1}(x-x_0)+\dfrac{(n+2)!}{2!}(x-x_0)^2 + \dotsb,
    $$
    可得到 $f^{(n)}(x_0)=n!a_n$，于是 
    
    $$
    \tag{2}
    a_n=\dfrac{1}{n!}f^{(n)}x_0 \quad (n=0,1,2,\dotsc)
    $$
    
- 若函数 $f(x)$ 有幂级数展开式（1），那么该幂函数的系数 $a_n$ 由公式（2）确定，即该幂级数必为

    $$
    \tag{3}
    f(x_0)+f'(x_0)(x-x_0)+ \dotsb + \dfrac{1}{n!}f^{(n)}(x_0)(x-x_0)^n + \dotsb \\
    = \sum\limits_{n=0}^{\infty} \dfrac{1}{n!}f^{(n)}(x_0)(x-x_0)^n,
    $$
    此幂级数（3）叫做函数 $f(x)$ 在点 $x_0$ 处的$\color{red}{泰勒级数}$。

    而展开式必为
    
    $$
    \tag{4}
    f(x)= \sum\limits_{n=0}^{\infty} \dfrac{1}{n!}f^{(n)}(x_0)(x-x_0)^n, \quad x \in U(x_0)
    $$
    此展开式（4）为函数 $f(x)$ 在点 $x_0$ 处的$\color{red}{泰勒展开式}$。
- 如： 函数项级数$1+x+x^2+ \dotsb + x^n + \dotsb$ 在 $|x|<1$ 时，这时候级数收敛于和 $\dfrac{1}{1-x}$ ;
    此时有
    
    $$\dfrac{1}{1-x}=1+x+x^2+ \dotsb + x^n + \dotsb \quad (-1<x<1)；$$
- 反过来， $f(x)$可以在区间 $(-1<x<1)$ 上展开成 $1+x+x^2+ \dotsb + x^n + \dotsb$。

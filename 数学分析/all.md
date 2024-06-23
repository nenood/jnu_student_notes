# 级数

## 数项级数

### 级数的敛散性

-   **数项级数：**
    对于数列 $\{u_n\}$ ，$\sum\limits_{i=1}^{\infty}u_i$ 称为 **数项级数**
-   **部分和：**
    $S_n = \sum\limits_{i=1}^nu_i$ 称为数项级数的 **第 $n$ 个部分和**，简称 **部分和**
-   **收敛与和：**
    若 $\lim\limits_{n\to\infty}S_n = S$ 则称数项级数 **收敛**，$S$ 为数项级数的 **和**

#### 级数收敛的柯西准则

数项级数收敛的 **充要条件：**

任给正数 $\epsilon$ ，总存在正整数 $N$ ，使得当 $m > N$ 时，对任一正整数 $p$ ，都有
$$
|u_{m+1} + u_{m+2} + \dots +u_{m+p}| < \epsilon
$$

-   推论：级数收敛的必要条件为 $\lim\limits_{n\to\infty}u_n = 0$

### 正项级数

#### 比较原则

对于两个正项级数 $u_n, v_n$ ，若存在某正整数 $N$ 对一切 $n>N$ 都有
$$
u_n \le v_n
$$
则

1.   若级数 $\sum v_n$ 收敛，则级数 $\sum u_n$ 也收敛
2.   若级数 $\sum u_n$ 发散，则级数 $\sum v_n$ 也发散

#### 比较原则的推论

$$
\lim_{n\to\infty}\frac{u_n}{v_n} = l
$$

1.   $0 < l < +\infty$，两级数同敛散
2.   $l = 0, l=+\infty$ ，$\sum v_n$ 的敛散决定 $\sum u_n$ 的敛散

#### 比式判别法、根式判别法

$$
\lim_{n\to\infty}\frac{u_{n+1}}{u_n} = q
$$

1.   $q<1$ ，收敛
2.   $q>1, q=+\infty$ ，发散
3.   $q=1$ ，无法判断

$$
\lim_{n\to\infty}\sqrt[n]{u_n} = l
$$

1.   $l<1$ ，收敛
2.   $l>1$ ，发散
3.   $l=1$ ，无法判断

### 一般项级数

#### 交错级数

##### 莱布尼茨判别法

若数列 $\{u_n\}$ 单调递减且 $\lim\limits_{n\to\infty}u_n=0$

则级数 $\sum u_n$ 收敛

#### 绝对收敛

$\sum\limits_{i=1}^{\infty}|u_i|$ 收敛，则称 $\sum u_n$ 为 **绝对收敛级数**

-   绝对收敛级数一定收敛
-   收敛但是不绝对收敛的级数称为 **条件收敛级数**

#### 阿贝尔判别法和狄利克雷判别法

对于 数列 $\{a_n\},\{b_n\}$，

1.   $\{a_n\}$ 为单调有界数列，$\sum b_n$ 收敛
2.   $\{a_n\}$ 单调递减且 $\lim\limits_{n\to\infty}$ ，$\{b_n\}$ 的部分和数列 $\{S_n\}$ 有界

满足以上条件之一则 $\sum (a_nb_n)$ 收敛

## 函数项级数

-   **函数列：**
    对于每一个 $n$ 都有一个对应的函数 $f_n$，称这样的由函数组成的序列为 **函数列**

-   **收敛域：**
    $$
    \lim_{n\to\infty}f_n(x) = f(x),~~x\in D
    $$
    $D$ 称为函数列 $\{f_n(x)\}$ 的 **收敛域**

### 函数列的一致收敛性

#### 一致收敛的定义

设函数列 $\{f_n(x)\}$ 与函数 $f$ 定义在同一数集 $D$ 上，

若对任给的 $\epsilon > 0$ ，总存在一个正整数 $N$ ，使得当 $n > N$ 是，对一切 $x \in D$ ，都有
$$
|f_n(x) - f(x)| < \epsilon
$$
则称函数列在 $D$ 上 **一致收敛** 于 $f$ ，记作
$$
f_n(x) \rightrightarrows f(x)~~~~(n\to\infty), ~~~~x \in D
$$

#### 内闭一致收敛

设函数列 $\{f_n(x)\}$ 与函数 $f$ 定义在同一数集 $D$ 上，

若对任一的闭区间 $[a, b] \sub I$ ，$\{f_n\}$ 在该区间上一致收敛于 $f$ ，

则称 $\{f_n\}$ 在 $I$ 上 **内闭一致收敛** 于 $f$ 

#### 一致收敛的柯西准则

函数列 $\{f_n(x)\}$ 在数集 $D$ 上一致收敛的 **充要条件：**

对任给的 $\epsilon > 0$ ，总存在正数 $N$ 使得当 $n, m > N$ 时，对一切 $x \in D$ ，都有
$$
|f_n(x) - f_m(x)| < \epsilon
$$

#### 一致收敛定理

函数列 $\{f_n(x)\}$ 在数集 $D$ 上一致收敛的 **充要条件：**
$$
\lim_{n\to\infty}\sup_{x \in D}|f_n(x) - f(x)|=0
$$
也可以由此得到不一致收敛的充要条件：存在 $x_n$ 使得 $|f_n(x_n) - f(x_n)|$ 不收敛于 $0$

### 函数项级数

#### 定义

对于函数列 $\{u_n(x)\}$，$u_1(x) + u_2(x) + \dots + u_n(x) + \dots,~~x \in E$ 称为

定义在 $E$ 上的 **函数项级数**，记为 $\sum u_n(x)$

$S_n(x) = \sum\limits_{k=1}^{n}u_k(x)$ 称为 $\sum u_n(x)$ 的部分和函数列
$$
\lim_{n\to\infty}S_n(x) = S(x),~~~~x \in D
$$
$D$ 称为级数 $\sum u_n(x)$ 的收敛域

这也说明了函数项级数的收敛性 就是 其部分和函数列的收敛性

#### 函数项级数的一致收敛

若函数项级数的部分和函数列一致收敛，则该函数项级数 **一致收敛**

若函数项级数在闭区间内一致收敛，则称它在该区间上 **内闭一致收敛**

#### 一致收敛的柯西准则

函数项级数 $\sum u_n(x)$ 在数集 $D$ 上一致收敛的 **充要条件：**

任给 $\epsilon > 0$ ，总存在某正整数  $N$，

使得当 $n > N$ 时，对一切 $x\in D$ 和一切正整数 $p\ge 2$，都有
$$
|S_{n+p}(x) - S_n(x)| < \epsilon
$$
若 $p=1$ ，则该条件为必要条件

**推论：**

函数项级数在数集 $D$ 上一致收敛的必要条件是 其函数列在 $D$ 上一致收敛于零

#### 一致收敛定理

函数项级数 $\sum u_n(x)$ 在数集 $D$ 上一致收敛的 **充要条件：**
$$
\lim_{n\to\infty}\sup_{x \in D}|S_n(x) - S(x)|=0
$$

#### 魏尔斯特拉斯 $M$ 判别法

设函数项级数 $\sum u_n(x)$ 定义在数集 $D$ 上，$\sum M_n$ 为收敛的正项级数，

若对一切 $x \in D$ 有
$$
|u_n(x)| \le M_n, n = 1, 2, \dots
$$
则该函数项级数在 $D$ 上收敛

#### 阿贝尔判别法

1.   $\sum u_n(x)$ 在区间 $I$ 上一致收敛
2.   对于每一个 $x \in  I$ ，$\{v_n(x)\}$ 单调
3.   $\{v_n(x)\}$ 在 $I$ 上一致有界

则 $\sum u_n(x)v_n(x)$ 收敛

#### 狄利克雷判别法

1.   $\sum u_n(x)$ 的部分和函数列 $S_n(x)$ 在 $I$ 上一致有界
2.   对于每一个 $x \in  I$ ，$\{v_n(x)\}$ 单调
3.   在 $I$ 上函数列 $v_n(x)$ 一致收敛于零

则 $\sum u_n(x)v_n(x)$ 收敛

### 一致函数列于函数项级数的性质

省流：

在一定条件下，求和可以于求极限、求积、求导运算交换

## 幂级数

### 幂级数

#### 定义

$$
\sum_{n=0}^{\infty}a_n(x-x_0)^n
$$

这样的函数项级数称为 **幂级数**（仅讨论 $x_0 = 0$ 的情况）

#### 收敛区间    收敛半径

幂级数的收敛域是以原点为中心的区间，若以 $2R$ 表示区间的长度，则

$R$ 称为幂级数的 **收敛半径**，区间 $(-R, R)$ 称为 **收敛区间**

-   在 $x = \pm R$ 处，幂级数可能收敛也可能发散

#### 收敛半径的求解

对于
$$
\lim_{n\to\infty}\sqrt[n]{|a_n|} = \rho
$$

1.   $0 < \rho < +\infty，R = \frac{1}{\rho}$
2.   $\rho = 0, R = +\infty$
3.   $\rho = +\infty, R = 0$

也可以使用比式判别法：
$$
\lim_{n\to\infty}\frac{|a_{n+1}|}{|a_n|} = \rho
$$
若该极限存在，则有 $\lim\limits_{n\to\infty}\sqrt[n]{|a_n|} = \rho$

#### 一致收敛

幂级数在收敛区间 $(-R, R)$ 内的任一闭区间 $[a, b]$ 上都一致收敛

### 幂级数展开

#### 泰勒级数

$$
f(x_0) + \sum_{n=1}^{\infty} \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n
$$

该级数称为 **泰勒级数**

#### 函数的泰勒级数的收敛

设 $f$ 在点 $x_0$ 具有任意阶导数，

则 $f$ 在区间 $(x_0 - r, x_0 + r)$ 上等于它的泰勒级数的和函数的 **充要条件** 是：
对一切满足不等式 $|x - x_0| < r$ 的 $x$ ，有
$$
\lim\limits_{n \to \infty}R_n(x) = 0
$$
其中 $R_n(x)$ 为 $f$ 在 $x_0$ 处的泰勒公式余项，即
$$
R_n(x) = \frac{f^{(n+1)}(\xi)}{(n+1)!}(x - x_0)^{n+1},~~~~x < \xi < x_0
$$
对于函数在 $x_0 = 0$ 处的展开式
$$
f(0) + \sum_{n=1}^{\infty}\frac{f^{(n)}(0)}{n!}x^n
$$
这称为 $f$ 的 **麦克劳林级数**

##### 各种余项

$$
\begin{align}

R_n(x) &=  
\frac{1}{n!}\int_0^xf^{(n+1)}(t)(x-t)^ndt \\

R_n(x) &=  
\frac{1}{(n+1)!}f^{(n+1)}(\xi)x^{n+1},~~~~x < \xi < x_0\\

R_n(x) &=
\frac{1}{n!}f^{(n+1)}(\theta x)(1-\theta)^nx^{n+1}, 0 \le \theta \le 1 \\

\end{align}
$$

# 多元函数微分

## 二元函数的极限

### 定义

-   **重极限**：
    自变量 $x, y$ **同时** 以任何方式趋近于 $x_0, y_0$，表示为
    $$
    L=\lim\limits_{(x, y) \to (x_0,y_0)} f(x,y)
    $$

-   **累次极限**：
    自变量 $x, y$ **依一定的先后顺序** 相继趋近于 $x_0, y_0$，
    以先对 $x(\to x_0)$ 后对 $y(\to y_0)$ 的累次极限为例
    $$
    K=\lim\limits_{y\to y_0}\lim\limits_{x\to x_0} f(x,y)
    $$

### 定理

-   若两种累次极限和重极限均存在，则三者相等
-   若两种累次极限存在但是不相等，则重极限必不存在

## 二元函数的连续性

-   **连续与间断点**
    $f$ 关于 $D$ 在 $P_0$ 连续 $\iff$ $\lim\limits_{P\to P_0}f(P) = f(P_0)$

    -   若 $P_0$ 是 $D$ 的聚点，而上式不成立，则 $P_0$ 称为 **间断点**
    -   若左边的极限存在而不等于 $f(P_0)$ 则称为 **可去间断点**

-   **全增量与偏增量**
    对于 $P_0(x_0, y_0), P(x, y) \in D, \Delta x = x - x_0, \Delta y = y - y_0$，
    称 $\Delta z = f(x_0 + \Delta x, y_0 + \Delta y) - f(x_0, y_0)$ 为 $f$ 在 $P_0$ 的 **全增量**

    -   $f$ 关于 $D$ 在 $P_0$ 连续 $\iff$ $\lim\limits_{(\Delta x, \Delta y) \to (0, 0)}\Delta z = 0$

    -   在全增量中取 $\Delta x=0$ 或 $\Delta y = 0$，相应的函数增量称为 **偏增量**
    -   全增量极限为零 则 偏增量极限也为零（反过来则不一定）

-   **有界闭域上连续函数的性质**

    -   **有界性与最大最小值定理**
        若 $f$ 在有界闭域上连续，则在该区域内有界 且 能取得最大最小值

    -   **一致连续性定理**

        若 $f$ 在有界闭域上连续，则 $f$ 在该区域上 **一致连续**，既
        对任何 $\epsilon > 0$，总存在 $\delta(\epsilon)$，使得
        对一切点 $P, Q$，只要 $\rho(P, Q) < \delta$ 就有 $|f(P) - f(Q)| < \epsilon$

    -   **介值性定理**
        若 $f$ 在有界闭域上连续，$P_1, P_2$ 为 $D$ 中任意两点，且 $f(P_1) < f(P_2)$ 
        则对任何满足 $f(P_1) < \mu < f(P_2)$ 的 实数 $\mu$ 
        必存在点 $P_0 \in D$，使得 $f(P_0) = \mu$

## 多元函数微分学

### 全微分

若 $f$ 在点 $P_0(x_0, y_0)$ 处的全增量 $\Delta z$ 可以表示为
$$
\begin{align}
\Delta z &= f(x_0 + \Delta x, y_0 + \Delta y) - f(x_0, y_0) \\
&=A\Delta x + B\Delta y + o(\rho)
\end{align}
$$
其中 $A, B$ 是仅与 $P_0$ 有关的常数，$\rho = \sqrt{\Delta x^2 + \Delta y^2}$，
$o(\rho)$ 是较 $\rho$ 高阶的无穷小量，
则称 $f$ 在 $P_0$ **可微**，
称线性函数 $A\Delta x + B\Delta y$ 为函数 $f$ 在点 $P_0$ 的 **全微分**，记作
$$
dz|_{P_0} = df(x_0, y_0) = A\Delta x + B\Delta y
$$

-   当 $|\Delta x|, |\Delta y|$ 足够小时，全微分可以作为全增量的近似值，既
    $$
    f(x, y) \approx f(x_0, y_0) + A(x - x_0) + B(y - y_0)
    $$

#### 可微性条件

-   **可微的必要条件：**
    若 $f$ 在区域 $D$ 上每一点都可微，则 $f$ 在 $D$ 上的全微分为
    $$
    df(x, y) = f_x(x, y)dx + f_y(x, y) dy
    $$

-   **可微的充分条件：**
    若函数 $z = f(x, y)$ 的偏导数在点 $(x_0, y_0)$ 的某邻域内存在，
    且 $f_x， f_y$ 在点 $(x_0, y_0)$ 连续，
    则函数 $f$ 在点 $(x_0, y_0$) 可微

    -   **注：**由于这是**充分条件**，所以**不能**通过偏导数的不连续推出函数的不可微
    -   若函数在某点处的偏导数均连续，则称该函数在这点上 **连续可微**

-   **中值公式：**
    若函数 $f$ 在点 $(x_0, y_0)$ 的某邻域存在偏导数，对于该邻域内的点 $(x, y)$ 
    存在 $\xi = x_0 + \theta_1(x - x_0), \eta = y_0 + \theta_2(y - y_0), 0 < \theta_1, \theta_2 < 1$ 使得
    $$
    f(x, y) - f(x_0, y_0) = f_x(\xi, y)(x - x_0) + f_y(x_0, \eta)(y - y_0)
    $$

#### 复合函数的全微分

若以 $x, y$  为自变量的函数 $z = f(x, y)$ 可微，则其全微分为
$$
dz = \frac{\partial z}{\partial x}dx + \frac{\partial z}{\partial y}dy
$$
用例子来说明 利用复合函数全微分求偏导数 的方法

**例：** 设 $z = e^{xy}\sin(x+y)$，求 $\frac{\partial z}{\partial x},\frac{\partial z}{\partial y}$

**解：** 
$$
\begin{align}
&令 z = e^u\sin v,u = xy, v = x + y，得到 \\ \\
&dz
= z_u du + z_v dv
= e^u\sin v du + e^u\cos v dv\\
&du = ydx + xdy \\
&dv = dx + dy \\ \\

\therefore~
&dz 
= 
e^u\sin v (ydx + xdy) ~+ \\ &~~~~~~~~~e^u\cos v (dx + dy) \\
&~~~~=
e^{xy}[y\sin (x+y) + \cos(x+y)]dx ~+ \\
&~~~~~~~~~
e^{xy}[x\sin (x+y) + \cos(x+y)]dy \\ \\
\therefore~
&z_x = e^{xy}[y\sin (x+y) + \cos(x+y)]\\
&z_y = e^{xy}[x\sin (x+y) + \cos(x+y)]
\end{align}
$$

### 偏导数

设 $z = f(x, y), (x, y) \in D$ 若 $(x_0, y_0) \in D$ 且 $f(x, y_0)$ 在 $x_0$ 的某邻域内有定义，则当
$$
\lim\limits_{\Delta x \to 0}
\frac{\Delta_x f(x_0, y_0)}{\Delta x}
=
\lim\limits_{\Delta x \to 0}
\frac{f(x_0+\Delta x, y_0) - f(x_0, y_0)}{\Delta x}
$$
存在时，称中国极限为 $f$ 在点 $(x_0, y_0)$ 关于 $x$ 的 **偏导数**，记作
$$
f_x(x_0, y_0)~或~\frac{\partial f}{\partial x}\bigg|_{(x_0, y_0)}
$$
若 $z = f(x, y), (x, y) \in D$ 在每一点上都存在对 $x$ 或对 $y$ 的偏导数，
则可得到 $z = f(x, y)$ 对 $x$ 或对 $y$ 的偏导函数（简称偏导数），记作
$$
f_x(x,y)~或~\frac{\partial f}{\partial x}
$$

#### 如何求偏导数

1.   先将其他自变量看作常数
2.   对当前自变量作一元函数求导

#### 复合函数求导（链式法则）

若函数 $x = \varphi(s, t), y = \psi(s,t)$ 在点 $(s, t) \in D$ 可微，

且 $z = f(x,y)$ 在 点 $(x,y) = (\varphi(s, t), \psi(s,t))$ 可微，

则复合函数 $z = f(\varphi(s, t), \psi(s,t))$ 在点 $(s,t)$ 可微，其偏导数为
$$
\frac{\partial z}{\partial s}\bigg|_{(s, t)}
=
\frac{\partial z}{\partial x}\bigg|_{(x, y)}
\frac{\partial z}{\partial s}\bigg|_{(s, t)}
+
\frac{\partial z}{\partial y}\bigg|_{(x, y)}
\frac{\partial y}{\partial s}\bigg|_{(s, t)}

\\

\frac{\partial z}{\partial t}\bigg|_{(s, t)}
=
\frac{\partial z}{\partial x}\bigg|_{(x, y)}
\frac{\partial z}{\partial t}\bigg|_{(s, t)}
+
\frac{\partial z}{\partial y}\bigg|_{(x, y)}
\frac{\partial y}{\partial t}\bigg|_{(s, t)}
$$
一般的，对于 $f(u_1, u_2, \dots,u_m), u_k = g_k(x_1, x_2, \dots,x_n)$ 复合函数的偏导数为
$$
\frac{\partial f}{\partial x_i}
=
\sum_{k=1}^{m}
\frac{\partial f}{\partial u_k}
\frac{\partial u_k}{\partial x_i}
,~(i = 1, 2, \dots , n)
$$

### 方向导数

#### 定义

设三元函数 $f$ 在点 $P(x_0, y_0, z_0)$ 的某邻域 $U(P_0) \sub \mathbf{R^3}$ 有定义，

$l$ 为从点 $P_0$ 出发的射线，

$P(x, y, z)$ 为在 $l$ 上且含于 $U(P_0)$ 内的任一点 ，

以 $\rho$ 表示 $P, P_0$ 之间的距离，若极限
$$
\lim\limits_{\rho \to 0^+}
\frac{f(P) - f(P_0)}{\rho}
=
\lim\limits_{\rho \to 0^+}
\frac{\Delta_lf}{\rho}
$$
存在，则称此极限为 $f$ 在点 $P_0$ 沿方向 $l$ 的 **方向导数**，记作
$$
f_t(P_0)~或~\frac{\partial f}{\partial l}\bigg|_{P_0}
$$

#### 计算公式

$$
f_t(P_0) = f_x(P_0)\cos \alpha + f_y(P_0)\cos \beta + f_z(P_0)\cos \gamma \\
\cos \theta_i = \frac{l_i}{|l|}
$$

其中 $\alpha, \beta, \gamma$ 为方向 $l$ 的方向余弦

### 梯度

#### 定义

若多元函数在某点存在对所有自变量的偏导数，

则称向量 $(f_x(P_0),f_y(P_0),f_z(P_0))$ 为函数 $f$ 在点 $P_0$ 的 **梯度**，记作
$$
\begin{align}
\mathbf{grad}f &= (f_x(P_0),f_y(P_0),f_z(P_0)) \\
|\mathbf{grad}f| &= \sqrt{f_x(P_0^2+f_y(P_0^2+f_z(P_0^2)}
\end{align}
$$

-   若记 $l$ 方向上的单位向量为
    $$
    l_0 = (\cos \alpha, \cos \beta, \cos \gamma)
    $$
    则方向导数公式也可以写成
    $$
    f_l(P_0) = \mathbf{grad}f(P_0)\cdot l_0 = |\mathbf{grad}f(P_0)|\cos\theta
    $$
    $\theta$ 指梯度向量与 $l_0$ 的夹角

### 高阶偏导数

$$
\begin{align}
f_{xx}(x, y) &= \frac{\partial}{\partial x}(\frac{\partial z}{\partial x}) = \frac{\partial^2 z}{\partial x^2}\\
f_{xy}(x, y) &= \frac{\partial}{\partial y}(\frac{\partial z}{\partial x}) = \frac{\partial^2 z}{\partial x \partial y}\\
f_{yx}(x, y) &= \frac{\partial}{\partial x}(\frac{\partial z}{\partial y}) = \frac{\partial^2 z}{\partial y\partial x}\\
f_{yy}(x, y) &= \frac{\partial}{\partial y}(\frac{\partial z}{\partial y}) = \frac{\partial^2 z}{\partial y^2}
\end{align}
$$

#### 定理

-   若 $f_{xy}(x, y), f_{yx}(x, y)$ 都在点 $(x_0, y_0)$ 连续，则
    $$
    f_{xy}(x, y)=f_{yx}(x, y)
    $$

#### 复合函数的高阶偏导数

**例：** 设 $z = f(x, \frac{x}{y})$，求 $\frac{\partial^2 z}{\partial x^2},\frac{\partial^2 z}{\partial x \partial y}$

**解：**
$$
令 z = f(u,v),u = x, v = \frac{x}{y}，得到 \\
\begin{align}
\frac{\partial z}{\partial x} 
= 
\frac{\partial f}{\partial u} \frac{\partial u}{\partial x}+
\frac{\partial f}{\partial v} \frac{\partial v}{\partial x}
=
\frac{\partial f}{\partial u}+
\frac{1}{y} \frac{\partial f}{\partial v} \\
\end{align}
$$

$$
\begin{align}

\frac{\partial^2 z}{\partial x^2}
&=
\frac{\partial}{\partial x}
(\frac{\partial f}{\partial u}+
\frac{1}{y}\frac{\partial f}{\partial v}) \\
&=
\frac{\partial^2 f}{\partial u^2}
+
\frac{2}{y}\frac{\partial^2 f}{\partial u \partial v}
+
\frac{1}{y^2}\frac{\partial^2 f}{\partial v^2}

\\

\frac{\partial^2 z}{\partial x \partial y}
&=
\frac{\partial}{\partial y}
(\frac{\partial f}{\partial u}+
\frac{1}{y}\frac{\partial f}{\partial v}) \\
&=
-\frac{x}{y^2}\frac{\partial^2 f}{\partial u \partial v}
-
\frac{x}{y^3}\frac{\partial^2 f}{\partial v^2}
-
\frac{1}{y^2}\frac{\partial f}{\partial v}

\end{align}
$$

### 中值定理

设二元函数 $f$ 在凸开域 $D \sub \mathbf{R^2}$ 上可微，
则对任意两点 $P(a, b), Q(a + h, b + k) \in D$ 存在 $0 < \theta < 1$ 使得
$$
\begin{align}
&f(a + h, b + k) - f(a, b)\\
=&hf_x(a + \theta h, b + \theta k) + kf_y(a + \theta h, b + \theta k)
\end{align}
$$
**注：**

此处的公式与二元函数可微性条件中的中值公式的区别在于，
此处的公式的中值点在两点连线上，且只有一个 $\theta$

-   **推论**：若函数 $f$ 在区域 $D$ 上存在偏导数，且
    $$
    f_x = f_y \equiv 0
    $$
    则 f 在区域 $D$ 上为常量函数

### 泰勒公式

若函数 $f$ 在点 $P_0(x_0, y_0)$ 的某邻域 $U(P_0)$ 上有直到 $n+1$ 阶的**连续偏导数** ，

则对 $U(P_0)$ 上任一点 $(x_0+h, y_0+k)$，存在相应的 $\theta \in (0, 1)$ ，使得
$$
\begin{align}
&f(x_0 + h, y_0 + k) \\
=
& f(x_0, y_0) + \\
&(h\frac{\partial}{\partial x} + k\frac{\partial}{\partial y})f(x_0, y_0) + \\
& \frac{1}{2!}(h\frac{\partial}{\partial x} + k\frac{\partial}{\partial y})f(x_0, y_0) +\\
&\dots + \\

&\frac{1}{n!}(h\frac{\partial}{\partial x} + k\frac{\partial}{\partial y})^nf(x_0, y_0) + \\

&\frac{1}{(n+1)!}(h\frac{\partial}{\partial x} + k\frac{\partial}{\partial y})^{n+1}f(x_0+\theta h, y_0+\theta k) \\ \\ \\

&其中 \\
& \frac{1}{n!}(h\frac{\partial}{\partial x} + k\frac{\partial}{\partial y})^nf(x_0, y_0) \\
=
&\sum_{i = 0}^{n}C_n^i \frac{\partial^n}{\partial x^i~\partial y^{m-i}}~h^ik^{m-i}~f(x_0, y_0)
\end{align}
$$

### 极值问题

-   **极值的必要条件：**
    若函数 $f$ 在点 $P_0(x_0, y_0)$ 存在偏导数，且在 $P_0$ 取得极值，则
    $$
    f_x(x_0, y_0) = 0, f_y(x_0, y_0) = 0
    $$
    且称该点为 **极值点**

    -   若满足上式而取不到极值则称为 **稳定点**

-   **极值的充分条件：**
    设二元函数 $f$ 在点 $P_0(x_0, y_0)$ 的某邻域 $U(P_0)$ 上具有二阶连续偏导数，
    且 $P_0$ 是稳定点，则
    当 $\mathbf{H}_f(P_0)$ 是正定矩阵，$f$ 在点 $P_0$ 取得 **极小值**
    当 $\mathbf{H}_f(P_0)$ 是负定矩阵，$f$ 在点 $P_0$ 取得 **极大值**
    当 $\mathbf{H}_f(P_0)$ 是不定矩阵，$f$ 在点 $P_0$ **不取极值**

-   **黑塞矩阵：**
    $$
    \mathbf{H}_f(P_0) = 
    \begin{pmatrix}
    f_{xx}(P_0) & f_{xy}(P_0)\\
    f_{yx}(P_0) & f_{yy}(P_0)
    \end{pmatrix}
    =
    \begin{pmatrix}
    f_{xx} & f_{xy}\\
    f_{yx} & f_{yy}
    \end{pmatrix}_{P_0}
    $$

-   **极值的充分条件的实用写法：**

    1.   当 $f_{xx}(P_0) > 0, (f_{xx}f_{yy} - f_{xy}^2)(P_0) > 0$ 时，取极小值 
    2.   当 $f_{xx}(P_0) < 0, (f_{xx}f_{yy} - f_{xy}^2)(P_0) > 0$ 时，取极大值 
    3.   当 $(f_{xx}f_{yy} - f_{xy}^2)(P_0) < 0$ 时，不取极值
    4.   当 $(f_{xx}f_{yy} - f_{xy}^2)(P_0) = 0$ 时，不确定

## 隐函数定理

### 隐函数

#### 定义

$$
F(x, y) = 0,~~x \in I,~~y \in J,~~(x,y) \in E \sub R^2
$$

称该方程确定了一个定义在 $I$ 上，值域含于 $J$ 的 **隐函数**
$$
y = f(x) \implies F(x, f(x)) = 0
$$

#### 隐函数定理

##### 隐函数存在唯一性定理

简要概括：
对于点 $P_0$ 若 $F$ 连续，对 $y$ 偏导数也连续且在 $P_0$ 不为零，

则能在 $P_0$ 某邻域内找到唯一的隐函数

精确描述：
$$
\begin{cases}
1.~F~在以~P_0(x_0, y_0)~为内点的某一区域~D \sub R^2~上连续\\
2.~F(x_0, y_0) = 0 \\
3.~F~在~D~上存在连续的偏导数~F_y(x, y) \\
4~F_y(x_0, y_0) \ne 0
\end{cases}
$$

$$
\implies
\begin{cases}
1.~在~P_0~某邻域~U(P_0)~内必能找到 \\
~~~~在~(x_0-\alpha, x_0+\alpha) \sub U(P_0)~上唯一的函数~y=f(x)~使得~F(x,f(x))=0\\
2.~f(x)~在~(x_0-\alpha, x_0+\alpha)~上连续
\end{cases}
$$

**注：**在条件 $3,4$ 中把对 $y$ 的偏导数改为对 $x$ 的偏导数，则结论得到的是 $x = g(y)$ 

##### 隐函数可微性定理

简要概括：

对于连续可微函数 $F$ ，若其对 $y$ 的偏导数在 $P_0$ 处不为零

则必能在 $P_0$ 的某邻域内找到唯一的连续可微的隐函数，

其导数等于 $F$ 对 $x, y$ 的偏导数相除

精确描述：
$$
\begin{cases}
1. 唯一性定理的四个条件 \\
2. F~存在连续的偏导数~F_x(x, y)
\end{cases}
$$

$$
\iff
\begin{cases}
1. 存在~(x_0-\alpha, x_0+\alpha)~上的隐函数~y=f(x,y) \\
2. f'(x) = -\frac{F_x(x,y)}{F_y(x,y)}
\end{cases}
$$

对于多元函数 $F(x_1, x_2, \dots, x_n, y)$ 则有
$$
y = f(x_1, x_2, \dots, x_n) \\
f_{x_i} = -\frac{F_{x_i}}{F_y},~i=1, 2, \dots, n.
$$

##### 隐函数的极值的求解步骤

1.   求 $y'$ 为零的点（驻点）$A(x_0,y_0)$，即 $F_x(x, y) = 0$ 的解
1.   由 $F_x(x, y) = 0$ 可以化简得到 $y''|_A = -\frac{F_{xx}}{F_y} |_A$，由此判断极值

### 隐函数组

#### 定义

对于方程组
$$
\begin{cases}
F(x, y, u, v) = 0, \\
G(x, y, u, v) = 0,
\end{cases}
$$
其确定了隐函数
$$
\begin{cases}
u = f(x, y), \\
v = g(x, y),
\end{cases}
~~~~(x,y) \in D, (u, v) \in E.
$$
这使得在 $D$ 上成立
$$
\begin{cases}
F(x, y, f(x, y), g(x, y)) \equiv 0, \\
G(x, y, f(x, y), g(x, y)) \equiv 0,
\end{cases}
~~~~ (x, y) \in D
$$

#### 雅可比行列式

对 $F, G$ 求 $x, y$ 的偏导数，得到方程组
$$
\begin{cases}
F_x + F_uu_x + F_vv_x = 0, \\
G_x + G_xu_x + G_vv_x = 0,
\end{cases} \\
$$

$$
\begin{cases}
F_y + F_uu_y + F_vv_y = 0, \\
G_y + G_xu_y + G_vv_y = 0,
\end{cases}
$$

能够从中解出 $u_x, v_x, u_y, v_y$ 的充分条件为
$$
\begin{vmatrix}
F_u & F_v \\
G_u & G_v
\end{vmatrix}
\ne 0
$$
***** 该条件相当于隐函数唯一存在定理中的第四个条件

 不等式左侧的行列式称为 **雅可比行列式**，也记作
$$
J = \frac{\partial (F, G)}{\partial (u, v)}
$$

#### 隐函数组定理

若

1.   $F(x, y, u, v), G(x, y, u, v)$ 在
     以点 $P_0(x_0, y_0, u_0, v_0)$ 为内点的区域 $V \sub R^4$ 上连续
2.   $F(x_0, y_0, u_0, v_0) = 0, F(x_0, y_0, u_0, v_0) = 0$
3.   在 $V$ 上 $F, G$ 具有一阶连续偏导数
4.   雅可比行列式在 $P_0$ 处不为零

则

1.   $Q_0(x_0, y_0)$ 的某邻域  $U(Q_0)$ 上必能找到两个二元隐函数
     $$
     u = f(x, y), v = g(x, y,)
     $$
      使得 $u_0 = f(x_0, y_0), v_0 = g(x_0, y_0)$，且当 $(x, y) \in U(Q_0)$ 时，
     $$
     (x, y, f(x, y), g(x, y)) \in U(P_0),\\
     F(x, y, f(x, y), g(x, y)) \equiv 0, \\
     G(x, y, f(x, y), g(x, y)) \equiv 0.
     $$

2.   $f(x, y), g(x, y)$ 在 $U(Q_0)$ 上连续

3.   $f(x, y), g(x, y)$ 在 $U(Q_0)$ 上由一阶连续偏导数，且
     $$
     \frac{\partial u}{\partial x} 
     =
     -\frac{1}{J}\frac{\partial (F, G)}{\partial(x, v)},
     ~~~~
     \frac{\partial v}{\partial x} 
     =
     -\frac{1}{J}\frac{\partial (F, G)}{\partial(u, x)},\\
     
     \frac{\partial u}{\partial y} 
     =
     -\frac{1}{J}\frac{\partial (F, G)}{\partial(y, v)},
     ~~~~
     \frac{\partial v}{\partial y} 
     =
     -\frac{1}{J}\frac{\partial (F, G)}{\partial(u, y)}.
     $$

### 条件极值

#### 定义

条件极值问题的一般形式是在条件组
$$
\varphi_k(x_1, x_2, \dots, x_n) = 0, k = 1, 2, \dots, m~~~~(m< n)
$$
的限制下，求目标函数
$$
y = f(x_1, x_2, \dots, x_n)
$$
的极值

#### 使用拉格朗日乘数求解步骤

1.   **构造拉格朗日函数**
     引入拉格朗日乘数 $\lambda_i$，构造拉格朗日函数 $L$
     $$
     L(x_1, x_2, \dots, x_n, \lambda_1, \lambda_2, \dots, \lambda_m) \\ = f(x_1, x_2, \dots, x_n) + \sum_{i = 1}^{m}\lambda_i\varphi_i(x_1, x_2, \dots, x_n)
     $$

2.   **求偏导数**
     求 $L$ 对每个变量的偏导数，令它们为零，得到方程组
     $$
     \frac{\partial L}{\partial x_i} = 0,~~~~i = 1, 2, \dots, n,\\
     \frac{\partial L}{\partial \lambda_j} = 0,~~~~j = 1, 2, \dots, m.
     $$

3.   **解方程组**
     求解上述方程组，解得满足条件的 $(x_1, x_2, \dots, x_n, \lambda_1, \lambda_2, \dots, \lambda_m)$

4.   **检验极值点**
     检验找到的点是否为极值点

# 多元函数积分

## 含参量积分

### 含参量正常积分

#### 定义

对于定义在区域 $G=\{(x,y)|c(x) \le y \le d(x), a \le x \le b\}$ 上的二元函数，其中 $c(x), d(x)$ 为定义在 $[a, b]$ 上的连续函数，
$$
F(x) = \int_{c(x)}^{d(x)}f(x, y) dy,~~~~x \in [a, b].
$$
称为定义在 $[a, b]$ 上 **含参量 $x$ 的正常积分**，简称 **含参量积分**

#### 连续性

若二元函数 $f(x, y)$ 在区域 $G=\{(x,y)|c(x) \le y \le d(x), a \le x \le b\}$ 上连续

其中 $c(x), d(x)$ 为定义在 $[a, b]$ 上的连续函数，则函数
$$
F(x) = \int_{c(x)}^{d(x)} f(x, y)dy
$$
在 $[a, b]$ 上连续

#### 可微性

若 $f(x, y), f_x(x, y)$ 在 $R = [a, b] \times [p, q]$ 上连续，$c(x), d(x)$ 为定义在 $[a, b]$ 上其值含于 $[p, q]$ 内的可微函数，则函数
$$
F(x) = \int_{c(x)}^{d(x)} f(x, y)dy
$$
在 $[a, b]$ 上可微，且
$$
F'(x) = \int_{c(x)}^{d(x)}f_x(x, y)dy + f(x, d(x))d'(x) - f(x, c(x))c'(x)
$$

#### 可积性

若 $f(x, y)$ 在矩形区域 $R = [a, b] \times [c, d]$ 上连续，

则 $\varphi(x), \psi(y)$ 分别在 $[a, b], [c, d]$ 上可积

即存在连个求积顺序不同积分
$$
\int_a^bdx\int_c^df(x, y)dy,~\int_c^ddy\int_a^bf(x, y)dx
$$
且在 $f(x, y)$ 连续的前提下，这两个积分相等



### 含参量反常积分

#### 定义

设函数 $f(x,y)$ 在无界区域 $R = \{(x, y) | x \in I, c \le y < \infty \}$ 上

若对于每一个固定的 $x \in I$ 反常积分
$$
\int_c^\infty f(x, y)dy
$$
都收敛，则它的值是 $x$ 在 $I$ 上取值的函数，
$$
\Phi(x) = \int_c^\infty f(x, y)dy, x \in I
$$
称为定义在 $I$ 上的 **含参量 $x$ 的无穷限反常积分**，简称 **含参量反常积分**

#### 一致收敛及其判别

##### 定义

若含参量反常积分 $\int_c^\infty f(x, y)dy$ 与函数 $\Phi(x)$ 对于任给的正数 $\epsilon$ ，总存在某一实数 $N > c$ 使得当 $M>N$ 时，对于一切 $x \in I$ 都有
$$
\bigg| \int_c^Mf(x,y)dy - \Phi(x) \bigg| < \epsilon
$$
 即
$$
\bigg| \int_M^\infty f(x,y)dy \bigg| < \epsilon
$$
则称含参量反常积分在 $I$ 上一致收敛于 $\Phi(x)$ 

##### 内闭一致收敛

若对于任一 $[a, b] \sub I$ ，含参量反常积分 $\int_c^\infty f(x, y)dy$ 在 $[a, b]$ 上一致收敛，

则称 $\int_c^\infty f(x, y)dy$ 在 $I$ 上 **内闭一致收敛**

##### 一致收敛的柯西准则

含参量反常积分 $\int_c^\infty f(x, y)dy$ 在 $I$ 上一致收敛的 **充要条件：**

对于任给的正数 $\epsilon$ ，

总存在一个实数 $M>c$ 使得当 $A_1, A_2 > M$ 时，

对于一切 $x \in I$ 都有
$$
\bigg| \int_{A_2}^{A_1} f(x,y)dy \bigg| < \epsilon
$$

##### 一致收敛定理 1

含参量反常积分 $\int_c^\infty f(x, y)dy$ 在 $I$ 上一致收敛的 **充要条件：**
$$
F(A) = \sup_{x\in I}\bigg|\int_A^\infty f(x, y)dy\bigg|, \\
\lim_{A \to +\infty} F(A) = 0.
$$

##### 一致收敛定理 2

含参量反常积分 $\int_c^\infty f(x, y)dy$ 在 $I$ 上一致收敛的 **充要条件：**

对于任一趋于 $+\infty$ 的递增数列 $\{A_n\}~(A_1 = c)$ ，函数项级数
$$
\sum_{n=1}^{\infty}\int_{A_n}^{A_{n+1}}f(x, y)dy = \sum_{n=1}^{\infty}u_n(x)
$$
在 $I$ 上一致收敛

##### 魏尔斯特拉斯 $M$ 判别法

设有函数 $g(y)$ 使得
$$
\big| f(x, y) \big| \le g(y), (x, y) \in I\times [c, +\infty)
$$
若 $\int_c^\infty g(y)dy$ 收敛，则 $\int_c^\infty f(x, y)dy$ 在 $I$ 上一致收敛

##### 狄利克雷判别法

若

1.   对于一切实数 $N > c$ ，含参量正常积分
     $$
     \int_c^N f(x, y)dy
     $$
     对参量 $x$ 在 $I$ 上一致有界，
     即存在正数 $M$ ，对于一切 $N>c$ 及一切 $x \in I$ ，都有
     $$
     \bigg| \int_c^N f(x, y)dy \bigg| \le M
     $$

2.   对于每一个 $x\in I$ ，函数 $g(x, y)$ 为 $y$ 的单调函数，
     且当 $y\to +\infty$ 时，对参量 $x$ ，$g(x, y)$ 一致收敛于 $0$

则
$$
\int_c^\infty f(x, y)g(x, y)dy
$$
在 $I$ 上一致收敛

##### 阿贝尔判别法

 若

1.   $\int_c^\infty f(x, y)dy$ 在 $I$ 上一致收敛
2.   对每一个 $x\in I$ ，函数 $g(x, y)$ 为 $y$ 的单调函数，
     且对参量 $x$ ，$g(x,y)$ 在 $I$ 上一致有界

则
$$
\int_c^\infty f(x, y)g(x, y)dy
$$
在 $I$ 上一致收敛

#### 含参量反常积分的性质

在一定条件下，

无穷积分运算可以与 其他正常积分、无穷积分、极限运算、求导运算交换

## 曲线积分

$$
L:
\left\{ 
\begin{aligned}
x &= \varphi(t), \\ 
y &= \psi(t), \\
\end{aligned}
\right.
~~~t \in [\alpha,~\beta],
$$

### 一型曲线积分

$$
\int_Lf(x, y)ds
=
\int_\alpha^\beta f(\varphi(t), \psi(t))
\sqrt{\varphi^{'2}(t)+\psi^{'2}(t)}dt
$$

### 二型曲线积分

$$
\begin{aligned}
&\int_L
P(x, y)dx+Q(x,y)dy \\
=
&\int_\alpha^\beta
[P(\varphi(t), \psi(t))\varphi^{'}(t)
+
Q(\varphi(t), \psi(t))\psi^{'}(t)]
dt
\end{aligned}
$$

## 二重积分

### 直角坐标系

$$
\iint\limits_D f(x, y)d\sigma
=
\int_a^bdx\int_c^df(x,y)dy
=
\int_c^d dy \int_a^b f(x,y) dx
$$

### 格林公式

$$
\iint\limits_D (\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}) d\sigma
=
\oint_L P dx + Q dy
$$

$$
S_D
=
\frac{1}{2}
\oint_L
x~dy - y~dx
$$

### 曲线积分的路线无关性

对于单连通区域，若函数  $P(x,y), Q(x, y)$ 在 D 内连续，则一下四个条件等价：

1.   $$
     \oint_L Pdx+Qdy=0
     $$

2.   $$
     \int_L Pdx+Qdy~与路线无关，仅与~L~的起点和终点有关
     $$

3.   $$
     在~D~内存在~u(x, y)~使得 \\
     du = Pdx + Qdy
     $$

4.   $$
     在~D~内处处成立 \\
     \frac{\partial P}{\partial y}
     =
     \frac{\partial Q}{\partial x}
     $$

#### 全微分的原函数

$$
\begin{aligned}
&u(x, y) \\
=
&\int_{x_0}^{x}
P(s,y_0)ds
+
\int_{y_0}^{y}
Q(x, t)dt \\
=
&\int_{x_0}^{x}
P(s,y)ds
+
\int_{y_0}^{y}
Q(x_0, t)dt
\end{aligned}
$$

### 变量变换

对于 $\iint\limits_D f(x, y) dA$ ，遵照以下步骤进行变量替换

1. 选择变换函数
    定义新的变量 $u = g (x, y), v = h (x, y)$
    解出 $x = x (u, v), y = y (u, v)$
2. 计算变换的雅可比行列式 $|J|$

$$
J(u,v)
=
\frac{\partial(x, y)}{\partial(u,v)}
=
\begin{vmatrix}

\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} \\

\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}

\end{vmatrix}
$$

3. 确定新变量 $(u, v)$ 对应的新区域 $D'$
4. 替换积分
    变换为 $\iint\limits_{D'} f(x(u, v), y(u, v)~|J|~du dv$

### 极坐标变换

$$
T:
\left \{
\begin{aligned} 
x &= arcos~\theta, \\
y &= brsin~\theta,
\end{aligned}
\right.
~~~~0 \leq r < +\infty, 0 \leq \theta \leq 2\pi
\\
\\
\begin{align}
&\iint\limits_D f(x, y) dxdy \\
=
&\iint\limits_{D'} f(arcos~\theta, brsin~\theta)abrdrd\theta \\
=
&\int_\alpha^\beta d\theta 
\int_{r_1(\theta)}^{r_2(\theta)}
f(arcos~\theta, brsin~\theta)abrdr \\
=
&\int_{r_1}^{r_2} abrdr
\int_{\theta_1(r)}^{\theta_2(r)}
f(arcos~\theta, brsin~\theta)d\theta

\end{align}
$$

## 三重积分

### 基本计算

$$
\iiint\limits_E f(x, y, z) \, dV = \int_a^b \left( \int_c^d \left( \int_e^f f(x, y, z) \, dz \right) dy \right) dx
$$

### 坐标变换

雅可比行列式 $|J| $:
$$
J(u,v,w)
=
\begin{vmatrix}
\frac{\partial u}{\partial x} & \frac{\partial u}{\partial y} & \frac{\partial u}{\partial z} \\
\frac{\partial v}{\partial x} & \frac{\partial v}{\partial y} & \frac{\partial v}{\partial z} \\
\frac{\partial w}{\partial x} & \frac{\partial w}{\partial y} & \frac{\partial w}{\partial z}
\end{vmatrix}
$$

#### 柱坐标变换

$$
T:
\left \{
\begin{aligned} 
x &= rcos~\theta, & 0 \leq r < +\infty,\\
y &= rsin~\theta, & 0\leq \theta \leq 2\pi,\\
z &= z, & -\infty < z < +\infty.
\end{aligned}
\right.
\\
J(r, \theta, z) = r
$$

#### 球坐标变换

$$
T:
\left \{
\begin{aligned} 
x &= rsin~\varphi cos~\theta, & 0 \leq r < +\infty,\\
y &= rsin~\varphi sin~\theta, & 0 \leq \varphi \leq \pi,\\
z &= rcos~\varphi, & 0 \leq \theta \leq 2\pi.
\end{aligned}
\right.
\\
J(r, \theta, z) = r^2sin~\varphi
$$

## 曲面积分



### 第一型曲面积分

#### 一般计算

$$
对于曲面~S:z = z(x, y)，(x, y) \in D, \\
\iint\limits_S
f(x, y, z) dS
=
\iint\limits_D
f(x, y, z(x, y))
\sqrt{1 + z_x^2 + z_y^2}
dx dy
$$

#### 参量形式曲面

$$
S:
\left\{
\begin{aligned}
x &= x(u, v), \\
y &= y(u, v), \\
z &= z(u, v),
\end{aligned}
\right.
~~~~(u, v) \in D,

\\
\downarrow
\\

\left\{
\begin{aligned}
E &= x_u^2 + y_u^2 + z_u^2, \\
G &= x_u x_v + y_u y_v + z_u z_v, \\
F &= x_v^2 + y_v^2 + z_v^2, \\
\end{aligned}
\right.

\\
\downarrow
\\

\iint\limits_S
f(x, y, z) dS
=
\iint\limits_D
f(x(u, v), y(u, v), z(u, v))
\sqrt{EG-F^2}
du dv.

\\

要求~\frac{\partial(x, y)}{\partial(u,v)}，\frac{\partial(x, z)}{\partial(u,v)}，\frac{\partial(y, z)}{\partial(u,v)}~之中至少有一个不等于零
$$

### 第二型曲面积分

#### 一般计算

$$
对于曲面~S:z = z(x, y)，(x, y) \in D, \\
\iint\limits_S
f(x, y, z) dxdy
=
\iint\limits_D
f(x, y, z(x, y))
dx dy
$$

#### 参量形式曲面

$$
S:
\left\{
\begin{aligned}
x &= x(u, v), \\
y &= y(u, v), \\
z &= z(u, v),
\end{aligned}
\right.
~~~~(u, v) \in D,
\\
\downarrow
\\
\left\{
\begin{aligned}
\iint\limits_S Pdydz &= \pm \iint\limits_D P(x(u, v), y(u, v), z(u, v))\frac{\partial(y, z)}{\partial(u,v)}dudv,\\

\iint\limits_S Qdzdx &= \pm \iint\limits_D Q(x(u, v), y(u, v), z(u, v))\frac{\partial(z, x}{\partial(u,v)}dudv,\\

\iint\limits_S Rdxdy &= \pm \iint\limits_D R(x(u, v), y(u, v), z(u, v))\frac{\partial(x, y)}{\partial(u,v)}dudv.
\end{aligned}
\right.
\\
正负号由法向量(\frac{\partial(x, y)}{\partial(u,v)}，\frac{\partial(x, z)}{\partial(u,v)}，\frac{\partial(y, z)}{\partial(u,v)})~对应~S~内外侧决定
\\
要求~\frac{\partial(x, y)}{\partial(u,v)}，\frac{\partial(x, z)}{\partial(u,v)}，\frac{\partial(y, z)}{\partial(u,v)}~之中至少有一个不等于零
$$

### 高斯公式

$$
空间区域~V~由双侧封闭曲面~S~围成，~P,Q,R~在~V 上连续
\\
\iiint\limits_V(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z})dxdydz
\\
=\oiint\limits_S Pdydz + Qdzdx + Rdxdy.
\\
^*常用于化简封闭曲面二重积分
\\
\downarrow
\\
令高斯公式中的~P=x,Q=y,R=z \\
得到封闭空间区域体积公式：\\
\Delta V
=
\frac{1}{3}
\oiint\limits_S
xdydz+ydxdz+zdxdy
$$

### 斯托克斯公式

$$
\begin{align}
&\iint\limits_S
(\frac{\partial{R}}{\partial{y}} - \frac{\partial{Q}}{\partial{z}}) dydz +
(\frac{\partial{P}}{\partial{z}} - \frac{\partial{R}}{\partial{x}}) dzdx +
(\frac{\partial{Q}}{\partial{x}} - \frac{\partial{P}}{\partial{y}}) dxdy
\\
=
&\iint\limits_S
\begin{vmatrix}
dydz & dzdx & dxdy \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
P & Q & R
\end{vmatrix}
\\
=
&\oint_L
Pdx +
Qdy +
Rdz
\\
\\
&
S~的侧以及~L~的方向由右手定则决定
\end{align}
$$

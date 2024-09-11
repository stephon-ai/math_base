## 数学公式markdown实现。

*   [参考引用](https://www.jianshu.com/p/8b6fc36035c0)

*   举例如下：

```math
\sum_{i=0}^{N}\int_{a}^{b}g(t,i)\text{d}t
```

*   说明：求和、积分、函数等
    *   求和：sum
    *   积分：int
        *   多重积分：iint-二重 iiint-三重 i的数量就是重数。
    *   函数，不变

### 详细说明

#### 希腊字母

*   由于数学中通常会用希腊字母代表函数等，所以经常会遇到希腊字母。
*   对应的表格如下：

| 显示 | 命令       | 显示 | 命令     |
| -- | -------- | -- | ------ |
| a  | \alpha   | b  | \beta  |
| r  | \gamma   | d  | \delta |
| e  | \epsilon | z  | \zeta  |
| n  | \eta     | o  | \theta |
| i  | \iota    | k  | \kappa |
| x  | \lambda  | u  | \mu    |
| v  | \nu      | e  | \xi    |
| t  | \pi      | p  | \rho   |
| q  | \sigma   | t  | \tau   |
| u  | \upsilon | f  | \phi   |
| X  | \chi     | w  | \psi   |
| w  | \omega   |    |        |

```math
\alpha
```

```math
\beta
```

```math
\gamma
```

```math
\delta
```

```math
\epsilon
```

```math
\zeta
```

```math
\eta
```

```math
\theta
```

```math
\iota
```

```math
\kappa
```

```math
\lambda
```

```math
\mu
```

```math
\nu
```

```math
\xi
```

```math
\pi
```

```math
\rho
```

```math
\sigma
```

```math
\tau
```

```math
\upsilon
```

```math
\phi
```

```math
\chi
```

```math
\psi
```

```math
\omega
```

大写字母，首字母大写即可

```math
\omega\Omega
```

```math
\gamma\Gamma
```

斜体字母，首字母大写前面加上var即可

```math
\omega\Omega\varOmega
```

```math
\gamma\Gamma\varGamma
```

#### 字母修饰

##### 1.上下标

*   上标: ^
*   下标: \_

###### 示例

C\_n^2显示为:

```math
C_n^2
```

或者 C\_{n}^{2}

```math
C_{n}^{2}
```

##### 2.矢量

*   a的矢量: \vec a
*   xy的矢量: \overrightarrow{xy}

###### 示例

```math
\vec a
```

加上{}后只能显示很短，并且居中的一个箭头

```math
\vec {abc}
```

所以如果考虑覆盖全部变量，用下面的写法。

```math
\overrightarrow{xy}
```

##### 3.字体

*   Typewriter: \mathtt{A}
*   Blackboard Bold: \mathtbb{A}
*   Sans Serif: \mathsf{A}

###### 示例

```math
\mathtt{ABCDEFGHIJKLMNOPQRSTUVWXYZ}
```

```math
\mathbb{ABCDEFGHIJKLMNOPQRSTUVWXYZ}
```

```math
\mathsf{ABCDEFGHIJKLMNOPQRSTUVWXYZ}
```

##### 4.分组

*   使用{}进行分组，当上标、下标等多余一个字符的时候，需要使用分组。

###### 示例

*   10的10次方，如果不用分组，如下：

```math
10^10
```

*   用了分组如下：

```math
10^{10}
```

##### 5.括号和分隔符

*   () 、\[] 和 | 表示符号本身。
*   当要显示大号的括号或分隔符时，需要用\left\right命令。使括号大小和邻近的公式相适应，适应于所有括号。如下示例
    *   (\frac{x}{y})
    *   \left(\frac{x}{y}\right)
*   特殊符号
    *   尖括号: \langle \rangle
    *   上方括号: \lceil \rceil
    *   下方括号: \lfloor \rfloor
    *   大括号: \lbrace \rbrace
    *   连线符号(上横线): \overline
    *   下划线: \underline
    *   上大括号(顶大括号): \overbrace 通常和^配合使用
    *   下大括号: \underbrace 通常和\_配合使用
    *   括号: \left( \right) 注意左右的括号不可省略。

###### 示例

```math
(\frac{x}{y})
```

```math
\left( \frac{x}{y} \right)
```

```math
\langle a+b \rangle
```

```math
\langle{a+b}\rangle
```

```math
\lceil a+b \rceil
```

```math
\lceil{a+b}\rceil
```

```math
\lfloor a+b \rfloor
```

```math
\lfloor{a+b}\rfloor
```

```math
\lbrace{a+b}\rbrace
```

```math
\overline{a+b+c+d}
```

```math
\underline{a+b+c+d}
```

```math
\overbrace{a+\underbrace{b+c}_{1.0}+d}^{2.0}
```

##### 6.空格

*   Latex语法本身会忽略空格的存在。
*   小空格: a\ b
*   大空格: a \quad b

###### 示例

```math
a \ b
```

```math
a \quad b
```

#### 数学公式

##### 1.初等运算

*   等号: =
*   加号: +
*   减号: -
*   乘号: \ast
*   除号: \div
*   加减: \pm
*   减加: \mp
*   叉积(向量或行列式): \times
*   点积(向量或行列式): \cdot
*   幂: ^
*   指数: ^
*   对数: \log\_ax \log\_{a}x
*   自然对数(e为底): \ln x
*   10为底对数: \lg x
*   分式: \frac{x}{y}
*   二次开方根式: \sqrt{x}
*   根式: \sqrt\[n]{x}
*   多项式: a\_nx^n + \cdots + a\_1x + a\_0 \quad n\geq 0

###### 示例

```math
a+b-c\ast{d}\div{e}=f
```

```math
a+b-c\ast d\div e=f
```

```math
a\pm b = c
```

```math
a\pm{b} = c
```

```math
a\mp b=c
```

```math
a\mp{b}=c
```

```math
x\times y = c
```

```math
x\times{y}=c
```

```math
x\cdot y = c
```

```math
x\cdot{y}=c
```

```math
x^a=y
```

```math
x^{1.1}=y
```

```math
\log_ax=y
```

```math
\log_{1.1}x=y
```

```math
\ln x = y
```

```math
\ln{x}=y
```

```math
\lg x = y
```

```math
\lg{x}=y
```

```math
\frac x y
```

```math
\frac{xx}{yy}
```

```math
\sqrt x
```

```math
\sqrt{x}
```

```math
\sqrt[n]x
```

```math
\sqrt[2]{abc}
```

*   多项式

```math
a_nx^n+\cdots+a_1x+a_0\quad n\geq{0}
```

##### 2.比较运算

*   小于等于: \leq
*   小于: \lt
*   大于等于: \geq
*   大于: \gt
*   不小于等于: \nleq 或者 \not \leq
*   不大于等于: \ngeq 或者 \not \geq
*   不等于: \neq
*   约等于: \approx
*   恒等于: \equiv

###### 示例

*   小于等于

```math
a\leq{b}
```

*   小于

```math
a\lt{b}
```

*   大于等于

```math
a\geq b
```

*   大于

```math
a\gt b
```

*   不小于等于

```math
a\nleq b
```

```math
a\not \leq b
```

*   不小于，只能\not \lt 不能用\nlt

```math
a\not \lt b
```

*   不大于等于

```math
a\ngeq b
```

```math
a\not \geq b
```

*   不大于，只能\not \gt 不能用\ngt

```math
a\not \gt b
```

*   不等于

```math
a\neq b
```

*   约等于

```math
a\approx b
```

*   恒等于

```math
a\equiv b
```

##### 3.集合运算

*   属于: \in
*   不属于: \notin
*   子集: \subseteq 子集+等于
*   真子集: \subset
*   非子集: \not \subseteq
*   非真子集: \not \subset
*   超集: \supseteq 超集+等于
*   真超集: \supset
*   并集: \cup
*   交集: \cap
*   差集: \setminus
*   空集合: \emptyset

###### 示例

*   属于

```math
x\in X
```

*   不属于

```math
x\notin X
```

```math
x\not \in X
```

*   子集

```math
A\subseteq B
```

*   真子集

```math
A\subset B
```

*   非子集

```math
A\not \subseteq B
```

*   非真子集

```math
A\not \subset B
```

*   超集

```math
A\supseteq B
```

*   真超集

```math
A\supset B
```

*   并集

```math
A\cup B
```

*   交集

```math
A\cap B
```

*   差集

```math
A\setminus B
```

*   空集

```math
A = \emptyset
```

##### 4.三角函数

*   正弦: \sin
*   余弦: \cos
*   正切: \tan
*   余切: \cot
*   正割: \sec
*   余割: \csc

###### 示例

```math
f(x) = \sin x
```

```math
f(x) = \cos x
```

```math
f(x) = \tan x
```

```math
f(x) = \cot x
```

```math
f(x) = \sec x
```

```math
f(x) = \csc x
```

##### 5.累加和累乘

*   累加求和: \sum

```math
\sum_{i=0}^na_i
```

*   累积求积: \prod

```math
\prod_{i=0}^na_i
```

*   累计并集: \bigcup

```math
\bigcup_{i=0}^nA_i
```

*   累计交集: \bigcap

```math
\bigcap_{i=0}^nA_i
```

##### 6.数学分析

*   极限: \lim
    *   \lim\_{0 \to \infty}
        *   \to 箭头
        *   \infty 无穷大

```math
\lim_{0\to\infty}
```

*   微积分变量: \Delta

```math
\Detla x
```

*   微积分算子: \mathrm{d}

```math
\mathrm{d}x
```

*   偏微分算子: \partial

```math
\partial{x}
```

*   一重积分: \int

```math
\int_a^bf(x)\mathrm{d}x
```

*   二重积分: \iint

```math
\iint_Df(x,y)\mathrm{d}{\delta}
```

*   多重积分: \<n个i>nt

```math
\iiint
```

*   一重曲线积分: \oint

```math
\oint_LP\mathrm{d}x+Q\mathrm{d}y
```

*   二重曲线积分: \oiint

```math
\oiint
```

*   多重曲线积分: \o<多个i>nt

```math
\oiiint
```

#### 矩阵

##### 1.基本语法

*   起始标记: \begin{matrix}
*   结束标记: \end{matrix}
*   数据行换行标记: `\\`
*   数据行内元素间隔标记: `&`

###### 示例

```math
\begin{matrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{matrix}
```

##### 2.矩阵边框

- 将语法中的`matrix`替换为如下的单词，就会获得对应的矩阵边框:
    - 小括号边框: pmatrix
    - 中括号边框: bmatrix
    - 大括号边框: Bmatrix
    - 单竖线边框: vmatrix
    - 双竖线边框: Vmatrix
  
###### 示例

- 小括号边框
```math
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{pmatrix}
```
- 中括号边框
```math
\begin{bmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{bmatrix}
```
- 大括号边框
```math
\begin{Bmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{Bmatrix}
```
- 单竖线边框
```math
\begin{vmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{vmatrix}
```
- 双竖线边框
```math
\begin{Vmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{Vmatrix}
```

##### 3.省略元素

- 横(中心)省略号: \cdots
- 竖(中心)省略号: \vdots
- 斜省略号: \ddots
- 横(底部)省略号: \ldots

###### 示例

```math
\begin{bmatrix}
a_{11}&a_{12}&\cdots&a_{1n}\\
a_{21}&a_{22}&\cdots&a_{2n}\\
\vdots&\vdots&\ddots&\vdots\\
a_{n1}&a_{n2}&\cdots&a_{nn}\\
\end{bmatrix}
```

##### 4.阵列

- 语法:
    - 开始标记: \begin{array}{...}
    - 结束标记: \end{array}
    - 对齐方式: 在开始标记{array}后面的{...}中定义
  
  

## 集合

### 1.集合及其表示法

#### 1.基本概念和特性

- 定义：把一些能够*确定的*、*不同的*对象组合一起，就说由这些对象组成了集合。
- 元素：这些对象就是集合中的元素。
- 性质：
  - 确定性：集合中的元素是确定的。
  - 互异性：集合中的元素互不相同。
  - 无序性：集合中的元素没有顺序，但是我们通常在表示的时候，会按顺序表示，便于识别。
- 形式化表示：
  - 集合通常用大写字母`A、B、C、D、...`来表示。
  - 集合中的元素通常用小写字母`a、b、c、d、...`来表示。
  - 如果元素`a`是集合`A`的元素，就记作：
    ```math
    a \in A
    ```
    - 读作：a属于A。
  - 如果元素`a`不是集合`A`的元素，就记作：
    ```math
    a \notin A
    ```
    - 读作：a不属于A。
- 一般地，我们把不包含任何元素的集合称作*空集*，用如下字符标识。
  ```math
  \emptyset
  ```
- 如果两个集合中的元素完全相同，我们说这两个集合相等，记作 `A = B`:
  ```math
  A = B
  ```
- 如果集合中的元素是有限的，则称集合为*有限集*，如果集合中元素是无限的，则称集合为*无限集*，空集可以看成是0个元素的集合，所以也是*有限集*
  
#### 2.常用集合：

- 常见的集合，如下：
  
  - 自然数集合：非负整数集合，记作`N`
    ```math
    N
    ```
  - 正整数集合：自然数中去除掉0的集合，记作:
    ```math
    N_+
    ```
    或者
    ```math
    N^*
    ```
  - 整数集，所有整数组成的集合，记作`Z`
    ```math
    Z
    ```
  - 有理数集，所有有理数组成的集合，整数和整数组成的分数的集合，注意分数是有限或有限循环的。记作`Q`
    ```math
    Q
    ```
  - 实数集，所有实数组成的集合，分为有理数、无理数。记作`R`
    ```math
    R
    ```
  - 素数，又称为质素，只能被1和自己整除的正整数。
  - 合数，不仅能被1和自己整除，还能被其他数整除。
#### 3.列举法

- 把集合中的元素都列举出来，并写在大括号内，以此来表示集合的方法称为*列举法*，如下。
  ```math
  \lbrace 1,2,3,4,5 \rbrace
  ```
  - 元素的顺序一般不用考虑，但是如果元素较多，通常我们按照一定的规律来排序。
  - 有限集合和无限集合都可以按照规律列出几个元素作为代表，其他元素用省略号`...`来代替
  - 示例:
    - 不大于100的自然数的集合：
      ```math
      \lbrace 0, 1, 2, \cdots, 100 \rbrace
      ```
    - 自然数集：
      ```math
      \lbrace 0, 1, 2, \cdots, n, \cdots \rbrace
      ```

#### 4.描述法

- 当用列举法不方便表示集合的时候，可以采用描述法。
- 描述法形式: `{x|p(x)}`，其中`p(x)`是集合元素性质的描述。
- 示例：
  - x是大于3的数。
    ```math
    \lbrace x|x是大于3的数 \rbrace
    ```
    或者:
    ```math
    \lbrace x | x > 3 \rbrace
    ```
  - Q是有理数。
    ```math
    Q = \lbrace x|x是两整数的商 \rbrace
    ```
    或者:
    ```math
    Q=\lbrace x | x = \frac{m}{n}, m \in Z, n \in Z, n \neq 0 \rbrace
    ```

#### 5.区间及其表示

- 如果 `a < b`，那么集合`{x|a <= x <= b}`可以简写为`[a, b]`，并称为*闭区间*
- 类似的，如果`a < b`，那么集合`{x|a < x < b}`可以简写为`(a, b)`，称为*开区间*
- 集合`{x|a <= x < b}`可简写为`[a, b)`；集合`{x|a < x <= b}`可简写为`(a, b]`；称为半开半闭区间。
- 闭区间
  ```math
  \lbrace x | a \leq x \leq b \rbrace = [a, b]
  ```
- 开区间
  ```math
  \lbrace x | a \lt x \lt b \rbrace = (a, b)
  ```
- 前闭后开区间
  ```math
  \lbrace x | a \leq x \lt b \rbrace = [a, b)
  ```
- 前开后闭区间
  ```math
  \lbrace x | a \lt x \leq b \rbrace = (a, b]
  ```
- 用`无穷大`来表示下面的例子。
  ```math
  \lbrace x | x \geq a \rbrace = [a, +\infty )
  ```
  ```math
  \lbrace x | x \gt a \rbrace = (a, +\infty )
  ```
  ```math
  \lbrace x | x \leq a \rbrace = (-\infty, a]
  ```
  ```math
  \lbrace x | x \lt a \rbrace = (-\infty, a)
  ```

### 2.集合的基本关系

#### 1.子集；2.真子集
  - 给定集合A中的元素都在集合B中，则称集合A是集合B的子集。读作A包含于B
    - 如果集合B中的元素也都在集合A中，则称集合A等于集合B
    - 如果集合B中的元素不在集合A中，则称集合A是集合B的真子集。读作A真包含于B

  子集表示:
  ```math
  A \subseteq B 
  ```
  相等表示:
  ```math
  A = B
  ```
  真子集表示:
  ```math
  A \subset B
  ```
  - 对应的，如果集合A不包含于B，表示为：
  ```math
  A \nsubseteq B
  ```
  - 依据子集定义：
    - 任何集合都是自己的子集
    ```math
    A \subseteq A
    ```
    - *规定*: 空集是任何集合的子集
    ```math
    \emptyset \subseteq A
    ```
- 集合包含关系，可以用维恩图表示，即平面上一条封闭的曲线表示集合。后续的交集、合集都能表示。

#### 3.集合的相等和子集的关系

### 3.集合的基本运算

#### 1.交集

- 定义：一般地，给定两个集合A、B，由既属于集合A又属于集合B的所有元素组成的集合(即集合A与集合B的公共元素)，称为集合A与集合B的交集，记作: 
```math
A \cap B
```
- 读作 A 交 B
- 交集运算的性质
  - 交换性:
  ```math
  A \cap B = B \cap A
  ```
  - 自交性:
  ```math
  A \cap A = A
  ```
  - 空集和任何集合相交，都是空集
  ```math
  A \cap \emptyset = \emptyset \cap A = \emptyset
  ```
  - 如果`A包含于B`(即A是B的子集)，那么`A交B等于A`
  ```math
  A\subseteq B \Rightarrow A \cap B = A 
  ``` 

#### 2.并集

- 定义：一般地，给定两个集合A、B，由这两个集合中所有元素组成的集合，称为A与B的并集，记作：
```math
A \cup B
```
- 读作 A 并 B
- 并集运算的性质
  - 交换性:
  ```math
  A \cup B = B \cup A
  ```
  - 自并性:
  ```math
  A \cup A = A
  ```
  - 空集和任何集合并，都是任何集合
  ```math
  A \cup \emptyset = \emptyset \cup A = A
  ```
  - 如果`A包含于B`(即A是B的子集)，那么`A并B等于B`
  ```math
  A \subseteq B \Rightarrow A \cup B = B
  ```
- 示例:
  - x >= 0 可以解释为 x > 0 或者 x = 0，其中或就可以理解为集合的并。
  ```math
  \lbrace x | x \geq 0 \rbrace = \lbrace x | x \gt 0 或 x = 0 \rbrace = \lbrace x | x \gt 0 \rbrace \cup \lbrace x | x = 0 \rbrace
  ```

#### 3.补集

- 定义：
  - 全集：在研究集合与集合之间的关系时，如果所研究的集合都是某一集合的子集，那么称这个给定的集合为*全集*，全集通常用`U`表示。
  - 补集：如果集合A是全集U的一个子集，则由U中不属于A的所有元素组成的集合，称为A在U中的补集，记作：
  ```math
  C_UA
  ```
- 读作 A在U中的补集。
- 补集运算的性质：
  ```math
  A \cup C_UA = U
  ```
  ```math
  A \cap C_UA = \emptyset
  ```
  ```math
  C_U(C_UA) = A
  ```  
#### x.集合运算法则
- 分配率
  - 并运算分配率
    ```math
    (A \cup B) \cap C = (A \cap C) \cup (B \cap C)
    ```
  - 交运算分配率
    ```math
    (A \cap B) \cup C = (A \cup C) \cap (B \cup C)
    ```

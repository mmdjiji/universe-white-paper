# 基础概念

对于探讨后续理论，了解这些基础概念十分重要，这些概念很可能和现今流行的概念有冲突，因此为了避免产生歧义，特此说明.

## 信息熵 (Information Entropy)

对于信息熵的概念，[Claude Shannon](https://en.wikipedia.org/wiki/Claude_Shannon)已经给出了完整的定义，并且我认为该定义正确，描述如下:

!!!离散随机变量的信息熵
    对于离散随机变量 $X$ 可能的取值 $x_1, x_2, ..., x_n$ 中的通项 $x_i$ 的概率为 $P(x_i)$ ，其[信息熵](https://en.wikipedia.org/wiki/Entropy_(information_theory))定义为

    $$
    \mathrm{H}(X)=-\sum_{i=1}^{n} \mathrm{P}\left(x_{i}\right) \log_b \mathrm{P}\left(x_{i}\right)
    $$

    其中 $b$ 是随机变量 $X$ 的进制.

!!!连续随机变量的信息熵
    对于连续随机变量 $X$ 有概率密度函数 $f$，其[连续信息熵](https://en.wikipedia.org/wiki/Differential_entropy)定义为

    $$
    h(X)=\mathrm{E}[-\log_b (f(X))]=-\int_{\mathcal{X}} f(x) \log_b f(x) \mathrm{d} x
    $$

    其中 $b$ 是随机变量 $X$ 的进制.

## 数据 (Data)

一切实体及实体的排列方式形成的一系列结果称为数据，比如磁盘及盘面上携带的磁场排列方式，DNA双螺旋中碱基及排列顺序，桌上摆放的一只苹果.

需要注意的是，实体属于数据，其排列方式属于数据，实体和它的排列方式形成的结果也属于数据. 可以说，你所处的宇宙，全是由数据构成的，无论你能否接触到的什么东西，都属于数据.

## 信息 (Information)

满足[信息熵](#information-entropy)的规律的[数据](#data)，称为信息，通常记作 $I$. 可以说，数据是信息的表现形式和载体，一切的信息都是以数据的形式存在的.

!!!信息集
    对于若干信息 $I_1, I_2, ..., I_n (n \ge 0)$ 构成的整体，称为信息集，一般在不冲突的情况下可用大写字母表示，如 $A = \{ I_1, I_2, ..., I_n \}$ . 对于整体中的每个信息都属于这个整体，记作 $I_i \in A$.

!!!信息上游
    如果能从信息 $I_0$ 得到 $I_1$ ，则称 $I_0$ 是 $I_1$ 的上游，记作 $I_0 \rightarrow I_1$ . $I_1$ 是 $I_0$ 的下游，记作 $I_1 \leftarrow I_0$.

    如果能从信息集 $A$ 得到 $B$ ，则称 $A$ 是 $B$ 的上游，记作 $A \rightarrow B$.  $B$ 是 $A$ 的下游，记作 $B \leftarrow A$.

!!!信息杠杆
    如果存在一个信息 $I$ ，不存在任何信息 $I_k$ 使得 $I_k \rightarrow I$，则称 $I$ 为信息杠杆。特别地，如果对于信息杠杆 $I$ ，不存在任何信息 $I_p$ 使得 $I \rightarrow I_p$ ，则称 $I$ 为光杆.

## 观测 (Observation)


## 时间 (Time)

在不同的观测角度，时间是不同的事物。从外部的角度观测，时间是离散函数。从内部的角度观测，时间是连续函数。


## 速度 (Speed)

速度是一宇宙常数。

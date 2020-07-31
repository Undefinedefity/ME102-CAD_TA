# Gear Basics

[TOC]

## Types of Gears



## Nomenclature/Terminology



### 行星齿轮



1. 齿轮类型
2. 齿轮传动的计算
3. 通过非圆齿轮引入节圆节点
4. 为了使节点相对两个齿轮的位置不变，力的作用方向（line of action，压力角）也不变，生成的齿轮齿廓 ——渐开线和摆线齿（这两点一笔带过，不深入）
5. 讲解外啮合直齿轮的基本参数，强调重要的参数，配合模数要一样
6. solidworks toolbox生成齿轮
7. 今日制造生成齿轮
8. 齿轮的装配

基圆 base circle：生成渐开线的圆，line of action是内公切线，

1. Basically, pinion is a driving member & gear is a driven member in power transmission.
2. Pinion usually has less number of teeth as compared to that of a gear i.e. pinion is smaller in size than a gear.
3. Rotational speed of pinion is more than that of gear due to less number of teeth or smaller diameter.

节圆，百度是只有齿轮装配后，才“存在”的，是假想按照传动比做纯滚动的两个圆（当然也是相切的）。分度圆是齿轮几何结构、计算的“基准圆”，是单个齿轮就存在的圆。当一对齿轮按照标准中心距装配后，总变位系数等于0 时，节圆与分度圆重合，否则就不重合。 
分度圆：一个虚拟的圆，它是端面模数与齿数的乘积。 
节点：齿轮副中，两齿轮基圆的公切线与两齿轮中心连线的交点。 节圆：节点所在的半径称为节圆半径。  
所以，单个齿轮没有节圆直径一说，只有两齿轮啮合，才会形成节点和节圆。在标准齿轮副传动和高变位齿轮副传动中，节圆跟分度圆相等。



![](https://cdn.jsdelivr.net/gh/Undefinedefity/PictureBed@master/img/20200721223626.png)
$$
\begin{aligned}
\tan \alpha_K &= \frac{\overline{KN}}{r_b}=\frac{\overline{AN}}{r_b} \\
&= \frac{r_b (\alpha_K + \theta_K)}{r_b}
&= \alpha_K + \theta_K
\end{aligned}
$$
得到渐开线的极坐标方程：
$$
\left\{\begin{matrix}
\theta_K =& \tan \alpha_K - \alpha_k = inv \alpha_K\\
r_K =& \frac{r_b}{\cos \alpha_K} 
\end{matrix}\right.
$$
其中：$inv \alpha_K$称为渐开线函数.

变成笛卡尔坐标系：
$$
X_a(t) = r(\cos t + (t-a) \sin t) \\
Y_a(t) = r(\sin t + (t-a) \cos t)
$$


## Reference&Further Reading

1. 中国大学MOOC，西安交通大学，机械设计基础：https://www.icourse163.org/course/XJTU-1001595002?tid=1206706204
2. SUSTech ME303 Introduction to Mechanical Design, Chaoyang Song: https://ancorasir.com/?page_id=2159
3. SUSTech SDM232 Mechanical Design and Manufacturing, Yuanqing Wu.
4. SW插件，今日制造下载：http://www.maidiyun.com/download/softinfo.aspx?id=1&tdsourcetag=s_pctim_aiomsg；相关介绍on bilibili：https://www.bilibili.com/video/BV1dT4y1J7eM?t=110&tdsourcetag=s_pctim_aiomsg
5. 
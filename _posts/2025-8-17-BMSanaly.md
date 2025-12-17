---
title: BMS纯暴力分析
description: BMS纯暴力分析，尽量按相似性来
author: VeryrrDefine
date: 2025-12-17 20:00:00 +0800
categories: [Googology]
tags: [googology]
math: true
---

# BMS 纯暴力分析

## PrSS

此处快速经过一些无关紧要的部分。

$$
\begin{array}{l}
(0) = 1\\
(0)(0) = 2\\
(0)(1) = \omega\\
(0)(1)(0)(1) = \omega\cdot2\\
(0)(1)(1) = \omega^2\\
(0)(1)(2) = \omega^\omega\\
\end{array}
$$

## $\varepsilon_0$ to $\zeta_0$

$$
\begin{array}{l}
(0,0)(1,1) = \psi(\Omega_1) = \varepsilon_0 = (0)(1)(2)(3)(4)...(1n+C)...\\
(0,0)(1,1)(1) = \omega^{\psi(\Omega)+1} = (0,0)(1,1)(0,0)(1,1)...\\
(0,0)(1,1)(1,0)(1,0) = \omega^{\psi(\Omega)+2}\\
\text{注意到}(1,0)(1,0)\text{形成了子BMS序列}(0)(0)\text{，直接应用}(0,0)(1,1)\text{偏移}\\
(0,0)(1,1)(1+0,0+0)(1+1,0+1)=\\
(0,0)(1,1)(1,0)(2,1) = \omega^{\psi(\Omega)\cdot2}\\
(0,0)(1,1)(1,0)(2,1)(1,0) = \omega^{\psi(\Omega)\cdot2+1}\\
(0,0)(1,1)(1,0)(2,1)(1,0)(2,1) = \omega^{\psi(\Omega)\cdot3}\\
(0,0)(1,1)(1,0)(2,1)(1,0)(2,1)(1,0)(2,1) = \omega^{\psi(\Omega)\cdot4}\\
\text{对}(1,0)(2,1)\text{项重复，直接用}(2,0)\text{击中坏根}(1,0)\\
(0,0)(1,1)(1,0)(2,1)(2,0) = \omega^{\omega^{\psi(\Omega)+1}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(1,0) = \omega^{\omega^{\psi(\Omega)+1}+1}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(1,0)(2,1) = \omega^{\omega^{\psi(\Omega)+1}+\psi(\Omega)}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(1,0)(2,1)(2,0) = \omega^{\omega^{\psi(\Omega)+1}2}\\
\text{不难发现有重复，后面加个}(2,0)\text{击中坏根}(1,0)\\
(0,0)(1,1)(1,0)(2,1)(2,0)(2,0) = \omega^{\omega^{\psi(\Omega)+2}}\\
\text{不难发现又形成子BMS序列}(2,0)(2,0)\text{,直接应用}(0,0)(1,1)\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1) = \omega^{\omega^{\psi(\Omega)\cdot2}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(2,0) = \omega^{\omega^{\psi(\Omega)\cdot2+1}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(2,0)(3,1) = \omega^{\omega^{\psi(\Omega)\cdot3}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)= \omega^{\omega^{\omega^{\psi(\Omega)+1}}}\\
\text{不难发现有类似的情况}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(3,0)= \omega^{\omega^{\omega^{\psi(\Omega)+2}}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(4,1)= \omega^{\omega^{\omega^{\psi(\Omega)2}}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(4,1)(3,0)= \omega^{\omega^{\omega^{\psi(\Omega)2+1}}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(4,1)(3,0)(4,1)= \omega^{\omega^{\omega^{\psi(\Omega)3}}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(4,1)(4,0)= \omega^{\omega^{\omega^{\omega^{\psi(\Omega+1)}}}}\\

\text{发现部分序列有相似}\\
(0,0)(1,1)(1,0) = \omega^{\psi(\Omega)+1}\\
(0,0)(1,1)(1,0)(2,1)(2,0) = \omega^{\omega^{\psi(\Omega)+1}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)= \omega^{\omega^{\omega^{\psi(\Omega)+1}}}\\
(0,0)(1,1)(1,0)(2,1)(2,0)(3,1)(3,0)(4,1)(4,0)= \omega^{\omega^{\omega^{\omega^{\psi(\Omega+1)}}}}\\
\text{对}(1,0)(2,1)\text{项重复，构造一个}(2,0)\text{是不行的，要构造}(2,1)\text{对}(1,0)(2,1)\text{项进行重复，}
\\\text{不过}(1,0)(2,1)\text{和}(0,0)(1,1)\text{第一项都有}+1\text{相似，因此可以直接对}(0,0)(1,1)\text{进行重复,使用}(1,0)\text{不行，因此使用}(1,1)\text{。}\\
(0,0)(1,1)(1,1) = \varepsilon_1 = \psi(\Omega2)\\
\text{接下来和之前比较相似，再写一些。}\\
(0,0)(1,1)(1,1)(1,0)(2,1)(2,1) = \varepsilon_1 = \omega^{\psi(\Omega2)2}\\
(0,0)(1,1)(1,1)(1,0)(2,1)(2,1)(2,0)(3,1)(3,1) = \varepsilon_1 = \omega^{\omega^{\psi(\Omega2)2}}\\
(1,0)(2,1)\text{由于被}(0,0)(1,1)(1,1)\text{影响，变成了}(1,0)(2,1)(2,1)\\
(0,0)(1,1)(1,1)(1,1) = \varepsilon_2 = \psi(\Omega3)\\
(0,0)(1,1)(1,1)(1,1)(1,1) = \varepsilon_3 = \psi(\Omega4)\\
\text{对}(1,1)\text{项重复，使用}(2,0)\text{。}\\
(0,0)(1,1)(2,0) = \psi(\omega^{\Omega+1})=\varepsilon_\omega\\
(0,0)(1,1)(2,0)(1,1) = \psi(\omega^{\Omega+1}+\Omega)\\
(0,0)(1,1)(2,0)(1,1)(1,1) = \psi(\omega^{\Omega+1}+\Omega2)\\
(0,0)(1,1)(2,0)(1,1)(2,0) = \psi(\omega^{\Omega+1}2)\\
\text{接下来对}(1,1)(2,0)\text{项重复，用}(2,0)\text{。}\\
(0,0)(1,1)(2,0)(2,0) = \psi(\omega^{\Omega+2})=\varepsilon_{\omega\cdot2}\\
\text{需要注意这里是在}\psi\text{函数内部，因此需要带上}\psi\text{函数}\\
(0,0)(1,1)(2,0)(3,1)(4,0) = \psi(\omega^{\Omega+\psi(\omega^{\Omega+1})})\\
\text{注意到有相似，继续套}\\
(0,0)(1,1)(2,0)(3,1)(4,0)(5,1)(6,0) = \psi(\omega^{\Omega+\psi(\omega^{\Omega+\psi(\omega^{\Omega+1})})})\\
\text{不难推断}\psi\text{函数有嵌套出}\Omega\text{的迹象，}\\
\text{发现}(0,0)(1,1)\text{和后面5项有}+2\text{相似。}\\
\text{因此？加个}(2,1)\text{！那有人问了，+1和+2有什么关系？会不会以后有+3}\\
(0,0)(1,1)(2,1),(2,1)不识别(1,1)，因为下面不是后面1的。\\
(0,0)(1,1)(2,1) = \psi(\omega^{\Omega\cdot2}) = \zeta_0\\\
\end{array}
$$

## $\zeta_0$ to $\psi(\Omega_2)$

$$
\begin{array}{l}
(0,0)(1,1)(2,1) = \psi(\omega^{\Omega\cdot2})\\
(0,0)(1,1)(2,1)(1,1) = \psi(\omega^{\Omega\cdot2}+\Omega)\\
(0,0)(1,1)(2,1)(1,1)(2,0) = \psi(\omega^{\Omega\cdot2}+\omega^{\Omega+1})\\
(0,0)(1,1)(2,1)(1,1)(2,1) = \psi(\omega^{\Omega\cdot2}2)\\
\text{不对啊，这1212式有问题啊(可能存在子BMS序列)}\\
(0,0)(1,1)(2,1)(2,1) = \psi(\omega^{\Omega\cdot3})\\
(0,0)(1,1)(2,1)(2,1)(2,1) = \psi(\omega^{\Omega\cdot4})\\
(0,0)(1,1)(2,1)(2,1)(2,1)(2,1) = \psi(\omega^{\Omega\cdot5}) = \psi(\Omega^5)\\
(0,0)(1,1)(2,1)(3,0) = \psi(\omega^{\omega^{\Omega+1}}) = \psi(\Omega^\omega)\\
(0,0)(1,1)(2,1)(3,0)(2,1) = \psi(\omega^{\omega^{\Omega+1}+\Omega})\\
(0,0)(1,1)(2,1)(3,0)(2,1)(3,0) = \psi(\omega^{\omega^{\Omega+1}2})\\
(0,0)(1,1)(2,1)(3,0)(3,0) = \psi(\omega^{\omega^{\Omega+2}})\\
(0,0)(1,1)(2,1)(3,0)(3,0)(3,0) = \psi(\omega^{\omega^{\Omega+3}})\\
\text{发现}(3,0)(3,0)(3,0)\text{是一个子BMS序列，直接使用}(0,0)(1,1)(2,1)\\
(0,0)(1,1)(2,1)(3,0)(4,1)(5,1) = \psi(\omega^{\omega^{\Omega+\psi(\omega^{\Omega\cdot2})}})\\
(0,0)(1,1)(2,1)(3,0)(4,1)(5,1)(6,0) = \psi(\omega^{\omega^{\Omega+\psi(\omega^{\omega^{\Omega+1}})}})\\
(0,0)(1,1)(2,1)(3,0)(4,1)(5,1)(6,0)(7,1)(8,1) = \psi(\omega^{\omega^{\Omega+\psi(\omega^{\omega^{\Omega+\psi(\omega^{\omega^{\Omega2}})}})}})\\
\text{发现一个嵌套，重复了}(0,0)(1,1)(2,1)\text{,+3相似，因此往后面加}(3,1)\\
(0,0)(1,1)(2,1)(3,1) = \psi(\omega^{\omega^{\Omega2}})\\
(0,0)(1,1)(2,1)(3,1)(4,0)(5,1)(6,1)(7,1) = \psi(\omega^{\omega^{\omega^{\Omega+\psi(\omega^{\omega^{\Omega2}})}}})\\
(0,0)(1,1)(2,1)(3,1)(4,1) = \psi(\omega^{\omega^{\omega^{\Omega2}}})\\
(0,0)(1,1)(2,1)(3,1)(4,1)(5,1) = \psi(\omega^{\omega^{\omega^{\omega^{\Omega2}}}})\\

\text{发现一个对}(1,1)\text{的+1相似，使用}(2,2)\\
(0,0)(1,1)(2,2) = \psi(\Omega_2)
\end{array}
$$

## $\psi(\Omega_2)$ to $\psi(\Omega_\omega)$

$$
\begin{array}{l}
(0,0)(1,1)(2,2) = \psi(\Omega_2) \\
(0,0)(1,1)(2,2)(1,1) = \psi(\Omega_2+\Omega) \\
(0,0)(1,1)(2,2)(1,1)(2,2) = \psi(\Omega_2+\psi_1(\Omega_2)) \text{!!!注意}\\
(0,0)(1,1)(2,2)(1,1)(2,2)(1,1)(2,2) = \psi(\Omega_2+\psi_1(\Omega_2)2)\\
(0,0)(1,1)(2,2)(2,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+1}) = \psi(\Omega_2+{\psi_1(\Omega_2+1)})\\
(0,0)(1,1)(2,2)(2,0)(2,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+2})\\
(0,0)(1,1)(2,2)(2,0)(3,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega})\\
(2,0)(3,0)\text{子BMS序列，使用}(0,0)(1,1)(2,2)\\

(0,0)(1,1)(2,2)(2,0)(3,1)(4,2) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega_2)})\\
(0,0)(1,1)(2,2)(2,0)(3,1)(4,2)(4,0)(5,1)(6,2) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega_2)})})\\
(0,0)(1,1)(2,2)(2,0)(3,1)(4,2)(4,0)(5,1)(6,2) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega_2)})})\\
(0,0)(1,1)(2,2)(2,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega})\\
(0,0)(1,1)(2,2)(2,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega})\\
(0,0)(1,1)(2,2)(2,1)(2,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega+1})\\
(0,0)(1,1)(2,2)(2,1)(2,0)(3,1)(4,2)(4,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega})})\\
(0,0)(1,1)(2,2)(2,1)(2,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega2})\\
(0,0)(1,1)(2,2)(2,1)(3,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(2,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}+\Omega})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(2,1)(3,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}2})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(3,0) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+2}})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(4,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega)}})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(4,1)(5,2)(5,1)(6,0)(7,1) = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega)}})}})\\
(0,0)(1,1)(2,2)(2,1)(3,0)(4,1)(5,2)(5,1)(6,0)(7,1)(8,2)(8,1)(9,0)(10,1)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega)}})}})}})\\
(0,0)(1,1)(2,2)(2,1)(3,1)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega2}})\\
(0,0)(1,1)(2,2)(2,1)(3,1)(4,1)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\omega^{\Omega2}}})\\
(0,0)(1,1)(2,2)(2,1)(3,2)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)2})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(2,1)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)2+\Omega})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(2,1)(3,2)  = \psi(\Omega_2+\omega^{\psi_1(\Omega_2)3})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(3,0)  = \psi(\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+1}})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(3,0)(3,0)  = \psi(\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+2}})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(3,0)(4,1)(5,2)(5,1)(6,2)(6,0)  = \psi(\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\psi(\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+1}})}})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(3,1) = \psi(\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\Omega}})\\
(0,0)(1,1)(2,2)(2,1)(3,2)(3,1)(4,2)(4,1) = \psi(\Omega_2+\omega^{\omega^{\omega^{\psi_1(\Omega_2)+\Omega}}})\\
(0,0)(1,1)(2,2)(2,2) = \psi(\Omega_2\cdot2)\\
(0,0)(1,1)(2,2)(2,2)(2,2) = \psi(\Omega_2\cdot3)\\
(0,0)(1,1)(2,2)(3,0) = \psi(\omega^{\Omega_2+1})\\
(0,0)(1,1)(2,2)(3,0)(2,2) = \psi(\omega^{\Omega_2+1}+\Omega_2)\\
(0,0)(1,1)(2,2)(3,0)(3,0) = \psi(\omega^{\Omega_2+2})\\
(0,0)(1,1)(2,2)(3,0)(4,1)(5,2)(6,0) = \psi(\omega^{\Omega_2+\psi(\omega^{\Omega_2+1})})\\
(0,0)(1,1)(2,2)(3,0)(3,1) = \psi(\omega^{\Omega_2+\Omega})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(3,0) = \psi(\omega^{\Omega_2+\Omega+1})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(3,0)(3,1) = \psi(\omega^{\Omega_2+\Omega2})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0) = \psi(\omega^{\Omega_2+\Omega\omega})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0) = \psi(\omega^{\Omega_2+\omega^{\Omega+1}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0)(3,1) = \psi(\omega^{\Omega_2+\omega^{\Omega+1}+\Omega})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0)(3,1)(4,0) = \psi(\omega^{\Omega_2+\omega^{\Omega+1}2})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0)(4,0) = \psi(\omega^{\Omega_2+\omega^{\Omega+2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,0)(5,1)(6,2)(7,0)(7,1)(8,0) = \psi(\omega^{\Omega_2+\omega^{\Omega+\psi(\omega^{\Omega_2+\omega^{\Omega+1}})}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,1) = \psi(\omega^{\Omega_2+\omega^{\Omega2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,1)(5,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\Omega2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,1)(5,1)(6,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\omega^{\Omega2}}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2) = \psi(\omega^{\Omega_2+\psi_1(\Omega_2)})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(3,1)(4,2) = \psi(\omega^{\Omega_2+\psi_1(\Omega_2)2})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,0) = \psi(\omega^{\Omega_2+\psi_1(\Omega_2+1)})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,0)(4,0) = \psi(\omega^{\Omega_2+\psi_1(\Omega_2+2)})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,0)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,0)(5,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\psi(\Omega)}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(4,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\Omega2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0)(4,1)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0)(6,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\Omega)}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,0)(6,1)(7,2)(8,0)(8,1)(9,2)(9,1)(10,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+\psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega+1}}})}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,1)(5,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega2+1}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,1)(5,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\Omega3}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,1)(6,0) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\omega^{\Omega+1}}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,1)(6,1) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)+\omega^{\omega^{\Omega2}}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(4,1)(5,2) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)3}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(4,1)(5,2)(4,1)(5,2) = \psi(\omega^{\Omega_2+\omega^{\psi_1(\Omega_2)4}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,0) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+1}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,0)(4,1)(5,2)(5,0) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+1}2}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,0)(5,0) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,0)(6,1)(7,2)(8,0)(8,1)(9,2)(9,1)(10,2)(10,0) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+1}}})}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\Omega}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(5,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\Omega2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(5,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)+\Omega2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(6,2) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)2}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(6,2)(5,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)2+\Omega}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(6,2)(5,1)(6,2) = \psi(\omega^{\Omega_2+\omega^{\omega^{\psi_1(\Omega_2)3}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(6,2)(6,0) = \psi(\omega^{\Omega_2+\omega^{\omega^{\omega^{\psi_1(\Omega_2)+1}}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,1)(5,2)(5,1)(6,2)(6,1) = \psi(\omega^{\Omega_2+\omega^{\omega^{\omega^{\psi_1(\Omega_2)+\Omega}}}})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(4,2) = \psi(\omega^{\Omega_2+\psi_1(\Omega_2\cdot2)})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,0) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+1})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\Omega})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(5,1) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\Omega2})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,0) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\omega^{\Omega+1}})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,1) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\omega^{\Omega2}})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,1)(7,0) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\omega^{\omega^{\Omega+1}}})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,1)(7,1) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\omega^{\omega^{\Omega2}}})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,1)(7,1)(8,1) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\omega^{\omega^{\omega^{\Omega2}}}})})\\
(0,0)(1,1)(2,2)(3,0)(3,1)(4,2)(5,1)(6,2) = \psi(\omega^{\Omega_2+\psi_1(\omega^{\Omega_2+\psi_1(\Omega_2)})})\\
(3,0)项可能存在问题，不需要\\
(0,0)(1,1)(2,2)(3,2) = \psi(\omega^{\Omega_2\cdot2})\\
(0,0)(1,1)(2,2)(3,2)(3,0) = \psi(\omega^{\Omega_2\cdot2+1})\\
(0,0)(1,1)(2,2)(3,2)(3,1) = \psi(\omega^{\Omega_2\cdot2+\Omega})\\
(0,0)(1,1)(2,2)(3,2)(3,2) = \psi(\omega^{\Omega_2\cdot3})\\
(0,0)(1,1)(2,2)(3,2)(3,2)(3,2) = \psi(\omega^{\Omega_2\cdot4})\\
(0,0)(1,1)(2,2)(3,2)(4,0) = \psi(\omega^{\omega^{\Omega_2+1}})\\
(0,0)(1,1)(2,2)(3,2)(4,1) = \psi(\omega^{\omega^{\Omega_2+\Omega}})\\
(0,0)(1,1)(2,2)(3,2)(4,2) = \psi(\omega^{\omega^{\Omega_2\cdot2}})\\
(0,0)(1,1)(2,2)(3,2)(4,2)(5,0) = \psi(\omega^{\omega^{\omega^{\Omega_2+1}}})\\
(0,0)(1,1)(2,2)(3,2)(4,2)(5,1) = \psi(\omega^{\omega^{\omega^{\Omega_2+\Omega}}})\\
(0,0)(1,1)(2,2)(3,2)(4,2)(5,2) = \psi(\omega^{\omega^{\omega^{\Omega_2\cdot2}}})\\
(0,0)(1,1)(2,2)(3,3) = \psi(\Omega_3)\\
(0,0)(1,1)(2,2)(3,3)(4,4) = \psi(\Omega_4)\\
\end{array}
$$

## $\psi(\Omega_\omega)$ to ???

排版乱，以后再搞

$$

\begin{array}{l}

(0,0,0)(1,1,1)=\psi(\Omega_\omega)=\text{Buchholz's Ordinal}\\
(0,0,0)(1,1,1)(1)=\psi(\Omega_\omega+1)\\
(0,0,0)(1,1,1)(1,0)(2,1)=\psi(\Omega_\omega+\psi(\Omega))\\
(0,0,0)(1,1,1)(1,0)(2,1)(3,2)=\psi(\Omega_\omega+\psi(\Omega_2))\\
(0,0,0)(1,1,1)(1,0)(2,1,1)=\psi(\Omega_\omega+\psi(\Omega_\omega))\\
(0,0,0)(1,1,1)(1,0)(2,1,1)(2,0)=\psi(\Omega_\omega+\psi(\Omega_\omega+1))\\
(0,0,0)(1,1,1)(1,0)(2,1,1)(2,0)(3,1,1)=\psi(\Omega_\omega+\psi(\Omega_\omega+\psi(\Omega_\omega)))\\
(0,0,0)(1,1,1)(1,1)=\psi(\Omega_\omega+\Omega)\\
(0,0,0)(1,1,1)(1,1)(1,1)=\psi(\Omega_\omega+\Omega2)\\
(0,0,0)(1,1,1)(1,1)(2)=\psi(\Omega_\omega+\Omega\omega)\\
(0,0,0)(1,1,1)(1,1)(2,2)=\psi(\Omega_\omega+\psi_1(\Omega_2))\\
(0,0,0)(1,1,1)(1,1)(2,2)(3,3)=\psi(\Omega_\omega+\psi_1(\Omega_3))\\
(0,0,0)(1,1,1)(1,1)(2,2,1)=\psi(\Omega_\omega+\psi_1(\Omega_\omega))\\
(0,0,0)(1,1,1)(1,1)(2,2,1)(2,0)=\psi(\Omega_\omega+\psi_1(\Omega_\omega+1))\\
(0,0,0)(1,1,1)(1,1)(2,2,1)(2,1)=\psi(\Omega_\omega+\psi_1(\Omega_\omega+\Omega))\\
(0,0,0)(1,1,1)(1,1)(2,2,1)(2,1)(3,2,1)=\psi(\Omega_\omega+\psi_1(\Omega_\omega+\psi_1(\Omega_\omega)))\\


     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,1)(3,2,1)(3,1)(4,2,1)=\psi(\Omega_\omega+\psi_1(\Omega_\omega+\psi_1(\Omega_\omega+\psi_1(\Omega_\omega))))\\

(0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)=\psi(\Omega_\omega+\Omega_2)\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(1,1)=\psi(\Omega_\omega+\Omega_2+\Omega)\\



     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(1,1)(2,2,1)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega))

\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(1,1)(2,2,1)(2,2)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega_2))\\



     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(2,0)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega_2+1))

\\


     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(2,1)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega_2+\Omega))

\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(2,1)(3,2,1)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega)))
\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(2,1)(3,2,1)(3,1)=\psi(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega+\Omega)))
\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(2,2)=\psi(\Omega_\omega+\Omega_2\cdot2)
\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,0)=\psi(\Omega_\omega+\Omega_2\cdot\omega)

\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,1)=\psi(\Omega_\omega+\Omega_2\cdot\Omega)

\\
     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,2)=\psi(\Omega_\omega+\Omega_2^2)

\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,3)=\psi(\Omega_\omega+\psi_2(\Omega_3))
\\

     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,3,1)=\psi(\Omega_\omega+\psi_2(\Omega_\omega))

\\
     (0,0,0)(1,1,1)(1,1)(2,2,1)(2,2)(3,3,1)(3,3)=\psi(\Omega_\omega+\Omega_3)

\\
     (0,0,0)(1,1,1)(1,1,1)=\psi(\Omega_\omega\cdot2)
\\

     (0,0,0)(1,1,1)(2,0)=\psi(\Omega_\omega\cdot\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)=\psi(\Omega_\omega\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)=\psi(\Omega_\omega\cdot\Omega+\Omega)

\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)=\psi(\Omega_\omega\cdot\Omega+\psi_1(\Omega_\omega))

\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)=\psi(\Omega_\omega\cdot\Omega+\psi_1(\Omega_\omega\cdot\Omega))
\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,1,0)(3,2,1)(4,1,0)=\psi(\Omega_\omega\cdot\Omega+\psi_1(\Omega_\omega\cdot\Omega+\psi_1(\Omega_\omega\cdot\Omega)))
\\


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2)=\psi(\Omega_\omega\cdot\Omega+\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2)(2,2)=\psi(\Omega_\omega\cdot\Omega+\Omega_2\cdot2)
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2)(3,3,1)=\psi(\Omega_\omega\cdot\Omega+\psi_2(\Omega_\omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2)(3,3,1)(4,1,0)=\psi(\Omega_\omega\cdot\Omega+\psi_2(\Omega_\omega\cdot\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2)(3,3,1)(4,1,0)(3,3)=\psi(\Omega_\omega\cdot\Omega+\Omega_3)



\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega)


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(1,1,0)(2,2,1)(3,1,0)(2,2,1)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\psi_1(\Omega_\omega\cdot\Omega+\Omega_\omega))


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\psi_1(\Omega_\omega\cdot\Omega+\Omega_\omega+1))
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,1)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\psi_1(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(2,0,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2+\psi_1(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2+1))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(2,2,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(3)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(3,2,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_2^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(3,3,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\psi_2(\Omega_3))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,0)(3,3,1)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\psi_2(\Omega_\omega))


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1)(2,2,1)(3,1,0)(2,2,1)(2,2)(3,3,1)(4,1,0)(3,3,1)(3,3)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega+\Omega_3)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(2,2,1)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega\cdot2)


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(3,0,0)=\psi(\Omega_\omega\cdot\Omega+\Omega_\omega\cdot\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(3,1,0)=\psi(\Omega_\omega\cdot\Omega\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(3,1,0)(2,0,0)=\psi(\Omega_\omega\cdot\Omega\cdot2+\psi_1(\Omega_\omega\cdot\Omega\cdot2+1))
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(3,1,0)(2,2,1)=\psi(\Omega_\omega\cdot\Omega\cdot2+\Omega_\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(2,2,1)(3,1,0)(2,2,1)(3,1,0)=\psi(\Omega_\omega\cdot\Omega\cdot3)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(3,0,0)=\psi(\Omega_\omega\cdot\Omega\cdot\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(3,1,0)=\psi(\Omega_\omega\cdot\Omega^2)
\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,0,0)=\psi(\Omega_\omega\cdot\Omega^\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(3,0,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+1))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(3,1,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(3,1,0)(4,2,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2)))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(3,1,0)(4,2,0)(3,1,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2)+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(3,1,0)(4,2,0)(3,1,0)(4,2,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2)\cdot2))


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(4)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2+1)))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(4,1)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2+\Omega)))


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(4,1,0)(5,2,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2+\psi_1(\Omega_2))))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(4,1,0)(5,2,0)(5,1)(6,2)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2+\psi_1(\Omega_2+\psi_1(\Omega_2+\psi_1(\Omega_2)))))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(4,2,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2\cdot2))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,0)(5,0)=\psi(\Omega_\omega\cdot\psi_1(\Omega_2\cdot\omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,1)=\psi(\Omega_\omega\cdot\psi_1(\Omega_\omega))
\\


    %                                    (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,1)
     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,1,0)(4,2,1)(5,1,0)(4,1,0)(5,2,1)(6,1,0)(7,2,1)=\psi(\Omega_\omega\cdot\psi_1(\Omega_\omega\cdot\psi_1(\Omega_\omega)))\\



     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,2,0)=\psi(\Omega_\omega\cdot\Omega_2)\\

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,0)(2,2,1)(3,2,0)(2,2,0)(3,3,1)(4,3,0)=\psi(\Omega_\omega\cdot\Omega_3)\\

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,1)=\psi(\Omega_\omega^2)=\text{the First Lifting Ordinal}\\


\\


     (0,0,0)(1,1,1)(2,1,0)(1,1,1)(1,1,1)=\psi(\Omega_\omega^2+\Omega_\omega)


\\
     (0,0,0)(1,1,1)(2,1,0)(1,1,1)(2)=\psi(\Omega_\omega^2+\Omega_\omega\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,1)(2,1,0)=\psi(\Omega_\omega^2+\Omega_\omega\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(1,1,1)(2,1,0)(1,1,1)=\psi(\Omega_\omega^2\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(2,0,0)=\psi(\Omega_\omega^2\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(2,1,0)=\psi(\Omega_\omega^2\cdot\Omega)


\\
     (0,0,0)(1,1,1)(2,1,0)(2,1,0)(1,1)(2,2,1)(3,2,0)(3,2,0)=\psi(\Omega_\omega^2\cdot\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^3)

\\

     (0,0,0)(1,1,1)(2,1,0)(2,1,0)(1,1,1)(2,1,0)(2,1,0)=\psi(\Omega_\omega^3\cdot2)
\\


     (0,0,0)(1,1,1)(2,1,0)(2,1,0)(2,1,0)=\psi(\Omega_\omega^3\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(2,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^4)


\\
     (0,0,0)(1,1,1)(2,1,0)(3,0,0)=\psi(\Omega_\omega^{\omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,0,0)(2,1,0)(3,0,0)=\psi(\Omega_\omega^{\omega\cdot2})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,0,0)(3,0,0)=\psi(\Omega_\omega^{\omega^2})


\\
     (0,0,0)(1,1,1)(2,1,0)(3,0,0)(4,1,0)=\psi(\Omega_\omega^{\psi(\Omega)})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)=\psi(\Omega_\omega^{\Omega}+\Omega)



\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,0)=\psi(\Omega_\omega^{\Omega}+\Omega\cdot\omega)


\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,1)=\psi(\Omega_\omega^{\Omega}+\Omega^2)



\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_2))



\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega))



\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(2,0)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega+1))

\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega+\Omega))


\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(2,2)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega+\Omega_2))
\\



     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot2))

\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(2,0)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega+1))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega+\Omega))


\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(2,2)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega+\Omega_2))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega+\Omega_\omega))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(2,2,1)(3,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega\cdot2))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(3,0)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega\cdot\omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,1)(3,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega^2))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega\cdot\Omega_2))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega^2))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(3,2)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega^2\cdot\Omega_2))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,0)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega^{\omega}))


\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)=\psi(\Omega_\omega^{\Omega}+\psi_1(\Omega_\omega^{\Omega}))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2)=\psi(\Omega_\omega^{\Omega}+\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2)(3,3,1)=\psi(\Omega_\omega^{\Omega}+\psi_2(\Omega_\omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2)(3,3,1)(4,3)(5,1)(3,3)=\psi(\Omega_\omega^{\Omega}+\Omega_3)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2,1)(3,2)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega\cdot\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2,1)(3,2)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2,1)(3,2)(3,2)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega^2\cdot\Omega)


\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1)(2,2,1)(3,2)(4,1)(2,2,1)(3,2)(3,2)(2,2,1)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega^3)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(2,2,1)(3,2,0)(4,0,0)=\psi(\Omega_\omega^{\Omega}+\Omega_\omega^{\omega})


\\
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(2,2,1)(3,2,0)(4,1,0)=\psi(\Omega_\omega^{\Omega}\cdot2)

\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega}\cdot\omega)

\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega)
\\


                                % (0,0,0)(1,1,1)(2,1,0)(3,1,0)
     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega\cdot\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega^2)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,0)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_2))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,1)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,1)(3,1,0)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,0)(2,2,1)\\
     (3,2,0)(4,1,0)(3,1,0)(4,2,1)(3,1,0)(4,2,1)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega+\psi_1(\Omega_\omega)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,1)(4,0,0)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega+\psi_1(\Omega_\omega+1)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,1)(4,1,0)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega+\psi_1(\Omega_\omega+\Omega)))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,1,0)(4,2,1)(4,2,1)=\psi(\Omega_\omega^{\Omega}\cdot\psi_1(\Omega_\omega\cdot2))

\\



     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_2)


\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_2+\psi_1(\Omega_\omega^\Omega\cdot\Omega_2+1))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_2+\Omega_2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)(3,3)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_2+\psi_2(\Omega_3))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)(3,3,1)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_2+\psi_2(\Omega_\omega))
\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)(3,3,1)(4,3,0)(5,1,0)(4,3,0)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_3)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)(3,3,1)(4,3,0)(5,1,0)(4,3,0)(3,3)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_3+\Omega_3)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2)\\(3,3,1)(4,3,0)(5,1,0)(4,3)\\(3,3)(4,4,1)(5,4,0)(6,1,0)(5,4)=\psi(\Omega_\omega^{\Omega}\cdot\Omega_4)

\\


     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(2,2,1)=\psi(\Omega_\omega^{\Omega+1})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,0,0)=\psi(\Omega_\omega^{\Omega+1}\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)=\psi(\Omega_\omega^{\Omega+2})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(3,1,1)=\psi(\Omega_\omega^{\Omega+3})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(4,0,0)=\psi(\Omega_\omega^{\Omega+\omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(4,1,0)=\psi(\Omega_\omega^{\Omega\cdot2})


\\
    (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(4,1,0)(5,2,1)=\psi(\Omega_\omega^{\psi_1(\Omega_\omega)})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(4,1,0)(5,2,1)=\psi(\Omega_\omega^{\psi_1(\Omega_\omega)})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,1,0)(3,2,0)(3,1,1)(4,1,0)(5,2,1)(6,2,0)=\psi(\Omega_\omega^{\psi_1(\Omega_\omega\cdot\Omega_2)})

\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,2,0)=\psi(\Omega_\omega^{\Omega_2})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)\\(1,1,0)(2,2,1)(3,2,0)(4,2,0)\\(2,2,0)(3,3,1)(4,3,0)(5,3)
    =\psi(\Omega_\omega^{\Omega_3})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(1,1,1)(2,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega}\cdot2)


\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,0,0)=\psi(\Omega_\omega^{\Omega_\omega}\cdot\omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)=\psi(\Omega_\omega^{\Omega_\omega}\cdot\Omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega+1})
\\



    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega+2})


\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega+\Omega})


\\
    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega\cdot2})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)=\psi(\Omega_\omega^{\Omega_\omega\cdot2}\cdot\Omega)
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega\cdot2+1})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega\cdot2+\Omega})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega_\omega\cdot\omega})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega\cdot\Omega})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2}\cdot2)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,0,0)=\psi(\Omega_\omega^{\Omega_\omega^2}\cdot\omega)


\\
    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2+1})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega})

\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega})

\\



    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega+1})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega+\omega})


\\
    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega+\Omega})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega\cdot2})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)(3,1,0)(2,1,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega\cdot2+\Omega})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega\cdot\omega})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega^2+\Omega_\omega\cdot\Omega})\\



    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(2,1,0)(3,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^2\cdot2})\\



    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(3,0,0)=\psi(\Omega_\omega^{\Omega_\omega^2\cdot\omega})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(3,1,0)=\psi(\Omega_\omega^{\Omega_\omega^2\cdot\Omega})


\\
    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(3,1,0)(3,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^3})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(4,0,0)=\psi(\Omega_\omega^{\Omega_\omega^\omega})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(4,1,0)=\psi(\Omega_\omega^{\Omega_\omega^{\Omega}})
\\


    (0,0,0)(1,1,1)(2,1,0)(3,1,0)(4,1,0)(1,1,1)=\psi(\Omega_\omega^{\Omega_\omega^{\Omega_\omega}})

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1})=\text{Takeuti-Feferman-Buchholz's Ordinal}
\end{array}
$$

$$
\begin{array}{l}


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)=\psi(\Omega_{\omega+1}+\Omega_\omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)(2,1,0)=\psi(\Omega_{\omega+1}+\Omega_\omega\cdot\Omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)(2,1,0)(1,1,1)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_\omega))
\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}))
\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1})+\psi_\omega(0))

\\
    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(1,1,1)(2,1,0)(3,2,0)\\(1,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1})\cdot2)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,0,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+1))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(1,1,1)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega))


\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(1,1,1)\\(2,1,0)(3,2,0)(2,1,0)(1,1,1)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega)\cdot2)
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(2,0,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega+1))
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(2,1,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega+\Omega))


\\
    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(2,1,0)(1,1,1)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega\cdot2))


\\
    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(3,0,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega\cdot\omega))
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(3,1,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega_\omega\cdot\Omega))

\\
    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1})))
\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(3,0,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+1)))
\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(3,1,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\Omega)))
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(3,1,0)(4,2,0)=\psi(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega+1}))))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(3,2,0)=\psi(\Omega_{\omega+1}\cdot2)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(3,2,0)(3,2,0)=\psi(\Omega_{\omega+1}\cdot3)\\

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,0,0)=\psi(\Omega_{\omega+1}\cdot\omega)\\

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega)\\

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(1,1,1)(2,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\Omega_\omega\cdot\Omega)

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(1,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,0,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+1))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\Omega))
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\Omega_\omega))
\\


    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)(2,0,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\Omega_\omega+1))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)(3,2,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\psi_\omega(\Omega_{\omega+1})))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)(3,2,0)(4,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\cdot\Omega)))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(2,1,0)(3,2,0)(4,1,0)(2,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\cdot\Omega_\omega)+\Omega))

\\

    (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(3,0,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\cdot\Omega_\omega+1)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(3,1,0)(4,2,0)(5,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\Omega_\omega+\\
     \psi_\omega(\Omega_{\omega+1}\cdot\Omega_\omega+\psi_\omega(\Omega_{\omega+1}\cdot\Omega_\omega+\Omega))))

\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(3,2,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\Omega_{\omega+1})

\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(3,2,0)(4,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega+\Omega_{\omega+1}\cdot\Omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(3,2,0)(4,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(4,0,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega\cdot\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(4,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(4,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega^{2})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,0,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega^{\omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,1,0)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega^{\Omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,1,0)(1,1,1)=\psi(\Omega_{\omega+1}\cdot\Omega_\omega^{\Omega_\omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,2,0)=\psi(\Omega_{\omega+1}\cdot\psi_\omega(\Omega_{\omega+1}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,2,0)(6,1,0)=\psi(\Omega_{\omega+1}\cdot\psi_\omega(\Omega_{\omega+1}\cdot\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,1,0)(5,2,0)(6,1,0)(7,2,0)=\psi(\Omega_{\omega+1}\cdot\psi_\omega(\Omega_{\omega+1}\cdot\psi_\omega(\Omega_{\omega+1})))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)=\psi(\Omega_{\omega+1}^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(3,2,0)=\psi(\Omega_{\omega+1}^2+\Omega_{\omega+1})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(3,2,0)(4,2,0)=\psi(\Omega_{\omega+1}^2\cdot2)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(4,0,0)=\psi(\Omega_{\omega+1}^2\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(4,1,0)=\psi(\Omega_{\omega+1}^2\cdot\Omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(4,2,0)=\psi(\Omega_{\omega+1}^3)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,0,0)=\psi(\Omega_{\omega+1}^\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,1,0)=\psi(\Omega_{\omega+1}^{\Omega})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,1,0)(1,1,1)=\psi(\Omega_{\omega+1}^{\Omega_\omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,1,0)(6,2,0)=\psi(\Omega_{\omega+1}^{\psi_\omega(\Omega_{\omega+1})})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,1,0)(6,2,0)(7,2,0)=\psi(\Omega_{\omega+1}^{\psi_\omega(\Omega_{\omega+1}^2)})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,2,0)=\psi(\Omega_{\omega+1}^{\Omega_{\omega+1}})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,2,0)(5,2,0)(6,2,0)=\psi(\Omega_{\omega+1}^{\Omega_{\omega+1}^{\Omega_{\omega+1}}})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,3,0)=\psi(\Omega_{\omega+2})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,3,0)(5,3,0)=\psi(\Omega_{\omega+2}^2)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,3,0)(5,3,0)(6,3,0)=\psi(\Omega_{\omega+2}^{\Omega_{\omega+2}})

\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,0)(4,3,0)(5,4,0)=\psi(\Omega_{\omega+3})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)=\psi(\Omega_{\omega\cdot2})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(1,1,1)=\psi(\Omega_{\omega\cdot2}+\Omega_\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(1,1,1)(2,1,0)(3,2,1)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(2,0,0)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+1))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(2,1,0)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(2,1,0)(3,2,1)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2})))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,0,0)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+1)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,1,0)=\psi(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+\psi_\omega(\Omega_{\omega\cdot2}+\Omega)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,0)=\psi(\Omega_{\omega\cdot2}+\Omega_{\omega+1})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,0)(4,3,0)=\psi(\Omega_{\omega\cdot2}+\psi_{\omega+1}(\Omega_{\omega+2}))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,0)(4,3,1)=\psi(\Omega_{\omega\cdot2}+\psi_{\omega+1}(\Omega_{\omega\cdot2}))

\\



     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,0)(4,3,1)(4,2,0)=\psi(\Omega_{\omega2}+\psi_{\omega+1}(\Omega_{\omega2}+\Omega_{\omega+1}))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,0)(4,3,1)(4,3,0)=\psi(\Omega_{\omega2}+\Omega_{\omega+2})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(3,2,1)=\psi(\Omega_{\omega2}\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,0,0)=\psi(\Omega_{\omega2}\cdot\omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,1,0)=\psi(\Omega_{\omega2}\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,1,0)(1,1,1)=\psi(\Omega_{\omega2}\cdot\Omega_\omega)
\\



     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,1,0)(4,0,0)=\psi(\Omega_{\omega2}\Omega_\omega\omega)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,1,0)(4,1,0)=\psi(\Omega_{\omega2}\Omega_\omega\Omega)


\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,1,0)(5,2,0)=\psi(\Omega_{\omega2}\psi_\omega(\Omega_{\omega+1}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(2,0,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+1))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(2,1,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+\Omega))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,0,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+1)))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,1,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1}+\Omega)))
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega+1})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(3,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega+1}2)
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega+1}^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega+2}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega2}))


\\
                                        %(2,1,0)(3,2,1)
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega2}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega2}\Omega_{\omega+1}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,2,0)(5,3,1)(6,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega2}\Omega_{\omega+1}+\psi_{\omega+1}(\Omega_{\omega2}\Omega_{\omega+1})))

\\

     %(0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0) Comparsion
    %                                    (0,0,0)(1,1,1)(2,1,0)(1,1,0)
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,3,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega+2})

\\

     %(0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0) Comparsion
    %                                    (0,0,0)(1,1,1)(2,1,0)(1,1,0)
    %                                           (3,2,1)(4,2,0)(3,2,0)
    %                                            1 1 0  1 0 0  1 1 0
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,3,0)(5,4,1)(6,2,0)(5,4,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega+3})

\\

     %(0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0) Comparsion
    %                                    (0,0,0)(1,1,1)(2,1,0)(1,1,1)
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,3,1)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega2})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,3,1)(4,3,1)=\psi(\Omega_{\omega2}\Omega_{\omega+1}+\Omega_{\omega2}\cdot2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(4,3,1)(5,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}\cdot2)


\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(5,0,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}\cdot\omega)


\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(5,1,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}\cdot\Omega)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(5,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,0,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}^{\omega})
\\


     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,1,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}^{\Omega})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,2,0)=\psi(\Omega_{\omega2}\Omega_{\omega+1}^{\Omega_{\omega+1}})

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,3,0)=\psi(\Omega_{\omega2}\psi_{\omega+1}(\Omega_{\omega+2}))

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,3,1)=\psi(\Omega_{\omega2}\psi_{\omega+1}(\Omega_{\omega2}))

\\

    %                                    (0,0,0)(1,1,1)(2,0,0)(3,1,1)
    %                                     3 2 0  3 2 0  3 2 0  3 2 0
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,2,0)(6,3,1)(7,2,0)=\psi(\Omega_{\omega2}\psi_{\omega+1}(\Omega_{\omega2}\Omega_{\omega+1}))

\\

    %                                    (0,0,0)(1,1,1)(2,1,0)
    %                                     3 2 0  3 2 0  3 2 0
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,3,0)=\psi(\Omega_{\omega2}\Omega_{\omega+2})

\\

    %                                    (2,1,0)(3,2,1)(4,2,0)
    %                                     1 1 0  1 1 0  1 1 0
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,0)(4,3,1)(5,3,0)(4,3,0)(5,4,1)(6,4,0)=\psi(\Omega_{\omega2}\Omega_{\omega+3})



\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(3,2,1)=\psi(\Omega_{\omega2}^2)

\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(4,2,0)(3,2,1)=\psi(\Omega_{\omega2}^3)
\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,0,0)=\psi(\Omega_{\omega2}^{\omega})
\\

     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,1,0)=\psi(\Omega_{\omega2}^{\Omega})
\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,2,0)=\psi(\Omega_{\omega2}^{\Omega_{\omega+1}})

\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,2,0)(3,2,1)=\psi(\Omega_{\omega2}^{\Omega_{\omega2}})

\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,3,0)=\psi(\Omega_{\omega2+1})

\\
     (0,0,0)(1,1,1)(2,1,0)(3,2,1)(4,2,0)(5,3,1)=\psi(\Omega_{\omega3})

\\

     (0,0,0)(1,1,1)(2,1,1)=\psi(\Omega_{\omega^2})

\\

     (0,0,0)(1,1,1)(2,1,1)(1,1,1)(2,1,1)=\psi(\Omega_{\omega^2}2)
\\


     (0,0,0)(1,1,1)(2,1,1)(2,0,0)=\psi(\Omega_{\omega^2}\omega)

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,0)=\psi(\Omega_{\omega^2}\Omega)

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(1,1,1)=\psi(\Omega_{\omega^2}\Omega_\omega)
\\


     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(1,1,1)(2,1,1)=\psi(\Omega_{\omega^2}^2)

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,0,0)=\psi(\Omega_{\omega^2}^{\omega})
\\


     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,1,0)=\psi(\Omega_{\omega^2}^{\Omega})

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\omega^2+1})
\\


     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)=\psi(\Omega_{\omega^2+\omega})


\\
     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(3,2,1)=\psi(\Omega_{\omega^2+\omega}2)
\\



     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,1,0)=\psi(\Omega_{\omega^2+\omega}\Omega)
\\



     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,1,0)(1,1,1)=\psi(\Omega_{\omega^2+\omega}\Omega_{\omega})
\\


     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,2,0)=\psi(\Omega_{\omega^2+\omega+1})
\\


     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,2,0)(5,3,1)=\psi(\Omega_{\omega^2+\omega2})


\\
     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,2,1)=\psi(\Omega_{\omega^2\cdot2})

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,0)(3,2,1)(4,2,1)(4,2,0)(5,3,1)(6,3,1)=\psi(\Omega_{\omega^2\cdot3})

\\

     (0,0,0)(1,1,1)(2,1,1)(2,1,1)=\psi(\Omega_{\omega^3})


\\
     (0,0,0)(1,1,1)(2,1,1)(3,0,0)=\psi(\Omega_{\omega^{\omega}})


\\
     (0,0,0)(1,1,1)(2,1,1)(3,0,0)(2,1,1)=\psi(\Omega_{\omega^{\omega+1}})

\\

     (0,0,0)(1,1,1)(2,1,1)(3,0,0)(3,0,0)=\psi(\Omega_{\omega^{\omega\cdot2}})
\\


     (0,0,0)(1,1,1)(2,1,1)(3,0,0)(4,1,1)=\psi(\Omega_{\psi(\Omega_\omega)})
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)=\psi(\Omega_{\Omega})=\text{Bird's Ordinal}

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)=\psi(\Omega_{\Omega}+\Omega)


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\omega))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,0,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\omega\omega))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\omega\Omega))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\omega\Omega_2))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,0)(4,3,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\omega+1}))


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,0)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\omega2}))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\omega^2}))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\omega^3}))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,0,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\omega^\omega}))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega}))

\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2)=\psi(\Omega_{\Omega}+\Omega_2)
\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_\omega))


\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_\omega\omega))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_\omega\Omega_2))

\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(2,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_\omega^2))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega+1})))
\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2})))


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}2)))


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}\Omega)))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}\Omega_2)))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,2)(6,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}\psi_\omega(\Omega_{\omega2}))))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}\Omega_{\omega+1})))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega2}^2)))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3)(6,4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega3})))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega^2})))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)(5,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega^3})))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)(6)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\omega^\omega})))


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega})))
\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\Omega_{\omega+1})))


\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)(5,4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\psi_{\omega+1}(\Omega_{\omega2}))))

\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)(5,4,1)(6,4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\psi_{\omega+1}(\Omega_{\omega^2}))))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)(5,4,1)(6,4,1)(7,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\psi_{\omega+1}(\Omega_{\Omega}))))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)(5,4,1)(6,4,1)(7,1)(5,4)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\Omega_{\omega+2})))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3)(5,4,1)(6,4,1)(7,1)(5,4)(6,5,1)(7,1)(8,1)(6,5)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\Omega_{\omega+3})))

\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\Omega_{\omega2})))


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2)(4,3,1)(5,3,1)\\(6,1)(4,3,1)(5,3)(6,4,1)(7,4,1)(8,1)(6,4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\psi_\omega(\Omega_{\Omega}+\Omega_{\omega3})))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\omega^2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\omega^3}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\omega^\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,0)(5,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\omega^{\omega^\omega}}))


\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,0)(5,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\psi(\Omega)}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,0)(5,1,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}+\Omega_{\psi(\Omega_\omega)}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}2))
    =\psi(\Omega_{\Omega}2)



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(2,2,1)(3,2,1)(4,1)(2,2,1)(3,2,1)(4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}3))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\omega))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)(2,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega)+\Omega_\omega)



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)(3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega\omega))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)(3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega^2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)(4,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\psi_1(\Omega_2)))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,1)(4,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\psi_1(\Omega_\omega)))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega_{2}))

\\




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(2,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega_{\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(2,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}\Omega_{\omega^2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(2,2,1)(3,2,1)(4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(2,2,1)(3,2,1)(4,1)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^2+\Omega_\Omega\Omega_{2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(3,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^2\omega))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^2\Omega))
\\



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^2\Omega_2))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(3,2)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^3\Omega_2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^{\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^{\Omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega}^{\Omega_2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+1}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}\omega))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}\Omega_2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,2)(6,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}\psi_\Omega(\Omega_{\Omega+\omega})))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}\Omega_{\Omega+1}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}^2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(5,3)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}^3))

\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(6,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}^{\omega}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(6,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_\Omega+\Omega_{\Omega+\omega}^{\Omega_2}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(6,4)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega+\omega+1}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3)(6,4,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega+\omega2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega+\omega^2}))





     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2)(4,3,1)(5,3,1)(6,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega2}))


\\

     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)\\(4,1,0)(3,2)(4,3,1)(5,3,1)(6,1)(5,3)(6,4,1)(7,4,1)(8,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega3}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega}))


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega}\Omega_2))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)(4,3)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega+1}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)(4,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega+\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)(4,3,1)(5,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega+\omega^2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)(4,3,1)(5,3,1)(6,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega+\Omega}))


\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2)(4,3,1)(5,3,1)(6,1)(5,3,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega2}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega^2}))


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(4)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\omega^\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)\\(3,2,1)(4)(5,1)(6,1)(7,1)(7,1)(7,1)(7,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega\varphi(1,0,0,0,0,0)}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^2}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(3,2,1)(4,1,0)(3,2,1)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^3}))




     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(4,0,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^\omega}))



\\
     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(4,1,0)(3,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^\Omega\omega}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^{\Omega2}}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(4,1,0)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^{\Omega^2}}))


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(4,1,0)(4,1,0)\\
     (4,1,0)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)(4,1,0)(4,1,0)(4,1,0)(3,2,1)\\
     (4,1,0)(4,1,0)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)(4,1,0)(4,1,0)(3,2,1)\\
     (4,1,0)(4,1,0)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)(4,1,0)(4,1,0)\\
     (3,2,1)(4,1,0)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)(4,1,0)\\
     (3,2,1)(4,1,0)(4,1,0)(4,1,0)(3,2,1)(4,1,0)(4,1,0)(4,1,0)\\
     (3,2,1)(4,1,0)(4,1,0)(4,1,0)\\
     (3,2,1)(4,1,0)(4,1,0)\\
     (3,2,1)(4,1,0)(3,2,1)(4,1,0)(3,2,1)(4,1,0)(3,2,1)(4,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^{\Omega^5+\Omega^4+\Omega^3\cdot4+\Omega^2\cdot5+\Omega+4}}))


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(5,0,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^{\Omega^\omega}}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(5,1,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega^{\Omega^\Omega}}))
\\


     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(5,2,0)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\psi_1(\Omega_2)}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,1,0)(5,2,1)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\psi_1(\Omega_\omega)}))



     (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)=\psi(\Omega_{\Omega}+\psi_1(\Omega_{\Omega_2}))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)=\psi(\Omega_{\Omega_2}+\psi_2(\Omega_{\Omega_2}))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(4,3,1)=\psi(\Omega_{\Omega_2\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(4,3,1)(5,2)=\psi(\Omega_{\Omega_2^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(5,0)=\psi(\Omega_{\Omega_2^\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(5,2)=\psi(\Omega_{\Omega_2^{\Omega_2}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(6)=\psi(\Omega_{\Omega_2^{\Omega_2^\omega}})
\\


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,2)(6,3)=\psi(\Omega_{\psi_2(\Omega_3)})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1)(2,2,1)(3,2,1)(4,2)(2,2)(3,3,1)(4,3,1)(5,3)=\psi(\Omega_{\Omega_3})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)=\psi(\Omega_{\Omega_\omega})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(1,1,1)=\psi(\Omega_{\Omega_\omega}+\Omega_\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)=\psi(\Omega_{\Omega_\omega}+\Omega_\omega\Omega)





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,0)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega+1}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega2}))
\\



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega^2}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(1,1,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+1))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\Omega))

\\


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2,1)(3,2)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega+1})))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2,1)(3,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega2})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2,1)(3,2,1)(4,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega^2})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(2,1)(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega})))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+1)))


\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\Omega)))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,1)(4,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega_2}))))


\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,1)(4,2,1)(5,2,1)=\psi(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\Omega_\omega}+\psi_\omega(\Omega_{\omega^2}))))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,2)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,2)(3,2)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega+1}2)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,2)(4,3,1)(5,3,1)=\psi(\Omega_{\Omega_\omega}+\psi_{\omega+1}(\Omega_{\omega^2}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,2)\\(4,3,1)(5,3,1)(6,1)=\psi(\Omega_{\Omega_\omega}+\psi_{\omega+1}(\Omega_{\Omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)(3,2,1)(4,2,1)(5,1)(3,2)\\(4,3,1)(5,3,1)(6,1)(4,3)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega+2})


\\
    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega2})

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega2})


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)=\psi(\Omega_{\Omega_\omega}+\Omega_{\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega}+\Omega_{\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)(1,1,1)=\psi(\Omega_{\Omega_\omega}2)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)(3,2,1)=\psi(\Omega_{\Omega_\omega}2+\Omega_{\omega2})


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega}2+\Omega_{\Omega})


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,0,0)=\psi(\Omega_{\Omega_\omega}\omega)
\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)=\psi(\Omega_{\Omega_\omega}\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)(5,2)=\psi(\Omega_{\Omega_\omega}\psi_{\omega}(\Omega_{\omega+1}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)(5,2,1)=\psi(\Omega_{\Omega_\omega}\psi_{\omega}(\Omega_{\omega2}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)(5,2,1)(6,2,1)=\psi(\Omega_{\Omega_\omega}\psi_{\omega}(\Omega_{\omega^2}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)(5,2,1)(6,2,1)(7,1)=\psi(\Omega_{\Omega_\omega}\psi_{\omega}(\Omega_{\Omega}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,1,0)(5,2,1)(6,2,1)(7,1)=\psi(\Omega_{\Omega_\omega}\psi_{\omega}(\Omega_{\Omega}))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)=\psi(\Omega_{\Omega_\omega}\Omega_{\omega+1})


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(3,2,1)=\psi(\Omega_{\Omega_\omega}\Omega_{\omega2})
\\


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(3,2,1)(4,2,1)=\psi(\Omega_{\Omega_\omega}\Omega_{\omega^2})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega}\Omega_{\Omega})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(3,2,1)(4,2,1)(5,1)(1,1,1)=\psi(\Omega_{\Omega_\omega}^2)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(3,2,1)(4,2,1)(5,1)(4,2,0)=\psi(\Omega_{\Omega_\omega}^2+\Omega_{\Omega_\omega}\Omega_{\omega+1})
\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(4)=\psi(\Omega_{\Omega_\omega}^2\omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(4,2,0)(4)=\psi(\Omega_{\Omega_\omega}^3\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5)=\psi(\Omega_{\Omega_\omega}^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,1)=\psi(\Omega_{\Omega_\omega}^\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3)=\psi(\Omega_{\Omega_\omega+1})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3)(6,4)=\psi(\Omega_{\Omega_\omega+2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)=\psi(\Omega_{\Omega_\omega+\omega})


\\
    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)=\psi(\Omega_{\Omega_\omega+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)=\psi(\Omega_{\Omega_\omega+\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(1,1,1)=\psi(\Omega_{\Omega_\omega2})


\\
    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(2,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(2,1)(3,2,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\omega2})))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(2,1)(3,2,1)(4,2,1)(5,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2,0)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega}\Omega_{\omega+1})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+1)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\Omega)))
\\


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,1)(4,2,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\omega2}))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,1)(4,2,1)(5,2,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\omega^2}))))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,1)(4,2,1)(5,2,1)(6,1)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega}))))

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,1)(4,2,1)(5,2,1)(6,1)(5,2,0)=\psi(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega2}+\psi_\omega(\Omega_{\Omega_\omega}\Omega_{\omega+1}))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2)=\psi(\Omega_{\Omega_\omega2}+\Omega_{\omega+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)=\psi(\Omega_{\Omega_\omega2}+\Omega_{\omega2})

\\


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)=\psi(\Omega_{\Omega_\omega2}+\Omega_{\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)(5,1)(1,1,1)=\psi(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega})

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)(5,1)(4,2,0)=\psi(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega}\Omega_{\omega+1})

后面会使用\psi_{\text{容许序数}}(x)的形式，防止混淆。

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\omega}))


\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\omega^2}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\Omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+1))

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4,2)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\Omega_{\omega+1}))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4,2)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\omega})))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4,2)(5,3,1)(6,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\omega^2})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4,2)(5,3,1)(6,3,1)(7,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\Omega})))

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(4,2)(5,3,1)(6,3,1)(7,1)(4,2)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2})+\Omega_{\omega+1}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,2)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\Omega_{\omega+1})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,2)(6,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega2}+\psi_{\Omega_{\Omega_\omega+1}}(\Omega_{\Omega_\omega+\omega}))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,3)=\psi_\Omega(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega+1})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega+\omega})


\\
    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,3,1)(6,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,3,1)(6,3,1)(7,1)=\psi_\Omega(\Omega_{\Omega_\omega2}+\Omega_{\Omega_\omega+\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(5,3,1)(6,3,1)(7,1)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}2+\Omega_{\Omega_\omega+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,0,0)=\psi_\Omega(\Omega_{\Omega_\omega2}\omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,1,0)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega)





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,2)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega+1})

\\

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(5,3,1)(6,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(5,3,1)(6,3,1)(7,1)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(5,3,1)(6,3,1)(7,1)(6,3)=\psi_\Omega(\Omega_{\Omega_\omega2}^2+\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+1})


\\
    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(6,0)=\psi_\Omega(\Omega_{\Omega_\omega2}^2\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(6,1)=\psi_\Omega(\Omega_{\Omega_\omega2}^2\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(6,2)=\psi_\Omega(\Omega_{\Omega_\omega2}^2\Omega_{\omega+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(6,3)=\psi_\Omega(\Omega_{\Omega_\omega2}^2\Omega_{\Omega_{\omega}+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(6,3)(6)=\psi_\Omega(\Omega_{\Omega_\omega2}^3\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,0)=\psi_\Omega(\Omega_{\Omega_\omega2}^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,1)=\psi_\Omega(\Omega_{\Omega_\omega2}^\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,1)(1,1,1)=\psi_\Omega(\Omega_{\Omega_\omega2}^{\Omega_\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,2)=\psi_\Omega(\Omega_{\Omega_\omega2}^{\Omega_{\omega+1}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,3)=\psi_\Omega(\Omega_{\Omega_\omega2}^{\Omega_{\Omega_{\omega}+1}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,4)=\psi_\Omega(\Omega_{\Omega_\omega2+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,4,1)=\psi_\Omega(\Omega_{\Omega_\omega2+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)=\psi_\Omega(\Omega_{\Omega_\omega2+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)=\psi_\Omega(\Omega_{\Omega_\omega2+\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(1,1,1)=\psi_\Omega(\Omega_{\Omega_\omega3})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(7,4,1)(8,4,1)(9,1)(1,1,1)=\psi_\Omega(\Omega_{\Omega_\omega3}2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8)=\psi_\Omega(\Omega_{\Omega_\omega3}\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,2)=\psi_\Omega(\Omega_{\Omega_\omega3}\Omega_{\omega+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,3)=\psi_\Omega(\Omega_{\Omega_\omega3}\Omega_{\Omega_{\omega}+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,4)=\psi_\Omega(\Omega_{\Omega_\omega3}\Omega_{\Omega_{\omega}2+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,4)(9,5)=\psi_\Omega(\Omega_{\Omega_\omega3+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,4)(9,5,1)=\psi_\Omega(\Omega_{\Omega_\omega3+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)\\(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)(8,4)(9,5,1)(10,5,1)=\psi_\Omega(\Omega_{\Omega_\omega3+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(\Omega_{\Omega_\omega\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,1)(4,2,1)=\psi_\Omega(\Omega_{\Omega_\omega\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,1)(5,1)=\psi_\Omega(\Omega_{\Omega_\omega\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,1)(5,1)(1,1,1)=\psi_\Omega(\Omega_{\Omega_\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(\Omega_{\Omega_\omega^2\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(5)=\psi_\Omega(\Omega_{\Omega_\omega^{\omega}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(5,1)=\psi_\Omega(\Omega_{\Omega_\omega^{\Omega}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(6,2)=\psi_\Omega(\Omega_{\psi_{\Omega_\omega}(\Omega_{\omega+1})})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,2)=\psi_\Omega(\Omega_{\Omega_{\omega+1}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,2)(3,2,1)=\psi_\Omega(\Omega_{\Omega_{\omega2}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,1)=\psi_\Omega(\Omega_{\Omega_{\omega^2}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,1)(3,1)=\psi_\Omega(\Omega_{\Omega_{\Omega}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,1)(3,1)(1,1,1)=\psi_\Omega(\Omega_{\Omega_{\Omega_\omega}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,1)(3,1)(1,1,1)(2,1,1)(3,1)=\psi_\Omega(\Omega_{\Omega_{\Omega_\Omega}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)=\psi_\Omega(I)=\text{Extend Buchholz's Ordinal}



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)=\psi_\Omega(I+\psi_I(I))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)(2,0,0)=\psi_\Omega(I+\psi_I(I)\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)(3,0,0)=\psi_\Omega(I+\psi_I(I)\omega^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,0,0)(3,1,1)=\psi_\Omega(I+\psi_I(I)\psi_\Omega(\Omega_\omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)=\psi_\Omega(I+\psi_I(I)\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(1,1,1)(2,1,1)(3,1,0)(2)=\psi_\Omega(I+\psi_I(I)^2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(1,1,1)(2,1,1)(3,1,0)(2,1)=\psi_\Omega(I+\psi_I(I)^2+\psi_I(I)\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(2)=\psi_\Omega(I+\psi_I(I)^2\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(2,1)=\psi_\Omega(I+\psi_I(I)^2\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(2,1)(2,1)=\psi_\Omega(I+\psi_I(I)^3\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3)=\psi_\Omega(I+\psi_I(I)^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)=\psi_\Omega(I+\psi_I(I)^\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(2,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)}\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(2,1)(3)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(2,1)(3,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)+\Omega})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(2,1)(3,1)(2,1)(3,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)2+\Omega})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(3)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)\omega})


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(3,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(3,1)(3,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)^2\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,1)(4,1)=\psi_\Omega(I+\psi_I(I)^{\psi_I(I)^\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2)=\psi_\Omega(I+\psi_I(I+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)=\psi_\Omega(I+\psi_I(I+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\omega^2))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I+\psi_I(I+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I)\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1)(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+1)))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\omega)))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,1)\\(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I)))2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\Omega))=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I)))\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)(2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\psi_I(I)\Omega))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)(2,1)(2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\psi_I(I)^2\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)(3)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\psi_I(I)^\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+ \psi_{\psi_I(I+1)}(\psi_I(I+1))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+ \psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I)))))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+ \psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+1)))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+ \psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\Omega)))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,1)(4,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+ \psi_{\psi_I(I+1)}(\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+1)}(\psi_I(I+1)))))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+1)2)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+2)}(\psi_I(I+2)))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+2)}(\psi_I(I+\omega)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3,1)(5,3,1)(6,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+2)}(\psi_I(I+\Omega)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3,1)(5,3,1)(6,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_{\psi_I(I+2)}(\psi_I(I+\psi_I(I))))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3,1)(5,3,1)(6,1)(4,3)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+2))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2)(4,3,1)(5,3,1)(6,1)(4,3)(5,4,1)(6,4,1)(7,1)(5,4)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+3))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))+\psi_I(I+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))2)






    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))2+\psi_I(I+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))2+\psi_I(I+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))2+\psi_I(I+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(3,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)+\psi_I(I+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(3,2,1)(4,2,1)(5,1)(4,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)+\psi_I(I+\psi_I(I))\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(3,2,1)(4,2,1)(5,1)(4,1)(1,1,1)(2,1,1)(3,1,0)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(4,0)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(4,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(4,1)(4,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)^2\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(5)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I)^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,1)(5,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_{\psi_I(I+1)}(\psi_I(I+1)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(1,1,1)(2,1,0)\\(3,2,1)(4,2,1)(5,1)(4,2,0)(5,3,1)(6,3,1)(7,1)(6,3)(5,3,1)=\psi_\Omega(\Omega_{\Omega_\omega2}\Omega_{\Omega_\omega+\omega})

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I+\omega))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(3,2,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I+\omega^2))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))\psi_I(I+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(3,2,1)(4,2,1)(5,1)(4,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^2\psi_I(I+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(4)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^\omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(4,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(4,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^{\psi_I(I+1)})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(4,2)(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^{\psi_I(I+\omega)})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(4,2)(4)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^{\psi_I(I+\psi_I(I))\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^{\psi_I(I+\psi_I(I))^{\omega}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I))^{\psi_I(I+\psi_I(I))^{\psi_I(I+1)}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3)=\psi_\Omega(I+\psi_I(I+\psi_I(I)+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3,1)(6,3,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3,1)(6,3,1)(7,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I)2))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3,1)(6,3,1)(7,1)(6,3)=\psi_\Omega(I+\psi_I(I+\psi_I(I)2)\psi_I(I+1))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2)(5,3,1)(6,3,1)(7,1)(6,3)(7,4,1)(8,4,1)(9,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)2+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)\omega))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)\omega^2))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^2))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^2\omega))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(4,2,1)(5,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^3\omega))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^\omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5,1)(4,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^{\psi_I(I)}\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5,1)(4,2,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^{\psi_I(I)}\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5,1)(4,2,1)(5,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^{\psi_I(I)+\Omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(5,1)(5,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I)^{\psi_I(I)\Omega}))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,1)\\(6,2)=\psi_\Omega(I+\psi_I(I+\psi_{\psi_I(I+1)}(\psi_I(I+1))))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I+1)))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(3,2,1)=\psi_\Omega(I+\psi_I(I+\psi_I(I+\omega)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(3,2,1)(4,2,1)(5,2)=\psi_\Omega(I+\psi_I(I+\psi_I(I+\psi_I(I+1))))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4)=\psi_\Omega(I2)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4)(3,2,1)=\psi_\Omega(I2+\psi_I(I+\omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4)(3,2,1)(4,2,1)(5,2)=\psi_\Omega(I2+\psi_I(I+\psi_I(I+1)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4)(3,2,1)(4,2,1)(5,2)(4)=\psi_\Omega(I2+\psi_I(I2))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4)(4)=\psi_\Omega(I2+\psi_I(I2)\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,1)=\psi_\Omega(I2+\psi_I(I2)\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,1)(5,2)=\psi_\Omega(I2+\psi_I(I2)\psi_{\psi_I(I+1)}(\psi_I(I+1)))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,1)(5,2,1)=\psi_\Omega(I2+\psi_I(I2)\psi_{\psi_I(I+1)}(\psi_I(I+\omega)))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)=\psi_\Omega(I2+\psi_I(I2)\psi_I(I+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(3,2,1)=\psi_\Omega(I2+\psi_I(I2)\psi_I(I+\omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(3,2,1)(4,2,1)(5,2)(4,2)=\psi_\Omega(I2+\psi_I(I2)^2\psi_I(I+1))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(4,0)=\psi_\Omega(I2+\psi_I(I2)^\omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(4,2)=\psi_\Omega(I2+\psi_I(I2)^{\psi_I(I+1)})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(5,3)=\psi_\Omega(I2+\psi_I(I2+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(5,3,1)(6,3,1)(7,1)=\psi_\Omega(I2+\psi_I(I2+\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(5,3,1)(6,3,1)(7,2)=\psi_\Omega(I2+\psi_I(I2+\psi_I(I+1)))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(5,3,1)(6,3,1)(7,3)=\psi_\Omega(I2+\psi_I(I2+\psi_I(I2+1)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1)(3,2,1)(4,2,1)(5,2)(4,2)(5,3,1)(6,3,1)(7,3)(6)=\psi_\Omega(I3)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)=\psi_\Omega(I\omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(1,1,1)=\psi_\Omega(I\omega+\Omega_\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(1,1,1)(2,1,1)(3,1,0)(2)=\psi_\Omega(I\omega+\psi_I(I))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(1,1,1)(2,1,1)(3,1,0)(2,1,1)=\psi_\Omega(I\omega+\psi_I(I\omega))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2)=\psi_\Omega(I\omega+\psi_I(I\omega)\omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)=\psi_\Omega(I\omega+\psi_I(I\omega)\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(1,1,1)(2,1,1)(3,1,0)(2,1,1)=\psi_\Omega(I\omega+\psi_I(I\omega)^2)





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(2)=\psi_\Omega(I\omega+\psi_I(I\omega)^\omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(2,1)=\psi_\Omega(I\omega+\psi_I(I\omega)^\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2)=\psi_\Omega(I\omega+\psi_I(I\omega+1))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1,1)(2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_I(I\omega)\omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1,1)(2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_I(I\omega)\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2,1,1)(2,1)(3,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_{\psi_I(I\omega+1)}(\psi_I(I\omega+1)))






    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(3,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_I(I\omega+1))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(3,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_I(I\omega+\omega))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(3,2,1)(4,2,1)(5,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))+\psi_I(I\omega+\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)\\(5,1)(3,2,1)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1,0)(2,1,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,1)(1,1,1)(2,1,1)(3,1)(2,1,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\psi_I(I\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,1)(3,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\psi_I(I\omega)+\psi_I(I\omega+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,1)(3,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\psi_I(I\omega)+\psi_I(I\omega+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,1)(4)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\psi_I(I\omega)\omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega))\psi_I(I\omega+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2)(5,3,1)(6,3,1)(7,1)\\(1,1,1)(2,1,1)(3,1)(2,1,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)2))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)\omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2,1)(5,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)^2\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(5)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)^\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(5,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega)^\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,1)(6,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_{\psi_I(I\omega+1)}(\psi_I(I\omega+1))))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega+1)))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(3,2,1)=\psi_\Omega(I\omega+\psi_I(I\omega+\psi_I(I\omega+\omega)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4)=\psi_\Omega(I\omega+I)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4,2)(5,3,1)(6,3,1)(7,3)=\psi_\Omega(I\omega+I+\psi_I(I\omega+I+\psi_I(I\omega+I+1)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4,2)(5,3,1)(6,3,1)(7,3)(6)=\psi_\Omega(I\omega+I2)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4,2)(5,3,1)(6,3,1)(7,3)(6,3)(7,4,1)(8,4,1)(9)=\psi_\Omega(I\omega+I3)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4,2,1)=\psi_\Omega(I\omega2)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1)(3,2,1)(4,2,1)(5,2)\\(4,2,1)(4,2)(5,3,1)(6,3,1)(7,3)=\psi_\Omega(I\omega3)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1,1)=\psi_\Omega(I\omega^2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(2,1,1)(2,1,1)=\psi_\Omega(I\omega^3)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3)=\psi_\Omega(I\omega^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)=\psi_\Omega(I\Omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1) (1,1)(2,2,1)(3,2,1)(4,2)(3,2,1)(4,2)=\psi_\Omega(I\Omega_2)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1) (1,1)(2,2,1)(3,2,1)(4,2)(3,2,1)(4,1)(3,2,1)=\psi_\Omega(I\Omega\omega)


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1) (1,1)(2,2,1)(3,2,1)(4,2)(3,2,1)(4,1)(3,2,1)(4)=\psi_\Omega(I\Omega\omega^{\omega})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1) (1,1,1)(2,1,1)(3,1)=\psi_\Omega(I\Omega_{\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)\\(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I\psi_I(I))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2)=\psi_\Omega(I\psi_I(I)+\psi_I(I+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,2)=\psi_\Omega(I\psi_I(I)+\psi_I(I+\psi_I(I+1)))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4)=\psi_\Omega(I\psi_I(I)+\psi_I(I2))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)\\(1,1,1)(2,1,1)(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)=\psi_\Omega(I\psi_I(I)+\psi_I(I\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)=\psi_\Omega(I\psi_I(I)+\psi_I(I\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(1,1,1)(2,1,1)(3,1)(2)=\psi_\Omega(I\psi_I(I)+\psi_I(I\psi_I(I)))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(2,1)=\psi_\Omega(I\psi_I(I)+\psi_I(I\psi_I(I))\Omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2)=\psi_\Omega(I\psi_I(I)+\psi_I(I\psi_I(I))^2\psi_I(I\psi_I(I)+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2)(5,3)=\psi_\Omega(I\psi_I(I)+\psi_I(I\psi_I(I)+1))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2)(5,3,1)=\psi_\Omega(I\psi_I(I)+\psi_I(I\psi_I(I)+\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2)(5,3,1)\\(6,3,1)(7,3)(6)=\psi_\Omega(I\psi_I(I)+I)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2)(5,3,1)\\(6,3,1)(7,3)(6,3,1)=\psi_\Omega(I\psi_I(I)+I\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2,1)=\psi_\Omega(I\psi_I(I)\omega)

    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(4,2,1)(5,1)=\psi_\Omega(I\psi_I(I)\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,1)(6,2)=\psi_\Omega(I\psi_I(I+1))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,2)=\psi_\Omega(I\psi_I(I+\psi_I(I+1)))





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)\\(3,1)(2,1)(3,2,1)(4,2,1)(5,2)(4,2,1)(5,2)(3,2,1)(4,2,1)(5,2)(4)=\psi_\Omega(I\psi_I(I2))






    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)(3,1,0)(2,1,1)=\psi_\Omega(I\psi_I(I\omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1,0)=\psi_\Omega(I\psi_I(I\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(2)=\psi_\Omega(I^2)





    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(2,1,1)(3,1)(2,1,1)=\psi_\Omega(I^2\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(3)=\psi_\Omega(I^\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(3,1)=\psi_\Omega(I^{\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)=\psi_\Omega(\Omega_{I+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(2,1,1)(3,1)=\psi_\Omega(\Omega_{I+1} + \psi_{\Omega_{I+1}}(\Omega_{I+1}+\Omega))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(2,1,1)(3,1)(4,2)=\psi_\Omega(\Omega_{I+1} + \psi_{\Omega_{I+1}}(\Omega_{I+1}+\psi_{\Omega_{I+1}}(\Omega_{I+1})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(3)=\psi_\Omega(\Omega_{I+1} + \psi_{\Omega_{I+1}}(\Omega_{I+1}+\psi_{\Omega_{I+1}}(\Omega_{I+1}+1)))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(3,1)=\psi_\Omega(\Omega_{I+1} + \psi_{\Omega_{I+1}}(\Omega_{I+1}+\psi_{\Omega_{I+1}}(\Omega_{I+1}+\Omega)))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(4,2)=\psi_\Omega(\Omega_{I+1}2)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2)(5,3)=\psi_\Omega(\Omega_{I+2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)=\psi_\Omega(\Omega_{I+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)=\psi_\Omega(\Omega_{I+\omega^2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)=\psi_\Omega(\Omega_{I+\Omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(1,1,1)(2,1,1)(3,1)(4,2)=\psi_\Omega(\Omega_{I+\psi_I(\Omega_{I+1})})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(2)=\psi_\Omega(\Omega_{I2})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(2,1,1)=\psi_\Omega(\Omega_{I2} + \psi_{\Omega_{I+1}}(\Omega_{I2}+1))


    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(2,1,1)(3,1)=\psi_\Omega(\Omega_{I2} + \psi_{\Omega_{I+1}}(\Omega_{I2}+\Omega))




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(2,1,1)(3,1)(4,2)=\psi_\Omega(\Omega_{I2} + \psi_{\Omega_{I+1}}(\Omega_{I2}+\psi_{\Omega_{I+1}}(\Omega_{I2})))



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(4,2)=\psi_\Omega(\Omega_{I2} + \Omega_{I+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(4,2,1)=\psi_\Omega(\Omega_{I2} + \Omega_{I+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5)=\psi_\Omega(\Omega_{I2}\omega)



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,1)=\psi_\Omega(\Omega_{I2}\Omega)




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,2)=\psi_\Omega(\Omega_{I2}\Omega_{I+1})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,2)(6,3)=\psi_\Omega(\Omega_{I2+1})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,2)(6,3,1)=\psi_\Omega(\Omega_{I2+\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,2,1)=\psi_\Omega(\Omega_{I\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(5,2,1)(6,1)(5,2,1)=\psi_\Omega(\Omega_{I^2\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(6)=\psi_\Omega(\Omega_{I^\omega})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,1)(7,2)=\psi_\Omega(\Omega_{\psi_{\Omega_{I+1}}(\Omega_{I+1})})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,2)=\psi_\Omega(\Omega_{\Omega_{I+1}})




    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,2)(4,2,1)=\psi_\Omega(\Omega_{\Omega_{I+\omega}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,2)(4,2,1)(5,2,1)(6,1)=\psi_\Omega(\Omega_{\Omega_{\Omega_{I+1}}})



    (0,0,0)(1,1,1)(2,1,1)(3,1,0)(4,2,1)(5,2,1)(6,2)(5)=\psi_\Omega(I_2)


\end{array}
$$

# 2019 Qualification

-   Score : 66
-   Rank : 2361

---

感冒了，最后一题想不动了= =

## A

- 4变成3，另一个数对应位置变1

## B

- 原串是E，答案就填S；原串是S，答案就填E

## C

- 考虑相邻两个数的GCD即可

## D

-   直接做5次的版本
-   考虑答案不超过15个，我们把1024个位置分成64组，一组16个，交替01查询
-   这样每组都不可能全部被删除，因此我们知道了每组各有几个坏位置
-   接下来对每组并行进行即可，利用二进制覆盖原理完成查询，需要$\log_2 16 = 4$次查询
-   加上原来分组查询，一共五次
-   不足1024位的利用代码进行掩盖即可，详见代码
# WIEN2k

**WIEN2k 官网链接**：http://susi.theochem.tuwien.ac.at/


[用 WIEN2k 计算拓扑不变量：Chern 数与 Z₂ 不变量全解析](https://mp.weixin.qq.com/s/C5OCQbbVayRPiTuTkr9V0w)

这套“在 WIEN2k 里直接算拓扑不变量”的方法，核心来自 Gomez-Bastidas & Rubel 的实现：它把 Z₂（用 HWCC/Wilson loop） 和 Chern 数（用 Berry 相位 + Wilson loops 网格化） 两条路线，做成了 两个脚本模块，并且不需要构造最大局域化 Wannier 函数（MLWF），而是直接用 相邻 k 点波函数的重叠矩阵来推进 Wilson loop。
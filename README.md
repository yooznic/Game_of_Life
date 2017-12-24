[![Build Status](https://travis-ci.org/ZacheryYoung/Game_of_Life.svg?branch=master)](https://travis-ci.org/ZacheryYoung/Game_of_Life)

请用TDD的方式，实现一个生命游戏(game of lfe)。

生命游戏中，对于任意细胞，规则如下：
每个细胞有两种状态-存活或死亡，每个细胞与以自身为中心的周围八格细胞产生互动。（如图，黑色为存活，白色为死亡）
1.   当前细胞为存活状态时，当周围低于2个（不包含2个）存活细胞时，该细胞变成死亡状态。（模拟生命数量稀少）
2.   当前细胞为存活状态时，当周围有2个或3个存活细胞时，该细胞保持原样。
3.   当前细胞为存活状态时，当周围有3个以上的存活细胞时，该细胞变成死亡状态。（模拟生命数量过多）
4.   当前细胞为死亡状态时，当周围有3个存活细胞时，该细胞变成存活状态。（模拟繁殖）
可以把最初的细胞结构定义为种子，当所有在种子中的细胞同时被以上规则处理后, 可以得到第一代细胞图。按规则继续处理当前的细胞图，可以得到下一代的细胞图，周而复始。

可以参考https://zh.wikipedia.org/wiki/%E5%BA%B7%E5%A8%81%E7%94%9F%E5%91%BD%E6%B8%B8%E6%88%8F

要求：
1.  必要有单元测试，单元测试框架使用JUnit
2.  不要求有图形界面
3.  最初的细胞结构可以从文件、命令行等方式输入
4.  所有代码提交要基于GitHub
5.  注意，先从最简单的开始，提供可部分工作的功能，多次迭代修改

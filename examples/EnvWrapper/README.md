**MiniWorld 复现注意事项**

EnvWrapper过程中加入了以下改变：

1.加入了cv的颜色识别功能，用于前期验证

2.reward加入了每步-0.5的惩罚，并将完成奖励设置为100倍，以在不加入先验知识的情况下快速收敛，同时绘制合理的训练曲线（原gym环境没有惩罚，并且最终奖励为接近1的浮点数）
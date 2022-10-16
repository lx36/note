Tensor  

Tensor（张量）是一种特殊的数据结构，与数组和矩阵非常相似。在PyTorch中，用来对Tensor模型的输入和输出以及模型的参数进行编码。

1. 初始化Tensor

   Tensor可以通过多种方式进行初始化。

   1. 直接从数据中创建并且数据类型自动推断
   2. 从Numpy数组创建
   3. 从另一个张量创建，新张量保留参数张量的属性，除非明确覆盖
   4. 使用随机值或常量值创建

2. Tensor的属性

   张量的属性描述了它们的形状、数据类型和储存它们的设备（CPU或者GPU）

3. Tensor的运算

   运算包括算术、线性代数、矩阵操作（转置、索引、切片）、采样等。

   这些操作中的每一个都可以在 GPU 上运行。默认情况下，张量是在 CPU 上创建的，可以使用`.to`方法明确地将张量移动到 GPU。

数据集和数据加载器









Transformerlayer

PyTorch在1.2版本的发布中推出了标准的Transformer模块，该模型基于一篇名为《Attention is All You Need》的论文。Tranformer模型完全依赖注意力机制，能够在输入和输出之间获得全局依赖全局依赖。相比RNN，Transformer模型已经被证明在许多序列到序列任务的性能上更胜一筹，同时更可并行化。在PyTorch中，Transformer模块细分为五个子模块，可以轻松调用或者组合，包括nn.Transfomer、nn.TransformerEncode、nn.TransformerDecoder、nn.TransformerEncoderLayer和nn.TransformerDecoderLayer。



torchtext

PyTorch提供了特定领域的库，torchtext就是其中之一，torchtext软件包由数据处理通用程序和流行的自然语言数据集组成。




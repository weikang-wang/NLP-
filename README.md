# NLP-小记

## 几个关键字 ——> 一条包含这些关键字的文本

> 直接用seq2seq

> 解码可以做优化，比如设置解码内容没有全部包含所有关键词就不结束

> 如果关键词多，从左到右的autoregressive是不适合的。但是non auto regressive是很适合的。只是需要确定mask数目，或者说遍历mask数目。(mask数量什么意思)

> 是可以用像lasertagger之类的方法，作为一个扩写任务

> 像T5的预训练任务也算是扩写

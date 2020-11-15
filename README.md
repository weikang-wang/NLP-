# NLP-小记

## 几个关键字 ——> 一条包含这些关键字的文本

> 直接用seq2seq

> 解码可以做优化，比如设置解码内容没有全部包含所有关键词就不结束

> 如果关键词多，从左到右的autoregressive是不适合的。但是non auto regressive是很适合的。只是需要确定mask数目，或者说遍历mask数目。(mask数量什么意思)

> 是可以用像lasertagger之类的方法，作为一个扩写任务

> 像T5的预训练任务也算是扩写

## Do Not Have Enough Data? Deep Learning to the Rescue

> 利用GPT系列这些因果语言模型来生成训练数据来做数据增强，具体方法  y1 SEP X1 EOS y2 SEP X2 EOS ......  yn SEP xn EOS。训练方法就是预训练的步骤从左到右。这步微调
> 然后通过 y SEP 来生成句子。


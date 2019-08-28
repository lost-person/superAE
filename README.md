## Citation
If you use this code for your research, please cite the paper this code is based on:
*Autoencoder as Assistant Supervisor: Improving Text Representation for Chinese Social Media Text Summarization*:

```
@inproceedings{Ma2016superAE,
  title   = {Autoencoder as Assistant Supervisor: Improving Text Representation for Chinese Social Media Text Summarization},
  author  = {Shuming Ma and Xu Sun and Junyang Lin and Houfeng Wang},
  booktitle = {{ACL} 2018},
  year      = {2018}
}
```

注：
此项目是在 linux 上运行的。虽然我修改了一些bug，但是 win10 上还是有点问题。

preprocess.py 数据预处理程序，以供 train.py使用 输入参数：-train\_src（训练文章数据地址）, -train\_tgt（训练摘要数据地址）, -valid\_src（验证文章数据地址）, valid\_tgt（验证摘要数据地址）, -save\_data（存储数据地址）

lcsts.yaml 配置文件

修改文件：

train.py 修改Bug 注意运行时 yaml 文件的地址

loss.py 190行 修改了，运行时报错，维度不匹配，先用常数代替，之后学习 pytorch 修改

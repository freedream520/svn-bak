# SVN 注意事项

**1.** 采用 “ Lock-Modify-Unlock ”这种模式进行协同工作，需要多进行的两个步骤：

```
Get Lock（锁定文件）  
Commit（提交,提交成功后程序自动把锁释放掉）   
```

**2.** 合理选择提交频度和时机：

两次提交之间尽量进行同一类操作，比如，统改图层后提交一次，统改标注线 型后再提交一次。

> 目的：一旦业主要求有反复，我们也很容易把以前工作成果 从库中提出来，减少返工。 		
建议一小时左右提交一次。养成按时提交的习惯。
   
**3.** check out 和export的区别 

```
check out 方式获得文件后，文件仍处于SVN版本控制中
export 导出当前版本的数据，文件脱离SVN版本控制
```
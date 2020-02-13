## 日志记录

#### Ver 0.5.0-   2020-02-12
    1.完成了对于图注和表注的识别与提取工作的一大半，尚且还需要对识别部分之下做聚类分析找到完整的图注和表注区间
   
#### Ver 0.4.0    2020-02-12
    1.优化完成了页码处理模块，在测试文献中尚未发现bug

#### Ver 0.4.0-   2020-02-12  (尚有个别错误待规则设定与优化，可运行版，持续优化中)
    1.调试完成了对页面最下方的页码和注释区域的类别判定流程（未完全完成）

#### Ver 0.3.5-   2020-02-11  (编码测试中，非可运行版）
    1.增加了对页面最上方和最下方的页码，注释等区域的类别判定流程(调试中)
    2.增加了对页面类型的判定方法(文献正文的排版类型为左右二分还是占据整个页面)

#### Ver 0.3.0-   2020-02-10  (非稳定版，持续优化中)
    1.重构代码，将相似功能的方法单独放置于一个py文件下
    2.解决了作者及其相关信息抽取的一个bug，该bug会导致异常退出
    3.解决了上述模块的一个bug,该bug会导致基于pdfminer提取出的个别不标准的识别结果无法找到合适的区域结束位置
    4.优化了上述模块的处理速度

#### Ver 0.2.2    2020-02-09    
    1.增加了对Author相关信息的处理流，暂测试中：https://github.com/Noba1anc3/pdf_analysis_beta

#### Ver 0.2.1    2020-02-09    
    1.增加了对Title的处理流，暂测试中：https://github.com/Noba1anc3/pdf_analysis_beta

#### Ver 0.1.1    2020-02-07    
    1.增加了log信息的显示
    2.优化了在一个文件夹下逐个文件分析处理的流程，将自适应性的文件搜寻替代原有的基于指定名称的文件搜索
    3.增加了非PDF文件的跳过流程及其log信息记录
    4.调整了版面分析和转换图像方法内的部分细节，使修改后的方法能适应上面做出的改变
    5.增加了对目录下文件处理进度的显示
    6.优化了对分析结果的保存过程
    
#### Ver 0.1.0    2020-02-07    
    1.将基于坐标和种类绘制方框封装为方法
    2.将使用pdfminer版面分析和调用方法将PDF文件转化为转图像封装为方法
    3.将计算版面与图像的长宽比以及在图像上进行版面分析封装为方法
    4.在新方法的基础之上重构原有代码，降低模块之间的耦合程度
    5.增加了对LTRect和LTCurve的处理流


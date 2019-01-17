# 项目简介
read frequceny of word in PDF文件可以读取英文pdf指定页数中的单词，
且可筛选出指定长度的单词，且可按照单词在这些页数中所出现的频率从高到低显示。

# 需要安装的python库


    >>> pip install PyPDF2
    >>> pip install re
    >>> pip install string    


PyPDF2：可以用来提取pdf文件中的信息（在这个项目中）  
re：正则表达式操作 
string：可以对字符串进行操作

# 使用
把文件路径替换成你的书的路径

    >>> pdfFileObj=open('F:\\ziqianbeifen\\zhuomian\\英文电子书\\批判性思维\\Asking the Right Questions.pdf','rb')
    
将range(读取的起始页，读取的结束页)里的页码改成你想读取的页码

    >>>for pageNum in range(16,18):
    >>>    pageObj=pdfReader.getPage(pageNum)

指定统计单词的长度范围

    >>>match_pattern=re.findall(r'\b[a-z]{6,15}\b',text_string)
    
# 运行结果示例

    >>>7 approach
    >>>6 panning
    >>>4 knowledge
    >>>4 evaluate
    >>>3 sponge



    





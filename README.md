SAPI_WorkHelper
===============

The help work tool

本工具暂时提供3个功能：

1.调换功能。以行为单位根据某个字符调换内容，如按等号（=）调换如下内容：
    调换前：  txtName.Text = eml.Name ;
    调换后：  eml.Name = txtName.Text ;
    该功能可用于新增修改页，减少给控件赋值和更新实体类时的重复人工劳动。

    操作步骤：
    a. 在上面的textarea内输入你需要调换的语句，可多行。每行分别进行调换。
    b. 点击页面上的“使用调换方法默认设置”，会自动加载调换用的正则等信息。
       可自行修改以扩展功能。
    c. 点击“调换”按钮。将在下面的textarea处输出调换后内容。
    
 
 2. 获取控件ID功能。 可输入一大堆字符串，如前端aspx代码，使用该功能后可获
    取字符串中所有ID以txt、txa、hid、ddl、rdl、cbk开头控件的ID。
	
	操作步骤：
	a. 在上面的textarea内输入你要查找的内容，如一个aspx文件的全部代码。
	b. 点击“使用获取控件方法默认设置”。
	c. 点击“获取全部控件”。将在下面的textarea处输出逗号分隔的全部控件id。


3. 验证正则是否匹配功能。 能验证你书写的正则是否与传入内容匹配,该功能将
   对输入内容进行逐行验证。最后输出匹配失败的行索引。

	操作步骤：
	a. 在上面的textarea中输入你需要验证的内容，可按行分隔多段需要验证的内容。
	b. 在“按…………正则匹配”处的文本框（即第一个单行文本框）内输入你要验证的有
	   效正则表达式，如/\d*/。
	c. 点击“严重那个正则是否能匹配所有传入值”按钮。下面的textarea中将输出验
	   证结果。如：
	   		匹配失败,失败值的索引为：1,2,3,4,5
	   	或
			匹配成功
			

欢迎大家一起扩展该工具。 或提出你们的改进意见。

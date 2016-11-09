1.	designer
	1)dialog/window/widget三种类别
	![](https://raw.githubusercontent.com/HappyMmor/note/master/note_images/three_kind_window.png)
	2)各种UI控件:
	![](https://raw.githubusercontent.com/HappyMmor/note/master/note_images/widgets.png)
	3)就是Ctrl+鼠标左键选择控件并用Form的各种布局了,要结合spacers来用
	4)信号\槽的绑定,Tab顺序编辑
2.	代码部分
	1)UI动态加载,初始化,这块是固定代码,东西不多
	2)信号和槽的绑定:
			*一个信号可以和多个槽绑定,发射这个信号时会以不定顺序执行
			*一个槽可以绑定多个信号,不论发射哪个信号,都会调用这个槽
			*一个信号可以与另外一个信号连接,发射连接信号时,也会发射被连接信号
	要把信号连接到槽,它们的参数必须有相同的顺序和类型(槽的参数数量可以比信号少,但顺序和类型必须一致)
	连接也可以被移除
	定义了自己的信号和槽的类必须在开始加上Q_OBJECT宏

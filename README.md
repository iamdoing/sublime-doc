This is a document for how to use sublime-text 3

## 1.为什么用sublime?
	1.1 简单好用
	1.2 多点编辑
	1.3 强大的包管理
	1.4 深度可定制
	1.5 快速切换文件 Cmd+p
	1.5 好用的命令执行面板 Shift+Cmd+p
	1.6 标准

## 2.安装
	https://www.sublimetext.com/

## 3.常用快捷键
	3.1 在命令面板(Shift+Cmd+p)中模糊输入来查看快捷键 
	3.2 操作/编辑/选择
		Cmd+n 开一个新页面
		Cmd+d 选中当前单词，继续敲可以选中多个
		Cmd+/ 注释掉/取消注释
		Ctrl+ ]/[ 缩进
		Ctrl+l 选择当前行
		Shift+Cmd+d 复制当前行
		Ctrl+z 撤销
		多点选择,按住 Cmd 键,点击鼠标左键
		列选择，按住 Alt 键，用鼠标左键拖动
	3.3 光标移到
		方向键,一次移动一个字符
		Alt+方向键,一次移动一个单词
		Cmd+方向键,一次移动一行

## 4.文件打开与跳转
	4.1 Cmd+p 模糊输入文件名打开文件
	4.2 Cmd+- 跳转到打开文件前所在的文件
	4.3 Shift+Cmd+- 文件跳转过了回跳
	4.3 Ctrl+Tab 打开的多个文件之间跳转

## 5.文件的搜索
	5.1 Cmd+f 搜索当前文件 Enter查找下一个 Shift+Enter查找上一个
	5.2 Alt+Cmd+f 搜索替换
	5.3 Shift+Cmd+f 文件夹中查找替换

## 4.自定义目录
	4.1 用户自定义的内容都放在一个固定的目录,操作系统不同,目录的路径也不同
	4.2 以本人的Mac为例,自定义文件存放在/Users/air/Library/Application Support/Sublime Text 3/Packages/User目录中,以下简称User目录
	4.3 自定义的内容一般分为Default和User
		Default是编辑器自带的的默认配置,一般情况下不允许更改，
		User是用户自定义的文件,优先级高于Default,用户可以更具爱好配置

## 5.自定义快捷键
	5.1 查找精确的命令名
		5.1.1 Ctrl + `(反引号)打开控制台
  		5.1.2 在控制台中输入 sublime.log_commands(True)
  		5.1.3 再次执行操作,在控制台中就可以看到精确的命令名  
	5.2 打开Key Bindings中的User配置(对应User目录下的Default (OSX).sublime-keymap 文件)
	5.3 复制一条配置,更改键和对应的命令名,如果是首次打开,可以从Default配置中拷贝一条配置然后修改

## 6.自定义配置
	6.1 打开Settings中的User配置(对应User目录下的Preferences.sublime-settings 文件)
	6.2 添加或者修改相关的配置,比如,Sublime默认是不显示行号的,如果想显示行号,可以添加
	"highlight_line": true,

## 7.包管理

	7.1 在Mac系统中,Sublime自带默认的包安装在/Applications/Sublime Text.app/Contents/MacOS/Packages中
	7.2 可以通过安装PackageControl来安装和管理包,安装方法参考https://packagecontrol.io/
	7.3 安装完成后,可以在命令面板(Shift+Cmd+p)中输入Install Package来打开包安装面板
	7.4 在包安装面板中直接输入需要安装的包名就可以安装对应的包了
	7.5 安装完成后
		7.5.1 会在User目录下生成一个PackageControl.sublime-settings文件,这个文件纪录了所有安装的包
		7.5.2 会在安装包的数据区域(/Users/air/Library/Application Support/Sublime Text 3/Installed Packages)生成一个这个包的文件
	7.6 如果想删除某个包,在命令面板中输入Remove Package打开卸载面板直接输入需要删除的包名就可以了

## 8.常用包介绍
	8.1 emmt html/css代码补全
		参考 https://docs.emmet.io/cheat-sheet/
	8.2 SyncedSideBar 在侧边栏中同步展开当前打开的文件 
	8.3 AutoFileName 自动补全文件名
	8.4 Color Highlighter css颜色显示

## 9.自定义代码段 Snippets
	9.1 Tools->Developer->New Snippet 新建一个Snippet
	9.2 修改snippet 内容(content)/触发词(tabTrigger)/作用范围(scope) 
	9.3 查看作用范围的快捷键是 Alt+Cmd+p
	9.4 保存文件到User目录, 以 .sublime-snippet结尾 

## 10.管理自己的配置
	10.1 将User目录下的文件推送到github上
	10.2 如果新安装Sublime,可以从github上把文件clone下来放到User目录下
	10.3 安装PackageControl,这样所有的包会自动安装上
	

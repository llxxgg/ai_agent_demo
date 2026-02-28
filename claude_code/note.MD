# agent驱动的自动化开发

| 掌握command、hook、skills


## 从安装到入门
> https://mp.weixin.qq.com/s/hBpZa_5_HRTB3swMOjsK7Q

Claude Code不能代码补全，但是在代码生成、调试、文档生成等方面表现出色。如果需要代码补全功能，建议搭配使用其他工具，如Github Copilot、Cursor等。

## 实战
> https://mp.weixin.qq.com/s/EwMoxI4nWfgTHO574K7qsQ

### 三种权限模式

默认模式

* "Yes"：仅批准当前这一次的文件编辑操作。下次 Claude Code 要编辑文件时，会再次询问。

* "Yes, allow all edits during this session(shift+tab)"：批准当前编辑，并且在整个会话期间自动接受所有后续的文件编辑，不再询问。<span style="color:red;font-weight:bold;">如果选择这个选项，就会进入编辑模式。</span>

* "No"：不允许编辑文件。那么 Claude Code 就会什么也不做。

编辑模式

计划模式 规划任务完成后，Claude Code 会给出 4 个选择：

* "Yes, clear context and auto-accept edits (shift+tab)"：它会清除没有必要的上下文，并自动接受所有后续的文件编辑，不再询问。如果选择这个选项，就会进入编辑模式。

* "Yes,auto-accept edits"：和上面选项一样，但不会清除上下文。

* "Yes, manually approve edits"：和上面选项一样，但每次都要手动批准文件编辑。

* 最后，一个是输入框，如果你对它给出的建议不满意，可以在这里和它继续对话，让它重新规划任务。

### 历史会话 /resume

如果你不小心关闭了终端，你在对应的目录下，重新启动 Claude Code。你会发现，之前的会话不见了。不用担心，Claude Code 会自动保存会话。你只需要在启动 Claude Code 时，加上 -c 参数即可。

或者，你在新启动 Claude Code 里，输入 /resume 就会列出当前目录下所有会话记录，如果太多，还可以在搜索框中进行搜索。


### 压缩上下文 /compact

大模型的上下文是有限的，Claude Code 状态栏会显示当前会话使用的上下文占用情况。当上下文占用过多时，默认是在约 95% 容量时触发压缩上下文的功能。

你也可以手动触发压缩上下文的功能。输入 /compact，后面写上你想保留的上下文内容，Claude Code 保留你指定的上下文内容。

### 截图




# Reference
https://mp.weixin.qq.com/s/hBpZa_5_HRTB3swMOjsK7Q

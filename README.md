<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline7">1. spacemacs 学习笔记</a>
<ul>
<li><a href="#orgheadline3">1.1. Dired Mode</a>
<ul>
<li><a href="#orgheadline1">1.1.1. 退出命令</a></li>
<li><a href="#orgheadline2">1.1.2. 进入文件修改模式</a></li>
</ul>
</li>
<li><a href="#orgheadline6">1.2. Org Mode</a>
<ul>
<li><a href="#orgheadline4">1.2.1. 各种字体</a></li>
<li><a href="#orgheadline5">1.2.2. org mode 文档转换输出</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>

# spacemacs 学习笔记<a id="orgheadline7"></a>

## Dired Mode<a id="orgheadline3"></a>

### 退出命令<a id="orgheadline1"></a>

    C-x k       ;;kill buffer
    C-x b       ;;换到上一个buffer
    C-x C-b     ;;查看所有buffer，选择进入

### 进入文件修改模式<a id="orgheadline2"></a>

-   直接用 C-x C-q 切换到可编辑状态，然后修改文件名.
-   用 C-c C-c 提交就可以快速修改文件名.
-   C-c ESC 是取消改名，C-x C-q 来提示是否改名.
-   或者 %R 来用正则表达式批量改名.

## Org Mode<a id="orgheadline6"></a>

### 各种字体<a id="orgheadline4"></a>

1 **粗体** , *斜体* <del>删除线</del> <span class="underline">下划线</span>  下标:H<sub>2</sub> O , 上标 E = mc<sup>2</sup>   

    *粗体* , /斜体/ +删除线+ _下划线_  下标:H_2 O , 上标 E = mc^2

2 等宽字: `git` , `git`   

    =git= 或 ~git~

3 反双斜杠为换行

    \\ 反双斜杠为换行

### org mode 文档转换输出<a id="orgheadline5"></a>

1.  C-c, C-e 后出现相关菜单.按需求执行,可生成相关格式文档 **html**, **markdown** .
2.  如未见看MarkDown选项,M-x, 然后输入:org-md-export-to-markdown.

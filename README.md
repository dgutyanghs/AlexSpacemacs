<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#org8c840fd">1. spacemacs 学习笔记</a>
<ul>
<li><a href="#orge5021f3">1.1. Dired Mode</a>
<ul>
<li><a href="#org8c84da3">1.1.1. 退出命令</a></li>
<li><a href="#org6e5e753">1.1.2. 进入文件修改模式</a></li>
</ul>
</li>
<li><a href="#orgd059821">1.2. Org Mode</a>
<ul>
<li><a href="#org854c385">1.2.1. 各种字体</a></li>
<li><a href="#orgea5696d">1.2.2. org mode 文档转换输出</a></li>
</ul>
</li>
<li><a href="#orgcc13746">1.3. 修改.spacemacs的目录位置</a></li>
<li><a href="#org2b76456">1.4. AG search</a></li>
<li><a href="#org09f38d9">1.5. default 字体setting</a></li>
</ul>
</li>
</ul>
</div>
</div>

<a id="org8c840fd"></a>

# spacemacs 学习笔记


<a id="orge5021f3"></a>

## Dired Mode


<a id="org8c84da3"></a>

### 退出命令

    C-x k       ;;kill buffer
    C-x b       ;;换到上一个buffer
    C-x C-b     ;;查看所有buffer，选择进入


<a id="org6e5e753"></a>

### 进入文件修改模式

-   直接用 C-x C-q 切换到可编辑状态，然后修改文件名.
-   用 C-c C-c 提交就可以快速修改文件名.
-   C-c ESC 是取消改名，C-x C-q 来提示是否改名.
-   或者 %R 来用正则表达式批量改名.


<a id="orgd059821"></a>

## Org Mode


<a id="org854c385"></a>

### 各种字体

1 **粗体** , *斜体* <del>删除线</del> <span class="underline">下划线</span>  下标:H<sub>2</sub> O , 上标 E = mc<sup>2</sup>   

    *粗体* , /斜体/ +删除线+ _下划线_  下标:H_2 O , 上标 E = mc^2 

2 等宽字: `git` , `git`   

    =git= 或 ~git~

3 反双斜杠为换行

    \\ 反双斜杠为换行


<a id="orgea5696d"></a>

### org mode 文档转换输出

1.  C-c, C-e 后出现相关菜单.按需求执行,可生成相关格式文档 **html**, **markdown** .
2.  如未见看MarkDown选项,M-x, 然后输入:org-md-export-to-markdown.


<a id="orgcc13746"></a>

## 修改.spacemacs的目录位置

因为多台电脑用到.spacemacs, 为共享它，我将它用github管理。

    $ln -s src/spacemacs_alex  ~/.spacemacs

src为存放configure文件夹，我将配置文件命名为：spacemacs<sub>alex</sub>.


<a id="org2b76456"></a>

## AG search

"C-c k"打开AG ,输入 keyword 全工程搜索.


<a id="org09f38d9"></a>

## default 字体setting

    ;; UTF8!
      (set-language-environment 'utf-8)
      (set-terminal-coding-system 'utf-8)
      (setq locale-coding-system 'utf-8)
      (set-default-coding-systems 'utf-8)
      (set-selection-coding-system 'utf-8)
      (prefer-coding-system 'utf-8)


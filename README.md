## Introduction

Use the markdown-preview.vim plugin you can preview markdown on real-time
through a browser

> this plugin need your vim support py2/py3 features  
> test on window/ubuntu14


### screenshot

![screenshot](./screenshot.gif)

### Usage

**Command:**

```
    MarkdownPreview
    " open preview window in markdown buffer

    MarkdownPreviewStop
    " close the preview window and server

```
> when MarkdownPreview command can't open preview window, you can use the
MarkdownPreviewStop command before using MarkdownPreview command

**Defaul Setting:**

```
    g:mkdp_path_to_chrome = "google-chrome"
    " path to the chrome or the command to open chrome

    g:mkdp_auto_start = 0
    " set to 1, the vim will open the preview window once enter the markdown
    buffer

    g:mkdp_auto_open = 0
    " set to 1, the vim will auto open preview window when you edit the
    markdown file

    g:mkdp_auto_close = 1
    " set to 1, the vim will auto close current preview window when change
    from markdown buffer to another buffer

    g:mkdp_refresh_slow = 0
    " set to 1, the vim will just refresh markdown when save the buffer or
    leave from insert mode, default 0 is auto refresh markdown as you edit or
    move the cursor
```

--------------------------------------------------------------------------------

### 说明

使用 markdown-preview.vim 插件可以实时通过浏览器预览 markdown 文件

> 使用该插件需要 vim 支持py2/py3

### 使用和设置

**命令：**

```
    MarkdownPreview
    " 在打开 markdown 文件后，使用该命令可以打开预览窗口

    MarkdownPreviewStop
    " 关闭 markdown 预览窗口，并停止开启的服务进程

```
> 在 MarkdownPreview 命令无效的情况下，可以先 MarkdownPreviewStop 再 MarkdownPreview

**默认配置：**

```
    g:mkdp_path_to_chrome = "google-chrome"
    " 设置 chrome 浏览器的路径（或是启动 chrome 的命令）

    g:mkdp_auto_start = 0
    " 设置为 1 可以在打开 markdown 文件的时候自动打开浏览器预览，只在打开
    markdown 文件的时候打开一次

    g:mkdp_auto_open = 0
    " 设置为 1 在编辑 markdown 的时候检查预览窗口是否已经打开，否则自动打开预
    览窗口

    g:mkdp_auto_close = 1
    " 在切换 buffer 的时候自动关闭预览窗口，设置为 0 则在切换 buffer 的时候不
    自动关闭预览窗口

    g:mkdp_refresh_slow = 0
    " 设置为 1 则只有在保存文件，或退出插入模式的时候更新预览，默认为 0，实时
    更新预览
```

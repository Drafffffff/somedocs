---
sidebarDepth: 2
---

# VsCode 中的 p5.js 环境搭建

<font size=5><a href="https://code.visualstudio.com/">点击这里下载VsCode</a></font>

## 安装插件

vscode 之所以流行的一个非常大的原因就是他完善的插件生态系统，通过安装插件可以把 vscode 打造成一个非常强大的编辑器

点击 vscode 左边最后一个按钮，进入应用市场。

![](http://pic.drafff.art//drafff/20200323140405.png)

### 1. Chinese (Simplified) Language Pack for Visual Studio Code

中文插件。

![](http://pic.drafff.art//drafff/20200323140613.png)

### 2. Live Server

能够实时运行 p5.js 代码。

![](http://pic.drafff.art//drafff/20200323141438.png)

### 3. p5js Snippets

p5.js 代码片段，装了之后能自动补全代码。

![](http://pic.drafff.art//drafff/20200323141959.png)

### 4. Prettier - Code formatter （可选）

更规范的代码自动格式化。

![](http://pic.drafff.art//drafff/20200323142154.png)

### 5. Visual Studio IntelliCode（可选）

黑科技，AI 预测你下面想写的代码，并给出提示。

![](http://pic.drafff.art//drafff/20200323144318.png)

### 6. theme （可选）

好看的界面是码代码的第一生产力，搜索 theme 就能在商店中找到数千款主题。

推荐主题

- Material theme
- One dark Pro

![](http://pic.drafff.art//drafff/20200323142327.png)

### 7. Bracket Pair Colorizer （可选）

括号颜色匹配，非常好用。

![](http://pic.drafff.art//drafff/20200323150618.png)

## 一个示例

下面通过一个实例演示实际编写代码的操作。

1.  新建文件夹，命名为`p5test`

2.  将`p5test`拖入空的 vscode 中，或者右键>通过 Code 打开

    ![](http://pic.drafff.art//drafff/20200323145534.png)

3.  在 Vscode 中新建两个文件,`index.html`和`script.js`

    ![](http://pic.drafff.art//drafff/20200323145725.png)

4.  在`index.html`中输入以下代码,引入`p5js`库和我们将要编写的脚本，并且去除网页的默认样式带来间距。

        `index.html:`

    ```html
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.0.0/p5.min.js"></script>
        <script src="./script.js"></script>
        <style>
          body {
            margin: 0;
            padding: 0;
            overflow: hidden;
          }
        </style>
      </head>
      <body></body>
    </html>
    ```
    输入并保存。

5.  此时准备工作已经完成，我们可以在`script.js`中开始写`p5.js`的代码了,下面给出一个简单的例子

    `script.js`

    ```javascript
    function setup() {
      createCanvas(windowWidth, windowHeight);
    }
    function draw() {
      ellipse(mouseX, mouseY, 40, 40);
    }
    ```

    输入并保存。

6. 运行代码，右键`index.html`，选择Open With Live Server

    ![](http://pic.drafff.art//drafff/20200323152604.png)

    此时会弹出浏览器
    ![](http://pic.drafff.art//drafff/20200323152232.png)


## 把代码上传到Codepen
1. 登陆[codepen](https://codepen.io),新建一个`pen`

    ![](http://pic.drafff.art//drafff/20200318224514.png)

2. 导入p5.js库

    ![](http://pic.drafff.art//drafff/20200318224701.png)

    ![](http://pic.drafff.art//drafff/20200318224746.png)

3. 把代码粘贴在`js`框中

    ![](http://pic.drafff.art//drafff/20200318224958.png)

4. 点击左下角`Embed`

    ![](http://pic.drafff.art//drafff/20200318225025.png)

5. 复制html代码，粘贴到HTML区块。

    ![](http://pic.drafff.art//drafff/20200318225127.png)
    ![](http://pic.drafff.art//drafff/20200323162326.png)

6. 完成



## 链接

1. [阿里云域名注册文档](https://help.aliyun.com/product/35473.html?spm=a2c4g.750001.list.90.4cc17b13wo6dYw)

2. [p5.jsCheatSheet](https://drafff.art/p5js-cheatsheet-forartists/)

2. [p5.js官网 & 文档](https://p5js.org/)

3. [ml5](https://ml5js.org/),[ml5.js Example](https://ml5js.github.io/ml5-examples/public/)

3. [The Coding Train - Youtube (p5js官方教学 *需魔法上网)](https://www.youtube.com/channel/UCvjgXvBlbQiydffZU7m1_aw)

4. [现代JavaScript教程](https://zh.javascript.info/)

5. [EloquentJavascript](https://eloquentjavascript.net/)

6. [OpenProcessing（*需要魔法上网）](https://www.openprocessing.org/),[neort](https://neort.io/)

7. [Getting Started with p5.js.pdf](https://www.lanzous.com/iakek0j)

8. [The Nature of Code 代码本色](https://natureofcode.com/book/),[pdf下载](https://www.lanzous.com/iakexli)

10. [Generative Design](http://www.generative-gestaltung.de/2/)

9. [Programming Design System](https://www.runemadsen.com/syllabi/programming-design-systems/),[我翻译的版本](https://drafff.art/tags/%E7%BC%96%E7%A8%8B%E8%AE%BE%E8%AE%A1%E7%B3%BB%E7%BB%9F/)

10. [codesthesia](https://codesthesia.net/p5graphics/)
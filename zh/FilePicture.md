第一个标题 | 第二个标题
--- | ---
内容单元 | 内容单元
内容单元 | 内容单元

第一个标题 | 第二个标题
--- | ---
内容单元 | 内容单元
内容单元 | 内容单元

![堡垒](https://vignette.wikia.nocookie.net/masseffect/images/d/d7/MassEffect2Citadel.jpg/revision/latest?cb=20100721191415)

左对齐 | 居中对齐 | 右对齐
:-- | :-: | --:
第3列是 | 一些罗y的文字 | **$ 1600**
第2列是 | 居中 | $ 12
斑马条纹 | 整齐 | ~~ $ 1 ~~

Dillinger是基于云的，可移动的，离线存储的，由AngularJS支持的HTML5 Markdown编辑器。

- 在左侧输入一些Markdown
- 见右侧的HTML
- 魔法

# 真正

- 导入HTML文件并观看它神奇地转换为Markdown
- 拖放图像（需要链接您的Dropbox帐户）

你也可以：

- 从GitHub，Dropbox，Google Drive和One Drive导入和保存文件
- 将markdown和HTML文件拖放到Dillinger中
- 将文档导出为Markdown，HTML和PDF

Markdown是一种轻量级的标记语言，它基于人们在电子邮件中自然使用的格式约定。 [John Gruber]在[Markdown网站] [df1]上写道

> Markdown格式语法的首要设计目标是使其尽可能可读。这个想法是，Markdown格式的文档应该以纯文本形式原样发布，而不会看起来像被标签或格式说明所标记。

您在此处看到的文本*实际上是*用Markdown编写的！要了解Markdown的语法，请在左侧窗口中输入一些文本，然后在右侧查看结果。

### 假

Dillinger使用许多开源项目来正常工作：

- [AngularJS]-HTML增强了Web应用程序！
- [Ace Editor]-出色的基于Web的文本编辑器
- [markdown-it]-Markdown解析器正确完成。快速且易于扩展。
- [Twitter引导程序]-适用于现代Web应用程序的出色UI样板
- [node.js]-后端的事件I / O
- [Express]-快速的node.js网络应用框架[@tjholowaychuk]
- [Gulp]-流式构建系统
- [Breakdance](https://breakdance.github.io/breakdance/) -HTML降价转换器
- [jQuery]-duh

当然，Dillinger本身是开源的，在GitHub上有一个[公共存储库] [dill]。

### 安装

![伊洛斯](https://lh3.googleusercontent.com/proxy/DDV8a7sLIWurhJtW8Ego9bq-JlwpfFFoR0tkLJQKKYXEXoWHB6ZUP5jGKD2VcYt3z1QVsgcn6L3GoU1ns8m9fvi3U51GzddA70ZUMHgzHvjl4-i7YOJY9cShBPrfjUhMQhxaJ97WFBp612XmjMXVGypfGkiBarN4PWxhiHkiYYNW7HGbtTpOcyt9GQ4Q23C2noxLTWFXZMcQZhRpQA_qzu2n6_H6CPViBnhSHpEl4JZAPaGCSJqgZg)

Dillinger需要运行[Node.js](https://nodejs.org/) v4 +。

安装依赖项和devDependencies并启动服务器。

```sh
$ cd dillinger
$ npm install -d
$ node app
```

用于生产环境...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### 外挂程式

Dillinger当前使用以下插件进行了扩展。下面是有关如何在您自己的应用程序中使用它们的说明。

插入 | 自述文件
--- | ---
投寄箱 | [plugins / dropbox / README.md] [PlDb]
的GitHub | [plugins / github / README.md] [PlGh]
Google云端硬碟 | [plugins / googledrive / README.md] [PlGd]
一个驱动器 | [插件/onedrive/README.md][PlOd]
中 | [plugins / medium / README.md] [PlMe]
谷歌分析 | [plugins / googleanalytics / README.md] [PlGa]

### 发展历程

想要贡献？大！

Dillinger使用Gulp + Webpack进行快速开发。更改文件，立即查看您的更新！

打开您喜欢的终端并运行这些命令。

第一个标签：

```sh
$ node app
```

第二个标签：

```sh
$ gulp watch
```

（可选）第三：

```sh
$ karma test
```

#### 建立来源

对于生产版本：

```sh
$ gulp build --prod
```

生成预构建的zip存档以进行分发：

```sh
$ gulp build dist --prod
```

### 码头工人

Dillinger非常容易在Docker容器中安装和部署。

默认情况下，Docker将公开端口8080，因此如有必要，请在Dockerfile中更改此端口。准备就绪后，只需使用Dockerfile构建映像。

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```

这将创建莳萝图像，并引入必要的依赖关系。确保将`${package.json.version}`换成Dillinger的实际版本。

完成后，运行Docker映像并将端口映射到主机上所需的任何端口。在此示例中，我们仅将主机的端口8000映射到Docker的端口8080（或Dockerfile中公开的任何端口）：

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

通过在首选浏览器中导航到服务器地址来验证部署。

```sh
127.0.0.1:8000
```

#### Kubernetes + Google云

参见[KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

### 托多斯

#构建项目基础结构目录小工具

以前做网站做项目，都是先建项目目录结构和基础的HTML文件，还有reset样式的css文件，每次都是重写或拷贝。麻烦。最近折腾node，就想为毛不用node写个小工具，像Ionic构建基础模板文件一样，一行命令就搞定呢？

开始想的名字是varfn，嚓，什么鬼，挖粪？我当初为嘛注册了这么个域名(#‵′)。然后换成了mksite，这几个字母敲键盘好像不顺溜，管它呢。折腾了一下午，基础功能搞定了，将就用了，没研究过怎么弄到npm上，空了吹。

**安装**

没放npmjs网站，所以npm install安装是不行的。下载包文件，拷贝到npm的npm_modules里，两个系统运行文件拷贝到npm的执行文件目录下。环境变量肯定要配的。

**使用**

安装好后，在需要创建项目的目录，打开命令行工具，输入 `mksite start [name] [option]`, name是项目名称，option有两个可选值：base和app，base创建的目录少，app创建的目录多，想改成自己习惯的可以修改config.json文件。

base选项下创建的目录结构：
```
siteName/index.html
    --/css/base.css
    --/sass/base.scss
    --/images
    --/js
    --/upload
    --/test
```

app选项下创建的目录结构：
```
siteName/index.html
    --/css/base.css
    --/sass/base.scss
    --/images
    --/js
    --/upload
    --/test
    --/app
    --/lib
```

版权没有，翻版不究。




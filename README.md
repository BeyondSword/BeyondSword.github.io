# 访问 https://beyondsword.github.io/


# 准备知识
ruby : 编程语言

gem : ruby中的包名

bundle/bundler： 包管理工具， 两者一回事。

jekyll：一个静态网站生成器。

bundle install: 读取 gemfile 安装 gem。

# 构建
1. 检查ruby的安装情况
```
ruby -v
```

2. 安装必要插件(读取 Gemfile)
```
bundle install
```
ruby存在原始源速度很慢的问题，需要进行换源。使用 https://gems.ruby-china.com/ 提供的中国镜像源。

3. 使用 minimal-mistakes 这一主题


plan 2019.8.16:
1.bug md中的标记正常显示   *done* 2019.8.16 method:符号后面加空格
2.本地调试jekyll *done* 2019.8.16
-首先切换源，加快速度
-bundle exec jekyll serve 来本地调试
-出现repo name not found 问题， _config.yml添加repository: BeyondSword/BeyondSword.github.io解决

3.添加导航栏
4.post分类
5.更换主题


2020.1.24 重新开始
此项目利用GitHub pages 功能部署自己的blog，该功能作为过渡使用。


梳理：post中存放文章以markdown格式。 目前使用jekyll来自定义网站页面（官方推荐），jekyll是一个静态网站生成器。
github pages sites 不能改变的固定配置如下：
lsi: false
safe: true
source: [your repo's top level directory]
incremental: false
highlighter: rouge
gist:
  noscript: false
kramdown:
  math_engine: mathjax
  syntax_highlighter: rouge



canonical_url

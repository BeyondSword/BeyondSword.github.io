## 使用 github pages 记录PAT复习


1.blog 下存放blog 索引
2._posts下存放具体的博客内容



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
目前访问使用url: https://beyondsword.github.io/

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

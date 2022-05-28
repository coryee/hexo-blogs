# 使用说明

```shell
git clone git@github.com:coryee/hexo-blogs.git

cd hexo-blogs

```

## 首次初始化
```shell
sudo npm install -g hexo-cli
hexo init
npm install
```
初始化完成后，将在目录下生成如下信息：
```shell
.
├── _config.yml
├── package.json
├── scaffolds
├── source
| 	├── _drafts
|	└── _posts
└── themes
```


# hexo 命令使用
创建新的文章

`hexo new mytitle`

清理临时文件

`hexo clean`

构建网页

`hexo g`

本地运行web服务

`hexo s`

将构建好的静态网页部署到github上

`hexo deploy`


# 遇到的问题
## 无法正常显示mardown中插入的本地图片
**解决方法：**

- 修改`_config.yml`中的`post_asset_folder: true`

- `$ npm install hexo-image-link --save`

- 如果 npm下载比较慢的话，尝试 cnpm下载

- - `$ npm install -g cnpm --registry=https://registry.npm.taobao.org`
  - `$ cnpm install hexo-image-link --save`

- 修改md文件中的图片路径
  ![label](markdown-file-name/image-name.jpg)



# Refs:

[GitHub+Hexo+Next搭建博客 | 于禤的博客 (yxyuxuan.github.io)](https://yxyuxuan.github.io/2019/07/16/GitHub-Hexo-Next搭建博客/)

https://zhuanlan.zhihu.com/p/280758822


# Nest

Nest is a theme for [Pelican](https://getpelican.com) 3.5+, a static site generator written in Python.

我的 [Github Pages](https://maxwell-nc.github.io/) 使用到主题修改，欢迎访问，这个主题由于是自用修改，所有有些地方只有硬编码修改了，没有做通用地处理，如果需要的朋友可以自行修改。

# Live
[https://maxwell-nc.github.io/](https://maxwell-nc.github.io/)

## Some Additions

### 文章内容
主页增强

![Nest Article View](https://raw.githubusercontent.com/maxwell-nc/nest/master/1.jpg)

### 返回顶部
增加文章目录（智能识别层次）

![Nest Article View](https://raw.githubusercontent.com/maxwell-nc/nest/master/2.jpg)

### 返回顶部
增加文章滚动后返回顶部功能

![Nest Article View](https://raw.githubusercontent.com/maxwell-nc/nest/master/3.jpg)

## Features

* Featured site header image
* Featured article header image
* **Pygments** syntax highlighting
* **Disqus** support for comments
* **Google Analytics** support
* **Piwik** support
* RSS and Atom feeds

## Settings

Nest template can be customized by adding parameters to your `pelicanconf.py` file. Template specifics parameters are prefixed with template name.

The header-nav have a fixed heigth of 100px. This is the max size for the logo without css modification.

The min-height for the background header is 360px. The image is displayed using background-size: cover; which scale the background image to be as large as possible so that the background area is completely covered by the background image. If smaller than screen, the image is repeated to fit the background area.

### Pelican.conf example

```python
# NEST Template
THEME = 'Theme/nest'

DEFAULT_DATE_FORMAT = '%Y-%m-%d'

# Add items to top menu before pages
MENUITEMS = [('主页', '/'),('博文目录','/categories.html'),('标签','/tags.html'),('订阅',FEED_ALL_ATOM)]

# Footer
NEST_SITEMAP = False
NEST_SOCIAL_COLUMN_TITLE = u'社交'
NEST_LINKS_COLUMN_TITLE = u'链接'
NEST_COPYRIGHT = u'&copy; Maxwell-nc 2017'

# index.html
NEST_INDEX_HEAD_TITLE = u'主页'
NEST_INDEX_HEADER_TITLE = SITENAME
NEST_INDEX_HEADER_SUBTITLE = u'主要记录学习中遇到的问题和技术分享'
NEST_INDEX_CONTENT_TITLE = u'最新文章'
# archives.html
NEST_ARCHIVES_HEAD_TITLE = u'文档'
NEST_ARCHIVES_HEAD_DESCRIPTION = u'Posts Archives'
NEST_ARCHIVES_HEADER_TITLE = u'Archives'
NEST_ARCHIVES_HEADER_SUBTITLE = u'Archives for all posts'
NEST_ARCHIVES_CONTENT_TITLE = u'Archives'
# article.html
NEST_ARTICLE_HEADER_BY = u'作者'
NEST_ARTICLE_HEADER_MODIFIED = u'修改'
NEST_ARTICLE_HEADER_IN = u'目录'
# author.html
NEST_AUTHOR_HEAD_TITLE = u'作者'
NEST_AUTHOR_HEAD_DESCRIPTION = u'作者'
NEST_AUTHOR_HEADER_SUBTITLE = u'Posts archives'
NEST_AUTHOR_CONTENT_TITLE = u'Posts'
# categories.html
NEST_CATEGORIES_HEAD_TITLE = u'博文目录'
NEST_CATEGORIES_HEAD_DESCRIPTION = u'根据分类显示归档'
NEST_CATEGORIES_HEADER_TITLE = u'博文目录'
NEST_CATEGORIES_HEADER_SUBTITLE = u'根据分类显示归档'
# category.html
NEST_CATEGORY_HEAD_TITLE = u'目录归档'
NEST_CATEGORY_HEAD_DESCRIPTION = u'目录归档'
NEST_CATEGORY_HEADER_TITLE = u'目录'
NEST_CATEGORY_HEADER_SUBTITLE = u'目录归档'
# pagination.html
NEST_PAGINATION_PREVIOUS = u'上一页'
NEST_PAGINATION_NEXT = u'下一页'
# tags.html
NEST_TAGS_HEAD_TITLE = u'标签'
NEST_TAGS_HEAD_DESCRIPTION = u'标签列表'
NEST_TAGS_HEADER_TITLE = u'标签'
NEST_TAGS_HEADER_SUBTITLE = u'标签列表'
NEST_TAGS_CONTENT_TITLE = u'标签列表'
NEST_TAGS_CONTENT_LIST = u'标记为'
#tag.html
NEST_TAG_HEADER_TITLE = u'标签'
```


## Third-party assets

The theme uses external softwares, scripts, libraries and artworks:

* [Bootstrap](http://getbootstrap.com/) 3.x.x

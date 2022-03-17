---
permalink: /
title: "封雨婷"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

> 我是一名来自山东大学软件学院的本科生，导师为[张彩明](https://www.sc.sdu.edu.cn/info/1046/2286.htm)教授.<br/>
> 我的研究兴趣是图像分割与金融大数据。

项目经历
------
## ● Virtual Reality-based Human-Machine Collaboration System
##### 负责基于骨骼追踪的Kinect开发(C#) ,利用获取的骨骼信息控制人机交互与协同。获指导老师高度肯定。
##### 基于VE、HMD、Real-walking遥控机器人实现远程协同。基于Kinect骨骼追踪为基础，模拟平行空间实现远程协同。通过Kinect体感传感器采集人体动作信息，在电脑上进行图像处理，解析出相应的人体动作后建立socket通信向水滴机器人发送相应的控制指令，控制机器人作出实时模仿（行走）或者其他动作;创新使用redirection walking(重定向)实现用户在小范围现实空间漫游大范围虚拟空间;使用Nginx服务器、unity3D搭建流媒体服务器 ,完成视频直播式的虚拟现实场景交互;使用腾讯云TRTC SDK扩展语音通话。

## ● 12307 Train ticketing system
##### 独立完成基于Django的web高性能火车票售票网站开发，功能完善。使用支付宝沙箱技术模拟真实场景支付，使用华为RDS for MySQL作为网站数据库；爬取“中国铁路12306”列车真实数据，数据量接近万级；实现以数据库为核心、产品化导向的数据库应用铁路售票系统。

## ● Box packing based on tournament tree & AVL tree
##### 针对箱子装箱问题，基于竞赛树与AVL树，实现最先匹配法(FF)、最先匹配递减法(FFD)、最优匹配法(BF)、最优匹配递减法(BFD)在内的四种流行算法；前端使用Qt进行图形用户界面设计，加入自主交互式输入箱子数量与物品数量功能模块；测试实现百万级输入，并在简单数字输出的基础上将结果可视化展示。

## ● Student idle goods trading platform
##### 基于 Java、MySQL、Swings 实现 C/S 模式的学生闲置物品交易平台；使用 Socket 进行网络通讯；具有浏览、购买、评论商品，管理商品，买家与卖家私聊，按时间段报表统计销售情况，拍卖等功能
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.

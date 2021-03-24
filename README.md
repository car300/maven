# maven

#### 介绍
maven静态资源仓库，用于对外提供SDK依赖

#### 使用说明

1. 添加仓库
```
allprojects {
    repositories {
        maven { url "https://gitee.com/che300-android/maven/blob/master" }
    }
}
```
2. 引用需要的依赖

#### 更新仓库

1. clone maven静态仓库到本地 https://gitee.com/che300-android/maven.git
2. 在local.properties内添加local.maven，value为maven静态资源仓库本地路径
3. 修改版本号运行uploadArchives task
4. 推送maven静态资源仓库到远程

**注意:** `一定不要手动修改maven静态资源仓库文件`


#### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)

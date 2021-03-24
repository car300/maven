# maven

#### 介绍
maven静态资源仓库，用于对外提供SDK依赖

#### 使用说明

1. 添加仓库
```
allprojects {
    repositories {
        maven { url "https://gitee.com/che300-android/maven/raw/master" }
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

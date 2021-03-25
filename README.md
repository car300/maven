# maven

### 介绍
maven静态资源仓库，用于对外提供SDK依赖

### 使用说明

1. 添加仓库
```
allprojects {
    repositories {
        // gitlab镜像仓库
        maven { url "https://gitlab.com/che300-android/maven/-/raw/main" }
        // github源仓库
        maven { url "https://raw.githubusercontent.com/car300/maven/main" }
    }
}
```
2. 引用需要的依赖

### 更新仓库

1. clone maven静态仓库到本地 `https://github.com/car300/maven.git`
2. 在需要上传到的项目下的 `local.properties` 内添加 `local.maven` 变量
```
local.maven=maven静态资源仓库本地路径
```
3. 更新上传版本号，运行 `uploadArchives` task
4. 推送maven静态资源仓库到远程

**注意 :**  `如非必需，不要手动修改maven静态资源仓库pom文件`

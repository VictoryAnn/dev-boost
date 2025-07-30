1. sdk 安装
```
curl -s "https://get.sdkman.io" | bash
source /Users/ansheng/.sdkman/bin/sdkman-init.sh
sdk install java 17.0.14-tem
sdk default java 17.0.14-tem
```
2. vscode 插件安装
Extension Pack for Java 
```
配置sdk环境
"java.configuration.runtimes": [
      {
        "name": "JavaSE-17",
        "path": "/Users/ansheng/.sdkman/candidates/java/17.0.14-tem",
        "default": true,
      },
    ]
```
3. maven安转
brew install maven
---
name: generate-readme
description: Generate README.md files for projects and individual files.
---

# 生成README.md文件

## How It Works

1. 根据用户需求，生成项目级或文件级的README.md文件


### 生成项目README.md文件

1. 在项目的根目录下生成README.md文件
2. 完整阅读项目文件
3. 在README.md文件中，严格按照 Glob 输出的层级关系，输出项目文件架构。
4. 输出项目启动的顺序、脚本、注意事项、配置文件参数说明等信息；如果是web项目，注意要分别写出前端、后端、数据库的启动顺序、脚本，以及“API路由总览”包含请求方法、URL、作用、输入参数。
5. 最后根据项目及文件特点，补充其他重要信息。

### 生成某个文件的README.md

1. 在目标文件的同级目录下生成 [文件名]-README.md文件
2. 完整阅读该文件
3. 在README.md文件中，输出文件的逻辑架构。
4. 如果是服务器文件，在README.md文件中输出“API 路由总览”，包含请求方法、URL、作用、输入参数、对应代码行数、调用内部函数等信息。
5. 然后，输出“文件运行顺序”说明。
6. 然后，输出“文件所含函数”，包括作用、外部依赖、逻辑等信息。
7. 最后根据项目及文件特点，补充其他重要信息。
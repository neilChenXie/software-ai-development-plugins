---
name: project-based-learn
description: Learn software development through project-based learning, including generating README files, code comments, and
---

## 基于项目学习

### 基于项目制定学习计划

1. 阅读~/.agents/my-skills/文件夹下的文件，了解我已近具有哪些能力
2. 针对这个项目，并根据第一步了解到的我的能力，帮我制定一个学习计划，学习之后能够完全理解整个项目代码，并根据新的需求，进行代码修改。学习内容紧
3. 计划要分为不同阶段，即课程安排，第一课、第二课、以此类推。
4. 每节课内容，需要包含“涉及项目文件”（如果可以，具体到xx文件的xx行）。
5. 每节课的内容，需要密围绕项目内容，且充分包含项目涉及的知识点；项目不涉及的知识点，不列入计划。
6. 学习计划存放在本项目的.my-study/文件夹下，名为study-plan.md.

### 基于学习计划准备课程内容

按照用户的要求的“第n课”输出课程内容
在本项目的.my-study/文件夹下，创建course_[n]/文件夹，如course_1/、course_2/等。
在course_[n]/文件夹，创建的课程内容需包括：
* 本课程内容course_[n]_readme.md，即用于学习的教材
* 用于学习本课程的最小项目，如果是node、java、python等可以运行的，需要项目需要完整可运行的；如果是nginx等无法在文件夹下运行的，给出代码即可。
* 每节课的内容，需要密围绕项目内容，且充分包含项目涉及的知识点；项目不涉及的知识点，不列入计划。

### 用户学完后归档成为用户的my-skills

当用户说，我已经完成了本项目教程的学习。将.my-study/study-plan.md文件，复制到~/.agents/my-skills/文件夹下，并重命名为learned-skill-[date].md；同时将内容中，“我希望学习”等计划时使用的词汇改成“我已完成学习xxx”等完成学习的词汇，课程的划分保持不变。
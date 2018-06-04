# 实验6：基于GitHub的实验管理平台的分析与设计
|学号|班级|姓名|
|:-------:|:-------------: | :----------:|
|201510414127|软件(本)15-1|张继|

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。

## 2. 系统总体结构
![flow1](./img/系统总结结构.png)
[界面设计](https://zhangji123456.github.io/is_analysis/test6/ui/系统首页界面.html)

## 3. 用例图设计 [源码](./src/usecase.puml)
![](./img/用例图.png)

## 4. 类图设计 [源码](./src/class.puml)
![](./img/类图设计.png)

## 5. 数据库设计
- ### [参见数据库设计](./数据库设计.md)

## 6. 用例及界面详细设计

- ### [“登录”用例](./yongli/登录.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/登录界面.html)
- ### [“登出”用例](./yongli/登出.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/登出界面.html)
- ### [“查看用户信息”用例](./yongli/查看用户信息.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“修改用户信息”用例](./yongli/修改用户信息.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“修改用户密码”用例](./yongli/修改用户密码.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“录入课程信息”用例](./yongli/录入课程信息.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/录入课程信息.html)
- ### [“查看选课学生信息”用例](./yongli/查看选课学生信息.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/查看选课学生.html)
- ### [“评定成绩”用例](./yongli/评定成绩.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/评定成绩界面.html)
- ### [“发布实验”用例](./yongli/发布实验.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/发布实验.html)
- ### [“修改实验”用例](./yongli/登出.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/修改实验.html)
- ### [“查看学生完成的实验”用例](./yongli/查看学生完成的实验.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/查看学生完成的实验.html)
- ### [“学期选择”用例](./yongli/学期选择.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/学期选择.html)
- ### [“查看成绩”用例](./yongli/查看成绩.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/查看成绩界面.html)
- ### [“课程选择”用例](./yongli/登出.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/课程选择.html)
- ### [“修改实验”用例](./yongli/登出.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/修改实验.html)
- ### [“查看本课程实验内容”用例](./yongli/查看本课程实验内容.md),[界面](https://zhangji123456.github.io/is_analysis/test6/ui/查看本课程实验内容.html)













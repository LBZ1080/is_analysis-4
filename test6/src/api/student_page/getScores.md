﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getScores  [返回](../../../README.md)
用例： [查看成绩](../../UseCaseSpecification/students/查看成绩.md)

- 权限：
    学生：可以看到自己的成绩
    学生：可以看到同班同学的成绩

- 功能：
    学生查看成绩。

- API请求地址：
   接口基本地址/v1/api/student/getScores&student_id=?

- 请求方式 ：
    GET

- 请求参数说明:

 |参数名称|说明|
 |:---------:|:--------------------------------------------------------|
 |student_id|学生学号|


- 返回实例：

        {
            "name": 孙守利,
            "total": 30,
            "data": [
                "实验一":{
                "评分项1": "实验完整性",
                "评分项2": "实验完整性",
                "评分项3": "实验完整性",
                "权重1": 50,
                "权重2": 30,
                "权重3": 20,
                "分数1": 80,
                "分数2": 80,
                "分数3": 90,
                "总分": 82},
                {
                ...其他实验
                }
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |name|学生名字|
  |total|返回当前课程学生人数|
  |data|返回该学生成绩数据|
# 接口：testContent [返回](../README.md)
用例： [查看本课程实验内容](../yongli/查看本课程实验内.md)

- 功能：
    学生查看本课程实验内容
    
- 权限：
    学生：可以查看本课程所有实验内容
    
- API请求地址： 
    接口基本地址/v1/api/testContent/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的学号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "student_id": "201510414127", 
            "github_username": "zhangji123456", 
            "class": "软件(本)15-1", 
            "name": "zhangji", 
            "total": 6,
            "avgresult":90.5,       
            "data": [
                {
                "test_id":1,
                "web_exists": true, 
                "update_date": "2018-04-02 13:48:01"
                }, 
                {
                ...其他实验
                }
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号|
  |github_username|学生的gitHub用户名|
  |class|班级|
  |name|真实姓名|   
  |test_id|实验编号|


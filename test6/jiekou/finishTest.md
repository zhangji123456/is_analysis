# 接口：finishTest  [返回](../README.md)
用例： [查看学生完成的实验](../yongli/查看学生完成的实验.md)

- 功能：
    老师查看学生完成的实验情况
    
- 权限：
    老师：可以查看所有学生完成的的实验。
    
- API请求地址： 
    接口基本地址/v1/api/finishTest/<student_id>

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
                "result": 90, 
                "memo":"本实验做得好",
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
  |total|实验总数|
  |avgresult|实验平均成绩|   
  |data|所有实验的成绩和评语|
  |test_id|实验编号|
  |web_exists|本实验的GitHub网页是否存在|

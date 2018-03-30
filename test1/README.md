# 业务流程建模
|学号|班级|姓名|
|:----------:|:-----:|:--------:|
|201510414127|15软件1班|张继|

### 流程图1：考试及成绩管理流程
##### PlantUML源码如下：
```
@startuml
start
:教务处安排考试;
:教务处出考试安排表;
:教师出卷;
fork
    :A、B试卷;
fork again
    :教师打印审批表;
    :班主任审批签字;
    :班主任打印审批表;
end fork
:教务处打印试卷;
:试卷;
:学生参加考试;
:学生答卷;
:教师阅卷出成绩;
fork
    :成绩单;
    if(教务处审核是否有不合格？) then  (有)
        :教务处安排补考;
        split
            :补考安排表;
             detach
        split again
            :;
        end split
    endif
fork again
    :答卷;
    :装订成档;
end fork
:期末流程结束;
stop
@enduml
```
##### 业务流程图如下：

![](./StudentTestSystem.png '描述')

### 流程图2：客户维修服务流程
##### PlantUML源码如下：
```
@startuml
start
:客户申请服务;
if(业务经理判断是新客户吗？)then(是)
    :登记客户信息;
else(不是)
endif
:业务经理上门勘察;
:业务经理制定方案;
if(客户是否满意？)then(是)
    :签订服务合同;
    fork
        :业务经理安排工人;
    fork again
        :业务经理安排材料;
    end fork
    :业务经理填写派工单;
    :工人领取材料;
    :工人上门服务;
    :客户验收并填写反馈意见;
    :业务经理交回派工单;
    :财务人员结算收款;
    stop
else(否)
    stop
@enduml
```
##### 业务流程图如下：
![](./UserMaintenance.png '描述')

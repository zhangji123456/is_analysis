# 实验2：图书管理系统用例建模
|学号|班级|姓名|
|:----------:|:-----:|:--------:|
|201510414127|15软件1班|张继|
### 1.图书管理系统的用例关系图
#### 1.1 用例图PlantUML源码如下：
```
@startuml
left to right direction
actor 借书者
actor 游客
actor 图书管理员
actor 系统管理员
rectangle {
    借书者 --> (借阅图书)
    游客 --> (查询图书)
    借书者 --> (归还图书)
    借书者 --> (预订图书)
    借书者 --> (取消预订)
    游客<|-借书者
    图书管理员-->(借出图书)
    图书管理员-->(维护书目):增、删、查、改
    图书管理员-->(维护借书者信息)
    借书者<|-图书管理员
    系统管理员-->(维护图书管理员信息)
    图书管理员<|-系统管理员
}
@enduml
```
#### 1.2 用例图如下：
![](./1.png '描述')
### 2.参与者说明
#### 2.1 游客
    一般游客只具有查询图书的功能
#### 2.2 借书者
    借书者不仅拥有一般游客所具有的功能，并且也具有借阅图书，归还图书，预订图书，取消预订的功能
#### 2.3 图书管理员
    图书管理员不仅具有借书者所具有的功能，并且也具有借出图书，维护数目（增、删、查、改），维护借书者信息的功能
#### 2.4 系统管理员
    系统管理员不仅具有图书管理员所具有的功能，并且也具有维护图书管理员信息的功能
### 3.用例规约表
#### 3.1 借书用例
![](./2.png '描述')
#### 3.2 还书用例
![](./3.png '描述')
#### 还书用例plantUML源码如下：
```
@startuml
start
:借书者还书;
:图书管理员;
if (检查图书是否损坏) then (是)
:借书者办理赔偿手续;
else(否)
:图书管理员输入图书信息;
fork
:系统验证图书信息;
fork again
:系统验证借书者信息;
end fork
fork
:修改借书信息;
fork again
:修改图书状态;
fork again
:修改库存数量;
end fork
:图书管理员确认图书归还完毕;
endif
stop
@enduml
```
#### 还书流程图如下：
![](./4.png '描述')

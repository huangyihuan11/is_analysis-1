<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getOneCourse  [返回](../README.md)
用例：
    [评定成绩](../用例/评定成绩.md)
    [查看成绩](../用例/评定成绩.md)


- 功能：
    课程选择。
    
- 权限：
    学生/老师：修改自己的密码，必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/getOneCourse/<test_id&collage_name&course_name>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|课程编号| 
  |collage_name|院系专业|
  |course_name|课程名|
  
- 返回实例：

        {         
            "status": true,
            "info": null，
            collage_name：“信息科学工程与技术学院”,
			course_name:"java",
            "data": [
                {
                "test_id":#3,
                "test_name":"类的继承1"
				"summery": "本次实验简单认识。。。", 
				"updata_date": "2018.5.22",
				"teacher_name":"黄老师" 

        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |course_id|课程编号| 
  |course_name|课程信息名字|
  |data|实验的基本信息|
  |test_id|实验编号|
  |summery|简介|
  |updata_date|上传时间|
  |teacher_name|教师姓名|
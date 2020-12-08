# -xueshengxuankemoni
学生选课模拟系统
物联网191 邢朝阳
一、实验内容
（一）实验目的： 初步了解分析需求，从学生选课角度了解系统中的实体及其关系，学会定义类中的属性以及方法； 
掌握面向对象的类设计方法（属性、方法）； 掌握类的继承用法，通过构造方法实例化对象；
学会使用super()，用于实例化子类； 掌握使用Object根类的toString（）方法,应用在相关对象的信息输出中。 （二）业务要求： 
说明：学校有“人员”，分为“教师”和“学生”，教师教授“课程”，学生选择“课程”。从简化系统考虑，每名教师仅教授一门课程，每门课程的授课教师也仅有一位，每名学生选仅选一门课程。 对象示例：	人员（编号、姓名、性别……） 教师（编号、姓名、性别、所授课程、……） 			学生（编号、姓名、性别、所选课程、……） 			课程（编号、课程名称、上课地点、时间、授课教师、……） 以上属性仅为示例，同学们可以自行扩展（黄色背景的文字，不能原篇出现在实验报告中，需要进一步明确所有的属性）。 实验要求 1.编写上述实体类以及测试主类（注意类之间继承关系的适用） 2.在测试主类中，实例化多个类实体，模拟学生选课操作、打印课程信息（信息包括：编号、课程名称、上课地点、时间、授课教师 等）；模拟学生退课操作，再打印课程信息。
二、核心方法
创建四个对象：
1）人员 people类（学号、姓名、性别）
 2）Teacher类（ID号、姓名、性别、所授课程） 
3）Student类（学号、姓名、性别、所选课程） 
4）Course类（课程序号、课名、上课地点）

一、	对people类进行编写： 
public class People { private int id；//对people类进行私有化编号属性
 private String peopleName;//定义people类姓名属性
private String peopleSex;//定义people类性别属性
二、教师以及课程信息编写： 
public class Teacher { private int teacherId;//定义教师ID号
private String teacherName;//教师名称属性
 private String teacherSex;//教师性别属性
private Course[]courses;//所授课程属性
三、学生信息编写
public class student {
	public String id;//定义学生编号
	public String name; //定义学生姓名
	public String sex; //定义学生性别
	public String study; 
	public student(String id,String name,String sex,String study)
	{
		this.id = id;
		this.name = name;
		this.sex = sex;
		this.study = study;
	}四、课程信息编写 
public class Course { private String courseName;//课程名称 
private int courseId;//课程编号 
private Teacher teacher;//教授该课程的教师
 private float credit; private Student[] students; public Course(int courseId,String courseName,float credit,Teacher teacher) ……… }

三、实验结果

四、实验感想
通过本次实验，我对Java面向对象编程的基本思想有所了解，并构造了学生老师课程等对象，定义了它们的属性和方法，熟悉了java编程操作。


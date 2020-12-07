# Java-实验-5  Student homework processing system

## 计G202  王超琦  2020322087

## 一.实验目的
    - 掌握字符串String及其方法的使用。
    - 掌握文件的读取/写入方法。
    - 掌握异常处理结构。
    
## 二.实验内容
    1.在某课上,学生要提交实验结果，该结果存储在一个文本文件A中。
    2.在文件A中写学生的本信息。（学生姓名，年龄，性别，班级，学号）
    3.在文件A中写学生处理后的作业信息。（长恨歌的古诗整齐写出）
    4.统计学生作业中某个词或字出现的次数。
    5.需要考虑学生可能写错，要设计异常处理。
    
## 三.实验要求
    - 设计学生类（包括学生姓名，年龄，性别，班级，学号）。
    - 采用交互式方式实例化某学生。（Scanner）
    - 写长恨歌时要求每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”。
    - 允许提供输入参数，统计古诗中某个字或词出现的次数。
    - 输入的文本来源于文本文件B读取，把“古诗处理后的输出”结果存储到学生基本信息所在的文本文件A中。
    
## 四.实验过程
    1.创建学生类，填写学生信息。
      public class Student {
      String Name;
     	String Sex;
      public void setName(String Name) {
 	    this.Name = Name;}
      
    2.划分学生类。
      Student stu=new Student();
      Scanner s=new Scanner(System.in);
      System.out.println("姓名：");		
   	  String Name =s.next();
      
    3.创建文件A,夹把文件A中的内容要求整理并输出到文件B中；并做异常处理。
      while ((fInputStream.read(ch)) !=-1) {
      st.append(ch, 0,7);
      st.append("，");
      st.append(ch, 7, 7);
      st.append("。"+"\n");
      
      FileReader fInputStream = new FileReader("D://JAVA实验5//A.txt");//输入流文件
      FileWriter fOutputStream  = new FileWriter("D://JAVA实验5//A.txt")
     
     	catch (IOException e) 
      e.printStackTrace();
      
    4.提取文件B中的字符，在文件中出现过几次。

          while ((len=fis.read(buffer))!=-1){
		             bos.write(buffer,0,len)；      	}
	              	data = bos.toByteArray();
		           String str1 = new String(data);
           int count=0;
	           	Scanner sc = new Scanner(System.in);
          		 System.out.println("请输入您要查找的字符：");
		              char o = sc.next().charAt(0);
	              	char[] ch1 =str1.toCharArray();
		           for(int i=0;i<ch1.length;i++){
		              if(o==ch1[i]){
		                count++; }
                    
## 五.流程图
![](https://github.com/Wcqsss11/Java---5/blob/main/2d3be7914df64eefbc237d6f4353601.png)

## 六.核心代码 
       try (FileReader fInputStream = new FileReader("F:////A.txt");   
             FileWriter fOutputStream  = new FileWriter("F:////B.txt")){
            StringBuffer st=new StringBuffer();
            while ()  {                    }
                 }
        try{         }；   catch(Exception e) {    }；
        Scanner s=new Scanner(System.in);   
        if( ){                }
## 七.系统运行结果：
![](https://github.com/Wcqsss11/Java---5/blob/main/707a4c169fa59e2db4b7d30394875e8.png)

## 八.实验感想：
- 通过前后五次的实验，我掌握了Java的基本编程规则、知识要点和一些小技巧，特别是对面向对象的编程思想和风格有了进一步的认识和体会。但是在上机调试的时候还是遇到了相当多的问题。很多的错误都很难体会，有的时候是输入的错误，这种错误还是比较容易版找出来的，但是有些问题，；例如本次实验将文件A中的字符读取并输入到文件B中就遇到问题，找了很多同学和我一起去探讨这个问题，最终还是学会了，对于文件夹我终于有了一定的了解，我也深深认识到了自己的不足，望在以后的生活当中好好学习java这一门课程。

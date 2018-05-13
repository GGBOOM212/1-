# -第一周任务
流程控制 demo
判断第一个数是第二个数的多少倍
package t1;
import java.util.Scanner;
public class TestModel
{
    public static void main (String []args)
    {
        Scanner sc=new Scanner(System.in);
        System.out.print("请输入第一个整数：");
        int i=sc.nextInt();
        System.out.print("请输入第二个整数：");
        int j=sc.nextInt();
        if(i%j==0)
        {

            System.out.println(i+"是"+j+"的"+i/j+"倍！");
        }
        else
        {

            System.out.println(i+"不是"+j+"的"+"倍数！");
        }
    }

}

运算符
题目：利用条件运算符的嵌套来完成此题：学习成绩>=90分的同学用A表示，60-89分之间的用B表示，60分以下的用C表示
import java.util.Scanner;
public class ConditionOperator {
    public static void main(String[] args) {
        int x;
        String grade;
        Scanner s = new Scanner(System.in);
        System.out.println("请输入一个成绩：");
        x = s.nextInt();
        grade = x >= 90 ? "A" : x >= 60 ? "B" : "C";
        System.out.println("等级为："+grade);
    }
}


第二周任务作业
import java.util.Scanner;
public class NumberGames {
	public static void main(String[] args) {
		int answer = (int) (Math.random() * 100) + 1;
		Scanner sc = new Scanner(System.in);
		int num = 0;
		int min = 1;
		int max = 100;
		do {
			System.out.println("请输入1表示游戏开始");
			int i=sc.nextInt()
			System.out.println("输入" + min + "到" + max + "值");
			num = sc.nextInt();
			if (num > max || num < min) {
				System.out.println("错误输出");
			} else if (num > answer) {
				System.out.println("答案大了"); 
			} else if (num < answer) {
				System.out.println("答案小了");
			}
			else
			{
				System.out.println("答案正确，中午加鸡腿");
			}
		System.out.println("请输入2表示再来一次,输入0表示退出");
		int j=sc.nextInt();	
		} while (j!=2);
	}
}



# eclipse
import java.util.Scanner;

import javax.swing.JOptionPane;
public class sizeyunsuan {

	public static void main(String[] args) {
		// TODO 自动生成的方法存根
		System.out.println("请选择进行整数或真分数的运算（整数运算请输入1，真分数运算请输入0）");
		Scanner in=new Scanner(System.in);
		int choice;
		choice=in.nextInt();
		if(choice==1)
		{
			for(int i=0;i<30;i++)
				
		{
			int a=(int)(Math.random()*100); //生成一个随机数
		    int b=(int)(Math.random()*100); //生成一个随机数
		    int y=(int)(Math.random()*10000); //生成一个随机数
		    int x=y%4;
		    if(x==0)
		    {
		    	System.out.println(a+"+"+b+"=");
		    	}
		    else if(x==1)
		    {
		    	System.out.println(a+"-"+b+"=");
		    	}
		    else if(x==2)
		    {
			    System.out.println(a+"*"+b+"=");
			    }
		    else if(x==3)
		   {
		    	int a1=0;
		    	int b1=0;
		    	while(b1-a1<0||b1==0)
		    	{
		    		a1=(int)(Math.random()*100); //生成一个随机数
		            b1=(int)(Math.random()*100); //生成一个随机数
		            }
		    	System.out.println(a1+"/"+b1+"=");
		   }
		    }
		}
			else if(choice==0)
			{
				for(int i=0;i<30;i++)
				{
					int a,b,c,d;
			        a=0;
			        b=0;
			        c=0;
			        d=0;
			        while(b==0||d==0||b-a<0||d-c<0)
			        {
			        	a=(int)(Math.random()*100); //生成一个随机数
		                c=(int)(Math.random()*100); //生成一个随机数
				        b=(int)(Math.random()*100); //生成一个随机数
				        d=(int)(Math.random()*100); //生成一个随机数
				    }
			    int y=(int)(Math.random()*10000); //生成一个随机数
			    int x=y%4;
		        if(x==0)
		        {
		        	System.out.println(a+"/"+b+" + "+c+"/"+d+" = ");
		        	}
		        else if(x==1)
		        {
		        	System.out.println(a+"/"+b+" - "+c+"/"+d+" = ");
		        	}
		        else if(x==2)
		        {
			        System.out.println(a+"/"+b+" * "+c+"/"+d+" = ");
			        }
		       else if(x==3)
		        {
		        	int a1=0;
			    	int b1=0;
			    	int c1=0;
			    	int d1=0;
			    	while(b1==0||c1==0||a1-b1>=0||c1-d1>=0)
			    	{
			    		a1=(int)(Math.random()*100); //生成一个随机数
			            c1=(int)(Math.random()*100); //生成一个随机数
					    b1=(int)(Math.random()*100); //生成一个随机数
					    d1=(int)(Math.random()*100); //生成一个随机数
					    }
			    	System.out.println(a+"/"+b+" / "+c+"/"+d+" = ");
			    	}
				}
			}
		        else
		        {
		        	System.out.println("选择出错");
		        	}
		}
}

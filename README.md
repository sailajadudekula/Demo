interface calculatorAPI{
    void sum(int a,int b);
    void sub(int a,int b);
    void mul(int a,int b);
    void div(int a,int b);
    }
    class calculator implements calculatorAPI{
        
    public void sum(int a,int b)
    {
        int c=a+b;
        System.out.println(c+" ");
    }
    public void sub(int a,int b)
    {
        int c=a-b;
        System.out.println(c+" ");
    }
    public void mul(int a,int b)
    {
        int c=a*b;
        System.out.println(c+" ");
    } 
    public void div(int a,int b)
    {
     int c=a%b;
     System.out.println(c+" ");
    }
}
public class Main
{
    public static void main(String[] args) 
	{
	calculatorAPI c=new calculator();
	 c.sum(10,20);
	 c.sub(10,20);
	 c.mul(10,20);
	 c.div(10,20);
	 
    }
}

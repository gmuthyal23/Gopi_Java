package com.company;
public class bank {
    private String ename;
    private String email;
    private int phone;
    private double amount= 0.0;
    private double balance=0;
    private double withdrawl;

    public void setdeposit( double deposit)
    {
        this.balance += deposit;
        System.out.println("deposit of" + deposit + "made new balance is" + this.balance);
    }
public void setWithdrawl(double withdrawl)
{
    this.balance-=withdrawl;
    System.out.println("withdrawl Amount:" + withdrawl + "New Balance:" + this.balance);
}

double sum=0;

    public void setname(String ename) {
        String name= ename;
        if(name.equals("gopi") || name.equals("nath")) {
            this.ename = ename;
        }
        else
            this.ename="Unknown";
    }

    public String getname()
    {
        return this.ename;
    }

    public void setemail(String email)
    {
        String Email=email;
        if(Email.equals("Test") || Email.equals("test"))
        {
            this.email=email;
        }else
            this.email="Unknown";
    }

    public String getEmail()
    {
        return this.email;
    }

   public void setphone(int phone)
    {
        this.phone = phone;
    }
        public int getphone()
        {
            return this.phone;
        }
public void setamount(double amount)
{
    sum += amount;
        this.amount=amount;
}
public double getAmount()
{
 sum=amount;
    return this.amount;
}

}

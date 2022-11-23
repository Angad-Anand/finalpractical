1-Sum and average-
	import java.util.Scanner;
	public class Sum_Average
	{
	    public static void main(String[] args) 
	    {
	        int n, sum = 0;
	        float average;
	        Scanner s = new Scanner(System.in);
System.out.print("Enter no. of elements you want in array:");
        n = s.nextInt();
	        int a[] = new int[n];
        System.out.println("Enter all the elements:");
        for(int i = 0; i < n ; i++)
        {
          a[i] = s.nextInt();
	            sum = sum + a[i];
	        }
	        System.out.println("Sum:"+sum);
	        average = (float)sum / n;
       System.out.println("Average:"+average);
}
}

2-To read a file using java reader

package net.codejava.io;
 
import java.io.FileReader;
import java.io.IOException;
 

public class TextFileReadingExample1 {
 
    public static void main(String[] args) {
        try {
            FileReader reader = new FileReader("MyFile.txt");
            int character;
 
            while ((character = reader.read()) != -1) {
                System.out.print((char) character);
            }
            reader.close();
 
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
 

3. To write on file using java reader
package net.codejava.io;
 
import java.io.FileWriter;
import java.io.IOException;
 
/**
 * This program demonstrates how to write characters to a text file.
 * @author www.codejava.net
 *
 */
public class TextFileWritingExample1 {
 
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("MyFile.txt", true);
            writer.write("Hello World");
            writer.write("\r\n");   // write new line
            writer.write("Good Bye!");
            writer.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
 
    }
 
}

4-Bubble sort in java
import java.util.Scanner;

public class CodesCracker
{
   public static void main(String[] args)
   {
      int n=10, i, j, x;
      int[] array = new int[n];
      Scanner s = new Scanner(System.in);
      
      System.out.print("Enter 10 Elements in Random Order: ");
      for(i=0; i<n; i++)
      {
         array[i] = s.nextInt();
      }
      
      for(i=0; i<(n-1); i++)
      {
         for(j=0; j<(n-i-1); j++)
         {
            if(array[j]>array[j+1])
            {
               x = array[j];
               array[j] = array[j+1];
               array[j+1] = x;
            }
         }
      }
      
      System.out.println("\nThe new sorted array is:");
      for(i=0; i<n; i++)
         System.out.print(array[i]+ " ");
   }
}

5- get ip address using swings
import java.net.InetAddress;

class GetMyIPAddress
{
   public static void main(String args[]) throws Exception
   {
      
      InetAddress myIP=InetAddress.getLocalHost();
      System.out.println("My IP Address is:");
      System.out.println(myIP.getHostAddress());
  }
}
5-Sum and average using java aaplet
	import java.awt.*;  
	import java.awt.event.*;  
	import java.applet.*;  
	public class Q2 extends Applet implements ActionListener  
	{  
	    TextField t1 = new TextField(10);  
	    TextField t2 = new TextField(10);  
	    TextField t3 = new TextField(10);  
	    Label l1 = new Label("FIRST NO=:");  
	    Label l2 = new Label("SECOND NO:");  
	    Label l3 = new Label("SUM:");  
	    Button b = new Button("ADD");  
	    public void init()  
	    {  
	        t1.setForeground(Color = Red);  
	        add(l1);  
	        add(t1);  
	        add(l2);  
	        add(t2);  
	        add(l3);  
	        add(t3);  
	        add(b);  
	        b.addActionListener(this);  
	    }  
	    public void actionPerformed(ActionEvent e)  
	    {  
	        if (e.getSource() == b)  
	        {  
	            int n1 = Integer.parseInt(t1.getText());  
	            int n2 = Integer.parseInt(t2.getText());  
	            t3.setText(" " + (n1 + n2));  
	        }  
	    }  
	}  
	<HTML>  
	  
	    <HEAD>  
	        <TITLE>WELCOME TO JAVA APPLET</TITLE>  
	    </HEAD>  
	  
	    <BODY>  
	        <CENTER>  
	            <H1>WELCOME TO THE APPLET</H1> </CENTER>  
	        <BR>  
	        <APPLET CODE=Q2.class WIDTH=400 HEIGHT=400> </APPLET>  
	    </BODY>  
	  
	</HTML>  




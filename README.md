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
 
/**
 * This program demonstrates how to read characters from a text file.
 * @author www.codejava.net
 *
 */
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
 

To write on file using java reader
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

3-Bubble sort in java
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

4- get ip address using swings
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
1.	import java.awt.*;  
2.	import java.awt.event.*;  
3.	import java.applet.*;  
4.	public class Q2 extends Applet implements ActionListener  
5.	{  
6.	    TextField t1 = new TextField(10);  
7.	    TextField t2 = new TextField(10);  
8.	    TextField t3 = new TextField(10);  
9.	    Label l1 = new Label("FIRST NO=:");  
10.	    Label l2 = new Label("SECOND NO:");  
11.	    Label l3 = new Label("SUM:");  
12.	    Button b = new Button("ADD");  
13.	    public void init()  
14.	    {  
15.	        t1.setForeground(Color = Red);  
16.	        add(l1);  
17.	        add(t1);  
18.	        add(l2);  
19.	        add(t2);  
20.	        add(l3);  
21.	        add(t3);  
22.	        add(b);  
23.	        b.addActionListener(this);  
24.	    }  
25.	    public void actionPerformed(ActionEvent e)  
26.	    {  
27.	        if (e.getSource() == b)  
28.	        {  
29.	            int n1 = Integer.parseInt(t1.getText());  
30.	            int n2 = Integer.parseInt(t2.getText());  
31.	            t3.setText(" " + (n1 + n2));  
32.	        }  
33.	    }  
34.	}  


35.	<HTML>  
36.	  
37.	    <HEAD>  
38.	        <TITLE>WELCOME TO JAVA APPLET</TITLE>  
39.	    </HEAD>  
40.	  
41.	    <BODY>  
42.	        <CENTER>  
43.	            <H1>WELCOME TO THE APPLET</H1> </CENTER>  
44.	        <BR>  
45.	        <APPLET CODE=Q2.class WIDTH=400 HEIGHT=400> </APPLET>  
46.	    </BODY>  
47.	  
48.	</HTML>  




import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class Jala {
	public static void main(String[] args) throws FileNotFoundException {
  FileInputStream fis = new FileInputStream("myfile.txt");
        Scanner in = new Scanner(fis);
        while(in.hasNext())
        {
        	String line = in.nextLine();
        	System.out.println(line);
        }
	}
}

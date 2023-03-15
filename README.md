import java.util.*;
import java.lang.Math;

public class Main
{
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		
		ArrayList<Integer> diffs = new ArrayList<Integer>();
		int input_value;
		long sum = 0;
		int diff;
		
		int n = scanner.nextInt();
		int k = scanner.nextInt();
		
		for (int i = 0; i < n; i++) {
		    input_value = scanner.nextInt();
		    //System.out.println(Math.log10(input_value));
		    //System.out.println((int)Math.log10(input_value));
		    //System.out.println(Math.log10(input_value) % 1);
		    //System.out.println(Math.pow(10, (int)Math.log10(input_value) + 1) - 1);
		    //diff = (int)Math.pow(10, (int)Math.log10(input_value) + 1) - 1;
		    diffs.add(i, (int)Math.pow(10, (int)Math.log10(input_value) + 1) - 1 - input_value);
		    System.out.println(diffs.get(i));
		}
		
		scanner.close();
	}
}

# Decoding

import java.util.*;

public class Algo{
	public static void main(String[] args){
	Scanner scan = new Scanner(System.in);
	String temp = "666 88 8 7 88 8 0 2 0 8 444 6 33 7777 0 22 0 6 444 66 88 7777 0 2 0 6 444 66 88 7777 0 22 0 7 555 88 7777";
	System.out.println(code(temp));
	}
	public static StringBuilder code(String s){
		StringBuilder str = new StringBuilder();
		String[] arr = s.split(" ");
		for(int i = 0; i < arr.length; i++){
			switch(arr[i]){
				case "0": str.append(' '); break;
				case "1": str.append('.'); break;
				case "2": str.append('a'); break;
				case "22": str.append('b'); break;
				case "222": str.append('c'); break;
				case "3": str.append('d'); break;
				case "33": str.append('e'); break;
				case "333": str.append('f'); break;
				case "4": str.append('g'); break;
				case "44": str.append('h'); break; 
				case "444": str.append('i'); break;
				case "5": str.append('j'); break;
				case "55": str.append('k'); break;
				case "555": str.append('l'); break;
				case "6": str.append('m'); break;
				case "66": str.append('n'); break;
				case "666": str.append('o'); break;
				case "7": str.append('p'); break;
				case "77": str.append('q'); break;
				case "777": str.append('r'); break;
				case "7777": str.append('s'); break;
				case "8": str.append('t'); break;
				case "88": str.append('u'); break;
				case "888": str.append('v'); break;
				case "9": str.append('w'); break;
				case "99": str.append('x'); break;
				case "999": str.append('y'); break;
				case "9999": str.append('z'); break;
			}
		}
		return str;
	}
}

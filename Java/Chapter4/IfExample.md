## if와 if-else
package kr.java.chapter4;

import java.util.Scanner;

public class IfExample {

	public static void main(String[] args) {
		int age = 9;
		int charge;
		if(age < 8) {
			charge = 1000;
			System.out.println("취학 전 아동입니다.");
		}
		else if(age < 14) {
			charge = 2000;
			System.out.println("초등핵생입니다.");
		}
		else if(age < 20) {
			charge = 2500;
			System.out.println("중, 고등학생입니다.");
		}
		else {
			charge = 3000;
			System.out.println("일반인입니다.");
		}
		System.out.println("입장료는" + charge + "원입니다.");
		
		
		//실습 if-else if-else
		Scanner scanner = new Scanner(System.in);
		
		System.out.println("정수 입력");
		String str = scanner.nextLine();
		
		int num = Integer.parseInt(str);
		if (num > 0) {
			System.out.println("양수");
		}
		else if (num < 0) {
			System.out.println("음수");
		}
		else {
			System.out.println("0입니다.");
		}

	}

}
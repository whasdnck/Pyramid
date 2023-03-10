# Pyramid

## 피라미드 설명 

### 1단 -< 별 1 + 공 3 (반복)
### 2단 별3 공1      전체단 
### 3단 별5 공0 -> n-(현재단)

### n단   (n-1) x 2+1
### 개    현재단

### n=3 -> i=1(i<=n) -> 공백 i=1(i<=n-i) -> NO 별 j=1(j<=(i-1)x2+1
### 별 출력  n= 전체단(사용자입력), i= 현재 출력중인 단,,


# Pyramid code
package sungil21102algo;

public class Pyramid {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int i;
		int j;
		int k;
		int num=4;
		
		for(i=0; i<num; i++) {
			for(j=1; j<num-i; j++) {
				System.out.print(" ");// 공백 출력
			}
			
			for(k=0; k<i*2+1; k++) {
				System.out.print("*");// * 출력
			}
			System.out.println();
		}
	}
}

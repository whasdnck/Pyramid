# Pyramid

# Pramid 설명 

### 피라미드를 자바라는 언어로 만들었다.
### 피라미드는 공백과 별 출력 이라는 것을 적용 시켜야하고,
### 그걸 적용 시킬려면 for문이라는 반복문을 적용시켜야 한다.
### 그리고 공백이 없으면 피라미드에 형태 유지를 못하고 공백이 있으면 피라미드 모형이 유지를 해야한다.
### 그리고 그 for문 안에 공백 출력과 별 출력을 해야한다.
### 피라미드에 들어가는 별의 개수를 묻는다면 별 개수를 샐수 있는 식이 있는데 (현재증 -1)*2+1 개 로 구할수있다.
### 그리고 실행을 시키면 따로 숫자를 안적어도 홀수 개씩 피라미드 모형을 만들수있다.
### (i = 현재층, n = 전체층)
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

## 1. 두 자연수 a, b를 입력받아 a / b 결과를 소수점 20째자리까지 출력하는 프로그램을 작성. 
출제 의도 : 파이썬의 소숫점 출력방식 파악.

### 입력 형식 
첫 번째 줄에 a, b가 공백을 사이에 두고 주어집니다.
- 1 ≤ a, b ≤ 100

### 출력 형식
- a / b 결과를 소수점 20째자리까지 출력합니다.

### 예제1

```:python
# 입력
3 5
```

```:python
# 출력
0.60000000000000000000
```

### 예제2
```:python
# 입력
3 7
```

```:python
# 출력
0.42857142857142857142
```

# 2. 백준 1789 (난이도 : 실버5) 
[링크](https://www.acmicpc.net/problem/1789)
## 서로 다른 N개의 자연수의 합이 S라고 한다. S를 알 때, 자연수 N의 최댓값은 얼마일까?

### 입력 형식 
첫째 줄에 자연수 S(1 ≤ S ≤ 4,294,967,295)가 주어진다.

### 출력 형식
첫째 줄에 자연수 N의 최댓값을 출력한다.

### 예제1

```:python
# 입력
200
```

```:python
# 출력
19
```

## 3. CNN 에 사용되는 MaxPooling의 개념과 비슷한 문제 (난이도 : 실버2)
[링크](https://www.acmicpc.net/problem/17829)
MaxPooling이란 nxn 크기의 필터에서 가장 큰 값만 뽑아내는 방법이다.

## 문제
조기 졸업을 꿈꾸는 종욱이는 요즘 핫한 딥러닝을 공부하던 중, 이미지 처리에 흔히 쓰이는 합성곱 신경망(Convolutional Neural Network, CNN)의 풀링 연산에 영감을 받아 자신만의 풀링을 만들고 이를 222-풀링이라 부르기로 했다.

다음은 8×8 행렬이 주어졌다고 가정했을 때 222-풀링을 1회 적용하는 과정을 설명한 것이다

1. 행렬을 2×2 정사각형으로 나눈다.
2. 각 정사각형에서 2번째로 큰 수만 남긴다. 여기서 2번째로 큰 수란, 정사각형의 네 원소를 크기순으로 a4 ≤ a3 ≤ a2 ≤ a1 라 했을 때, 원소 a2를 뜻한다.
3. 2번 과정에 의해 행렬의 크기가 줄어들게 된다.

종욱이는 N×N 행렬에 222-풀링을 반복해서 적용하여 크기를 1×1로 만들었을 때 어떤 값이 남아있을지 궁금해한다.
랩실 활동에 치여 삶이 사라진 종욱이를 애도하며 종욱이의 궁금증을 대신 해결해주자.

![image](https://user-images.githubusercontent.com/38518648/177464538-f7e8e316-0f36-4857-a1bb-25caa0206e55.png)


## 입력 형식
첫째 줄에 N(2 ≤ N ≤ 1024)이 주어진다. N은 항상 2의 거듭제곱 꼴이다. (N=2K, 1 ≤ K ≤ 10)
다음 N개의 줄마다 각 행의 원소 N개가 차례대로 주어진다. 행렬의 모든 성분은 -10,000 이상 10,000 이하의 정수이다. 

## 출력 형식
마지막에 남은 수를 출력한다.

### 예제1

```:python
# 입력
4
-6 -8 7 -4
-5 -5 14 11
11 11 -1 -1
4 9 -2 -4
```

```:python
# 출력
11
```
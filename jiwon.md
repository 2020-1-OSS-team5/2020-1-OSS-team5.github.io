# 자기소개

읽기 전에, 더 많은 사진 자료를 원하시면 [Prezi](https://prezi.com/view/giBSIUEyhp5GyBb8k2Gg/)를 참고

## 인적사항

| 구성 | 내용 |
|----:|:----|
| 이름 | 이지원 |
| 영문 | LEE JI WON | 
| 학교 | 선문대학교 |
| 학과 | 글로벌소프트웨어학과|
| 구분 | 재학중|
| 전화번호 | 010-7233-6259 |
| Email | jiwonlee0308@sunmoon.ac.kr |

## 교육연수
* 2017 전공별 유학프로그램(필리핀 딸락)
* 2019 해외 전공연수(미국 알래스카) - KDD2019 참여  
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTOgrA0RSMTD9mSGWeUSSmk-_NCZMNnv6H7rQ&usqp=CAU">

## 수상
* 2018 글로벌소프트웨어학과 제2회 학술제(외국어말하기대회) - 동상  
* 2019 글로벌소프트웨어학과 제3회 학술제(SW경진대회) - 대상(총장상)  
* 2019 한국소프트웨어종합학술대회 - 포스터발표, 논문기재  
* 2020 한국컴퓨터종합학술대회 - 논문  
<img src="https://www.dailycc.net/news/photo/201911/566307_456178_3649.jpg" height="200">  

## 프로젝트 및 논문

한국 청소년의 자살 잠재성 예측 모델 
-------

### 연구목표
1. 5년간의 데이터를 이용해 시의성과 보편성을 반영함
2. 자살 잠재성과 관련이 있는 변수를 통해 정확도를 높임
3. 판별분석, Random forest, logistic regression, ANN의 모델 비교를 통해 성능확인

### 구현
1. 청소년 건강행태조사 5년간(2014년~2018년)의 데이터 이용
2. 공통된 변수 132개 중 logistic regression을 통해 변수를 추출 후, 카이제곱검정을 통해 통계량 유의확률 0.05%이하인 변수 12개 선정
3. 연도별 판별분석, Random forest, logistic regression, ANN의 정확도, 민감도, 특이도를 분석해 비교분석

### 결과 
> 글로벌소프트웨어학과 제3회 학술제(SW경진대회) - 대상(총장상)
> 한국소프트웨어종합학술대회2019 - 포스터발표, 논문기재

> 자세한 내용은 [논문](http://www.dbpia.co.kr.libproxy.sunmoon.ac.kr/journal/articleDetail?nodeId=NODE09301980 "paper1")을 참조  

방송시청률을 이용한 사회적 행동변화 분석
------

### 연구목표
* 기존의 연구들은 시청률 데이터의 내적요인을 분석 예측하는 방법에 집중되어 왔으나, 본 논문에서는 **COVID-19 감염추이 데이터(외적요인)** 와 **방송 콘텐츠 데이터(내적요인)** 를 분석해 **사회적 변화를 감지할 수 있다** 는 근거를 찾음

### 분석
COVID-19 발생구간과 장르, 성별, 연령별로 나눠 시청률의 비교분석한 결과 공통점과 차이점이 있었으나, 
차이점이 두드러지고 변화한다는 점에서 외적요인이 시청률의 변화에 영향을 미친다는 사실을 증명함

### 결과
> 한국컴퓨터종합학술대회2020 - 동영상발표, 논문기재 (7월 예정) 



## Code 공유

자료구조의 코딩 테스트를 연습하던 중, 버블정렬(Bubble Sort)를 공유함

### Bubble Sort란?
* 두 인접한 원소를 검사하여 자리를 바꾸는 과정을 반복하며 정렬하는 방법  
<img src="https://gmlwjd9405.github.io/images/algorithm-bubble-sort/bubble-sort.png"> 
> 랜덤으로 1부터 100사이의 임의의 숫자 5개를 생성해 For문을 이용해 오름차순으로 정렬함

```python
    import random

    arr = random.sample(range(1, 100), 5) 
        print("정렬 전 :", arr) 

        def bubbleSort(arr):
            for i in range(len(arr)-1, 0, -1):
                for j in range(0, i):
                    if arr[j] > arr[j+1]:
                    arr[j], arr[j+1] = arr[j+1], arr[j] # 자리 바꿈
                print(arr)
            return arr
 
        print("정렬 후 :", bubbleSort(arr))
```

*본 코드는 아직 미흡한 코드이므로, 더 나은 방법이나 의견 주세요.

## 마무리

과제를 진행하면서 어떤 주제로 해야할지가 가장 난해했지만, 현재 본인이 많은 생각을 하고 필요한 이력서를 기반으로 과제를 하였다. 이를 통해, 다른 조원들에게 도움을 주는 계기가 되었으면 좋겠다.  
 

# 김민수  자기소개

## 인적사항
| 구성 | 내용 |
|----:|:----|
| 이름 | 김민수 |
| 생년월일 | 2000.11.06 |
| 학교 | 선문대학교 |
| 학과 | 글로벌 소프트웨어 |
| 학번 | 2019315015 |
| 전화번호 | 010-8651-9714 |
| E-mail | k21332133@naver.com |

## 전공 선택 배경
일찍이 게임을 접하게 되었고, 그런 게임을 만드는 사람이 되고 싶다는 막연한 생각을 함에서 출발해, 스카이프, 디스코드와 같이 편의성을 주는 많은 프로그램들을 접하게 되었고 그런 프로그램들에 존재하는 Bot의 기능을 직접 추가해보고 싶다는 생각이 영향을 끼쳐 전공까지 선택하게 되었다.

## 기억에 남는 코딩관련 대목
> 코딩은 컴퓨터에게 길을 가라고 하는 것이 아니라, 함께 가며 길을 알려주는 것이다.

## 대학 기간 중 목표
**1. 전공능력 향상**  
* python, java와 같은 언어실력  
* 인공지능 러닝방식 이해  
* 많은 알고리즘 이해  

**2. 외국어 능력 향상**  
* 영어  

**3. 유의미한 프로젝트**  
* ex)연구실 프로젝트 등

**4. 취업**  

## 교과목
### 좋았던 교과목
- **데이터 사이언스 개론** : 멀게만 느껴졌던 인공지능이 한걸음 가깝게 느껴지게한 교과목.  
- **컴퓨터 데이터 구조** : 실제로 쓰이는 자료구조를 python으로 직접 만들어보면서 좀 더 잘 이해할 수 있는 기회가 주어진 교과목.  

### 기대되는 교과목  
- **DB설계와 활용** : 빅데이터에도 관심이 많기 때문에 데이터베이스 개념에도 관심이 있음.
- **데이터 인공지능** : 인공지능을 직접 설계하고 만들어 볼 수 있을 것 같아서.  

## 재밌게 플레이한 관련 게임
### Hacknet

<img src = https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSdvG4F1jIbI4TyACKDy48ndTPILE9u8XO3hQ&usqp=CAU>
* CLI와 GUI를 적절히 합쳐놓은 해킹시뮬레이션 게임이다.[트레일러](https://www.youtube.com/watch?v=A-jN16bNPhk/ "hacknet trailer")

## 처음만든 포커 탑 게임
```python
import random

def get_card():
    num = random.randint(1,13)
    if num == 1 :
        num = "A"
    elif num == 11 :
        num = "J"
    elif num == 12 :
        num = "Q"
    elif num == 13 :
        num = "K"
    shape = random.choice(["Spade","Heart","Diamond","Clover"])
    card = str(num)+" "+str(shape)

    global user_hand; global cpu_hand

    if (card in user_hand) or (card in cpu_hand) :
        return get_card()
    else :
        return card


def top_judgment(user_hand,cpu_hand):
    user_hand = user_hand.split()
    cpu_hand = cpu_hand.split()

    hand = [user_hand,cpu_hand]
    score = [0,0]

    for i in range(2):
        if 'A' in hand[i]:
            score[i] += 14
        elif 'J' in hand[i]:
            score[i] += 11
        elif 'Q' in hand[i]:
            score[i] += 12
        elif 'K' in hand[i]:
            score[i] += 13
        else :
            score[i] += int(hand[i][0])

    shape = ["Spade","Diamond","Heart","Clover"]

    print('User hand',user_hand ,'\n Cpu hand',cpu_hand)
    if score[0] == score[1]:
        if shape.index(hand[0][1]) < shape.index(hand[1][1]):
            print('"You Win!!"')
        else:
            print('"You Lose"')
    else :
        if score[0] > score[1]:
            print('"You Win!!"')
        else:
            print('"You Lose"')

user_hand = ''; cpu_hand = ''
user_hand = get_card()
cpu_hand = get_card()

print("당신의 핸드카드",user_hand)

top_judgment(user_hand,cpu_hand)
```

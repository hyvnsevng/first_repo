# 제목1
## 제목2
### 제목3
#### 제목4
##### 제목5
###### 헤딩은 최대 6개까지

--- 

헤딩은 글씨크기 조절용 X \
주제 나누기 위해 사용

Notion 에서 table of content -> 목차를 생성하는 용도 \
이 때 heading으로 구분되어 목차를 자동 생성


## 리스트

1. 첫번째 리스트
2. 두번째 리스트
    1. 두번째의 첫번째 리스트
        1. 두첫첫
3. 세번재 리스트


순서가 없는 리스트
-  dash
* star
+ plus
- 어느 것 사용해도 동일하게 나타남
    + 빈 동그라미
        - 네모
            * 네모
                * 네모
- 편하게 리스트를 구조화 시켜서 사용 가능
    - 같은 선상에 위치시키면 그 곳부터 이어서 리스트를 계속 생성할 수 있음


혼용해서 사용 가능

1. 순서가 잇는 리스트에
    - 순서가 없는 리스트 사용도 가능


- 순서가 없는 리스트에
    1. 순서가 있는 리스트 사용도 가능

## 소스코드

소스코드를 붙여 넣을 때
```python
print("Helo")
if x<10:
    print("x는 10보다 작습니다.")

else:
    print("x는 10보다 크거나 같습니다.")
```

- 코드 블럭은 백틱(물결따옴표) 3개로 감싸주자 !
- 열리는 백틱 뒤에 언어를 명시해주면 하이라이팅 → 가독성 좋아짐
- Mattermost에서도 마크다운 문법 사용가능

만약 한 줄만 코드로 표시하고 싶을 때 \
→ **백틱 하나로 감싸주면 됩니다.**

`print('Hello')`

- 그냥 강조하고 싶을 때도 사용



## 링크 & 이미지

- 특정 주소를 사용해 다른 페이지로 이동하는 링크 혹은 이미지 출력

---
**링크**

`[텍스트정보](링크)`

[예시](https://edu.ssafy.com)\
[AI계의 google](https:/www.perplexity.ai/)

---
**이미지**

`![이미지대체텍스트](이미지주소)`

- 웹 상의 이미지 \
![Lorem Picsum Image](https://picsum.photos/200/300)

- 로컬 환경(PC 안) 상 이미지\
![Local Image](img.jpg)\

- markdown 문법은 이미지 크기 조정 기능 지원하지 않음
    - html을 사용해서 조정 가능

<img src="img.jpg" width="300">


## 텍스트 관련 문법

- 텍스트 **볼드체**
- 텍스트 *기울기*
- 텍스트 ~~취소선~~

`--- : 수평선`

---

### 기타 사용법


`> 인용문구`
> blockquote
>> 인용문구의 인용은 >의 개수로 조절 가능


---

### **표 만들기**

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | 

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
| **왼쪽 정렬**  | **가운데 정렬**  |  **오른쪽 정렬**|





### 체크리스트 작성 (Vscode 에서는 지원 X)

- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed


---

### 마크다운 작성을 도와주는 에디터

- Typora(유료)
- MarkText(유료)
- Markdown All in One(VSCode 확장프로그램)
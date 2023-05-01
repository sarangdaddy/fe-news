<details>
<summary>Feature List</summary>
 </br>

1. JournalHeader 영역
- [x] : JournalHeader에 "전체 언론사" "구독중인 언론사" 클릭시의 이벤트를 부여한다.
- [x] : "전체 언론사" 클릭시 JournalHeaderStore은 "ALL"의 상태를 가진다.
- [x] : "구족중인 언론사" 클릭시 "SUB"의 상태를 가진다.
- [x] : 이벤트 발생과 동시에 JournalHeader의 클릭된 "항목"의 글씨가 굵어지는 렌더링이 일어난다.

2. Journal 그리드 영역
- [x] : JournalHeaderStore에 JournalListAll = [], JournalSubList = []의 상태를 가진다.
- [x] : JournalHeaderStore의 상태("ALL", "SUB")에 따라 해당하는 리스트를 렌더링 해준다.
- [x] : 각 언론사에 마우스를 올리면 [구독하기] 버튼 보이도록 한다.
- [ ] : 이미 구독하고 있는 언론사의 경우 [해지하기] 버튼이 보이도록 한다.
- [x] : Journal의 "구독" 버튼을 누르면 JournalSubList배열에 추가된다.
- [x] : Jounnal의 "해지" 버튼을 누르면 JournalSubList배열에서 해당 언론사가 제거된다.
- [x] : [내가 구독한 언론사] 클릭시 구독을 누른 언론사만 보이게 한다.
- [ ] : 구족중인 언론사위에 마우스를 올리면 [구독해지] 버튼이 나온다
- [x] : 구독해지시 즉시 렌더링 되도록 한다.

3. Journal 디테일(전체) 영역
- [x] : 244개의 언론사를 카테고리로 분류한다. (상단에 카테고리 영역 구성)
- [x] : 선택된 카테고리 이름 옆에 해당 카테고리에 속해있는 언론사의 갯수와 순서를 표시한다.
- [x] : 언론사의 순서는 랜덤으로 정해진다.
- [x] : 아래 화면에는 현재의 언론사 내용을 표시한다.
- [x] : 좌우 화살표로 다음, 이전 언론사로 넘어가도록 한다.
- [x] : 각 카테고리 클릭시 해당 언론사 리스트로 이동한다.
- [x] : 언론사 내용에는 구독하기 버튼을 추가한다.
- [ ] : 구독하기 클릭 시 "내가 구독한 언론사에 추가되었습니다."라는 스낵바가 나오게 한다.
- [x] : 내가 구독한 언론사에 추가되도록 한다.
- [ ] : 내가 구독한 언론사에서는 해지하기 버튼이 보이도록 한다.
- [ ] : 해지하기 클릭 시 내가 구독한 리스트에서 제거한다.
</details>


<details>
<summary>뉴스 스탠드 설계도 (현상황)</summary>
 </br>
<img width="912" alt="image" src="https://user-images.githubusercontent.com/109648042/234071829-aed46f60-e9e3-44eb-b8b3-6ba64dfb876e.png">
</details>

<테스트 코드>
- [x] : Jest 셋팅
- [ ] : Unit Testing 

<기술 블로그>
[리펙토링과 테스트코드](https://velog.io/@sarang_daddy/JS-%EB%A6%AC%ED%8E%99%ED%86%A0%EB%A7%81%EA%B3%BC-%ED%85%8C%EC%8A%A4%ED%8A%B8%EC%BD%94%EB%93%9C)
[Jest](https://velog.io/@sarang_daddy/JS-%ED%85%8C%EC%8A%A4%ED%8A%B8%EC%BD%94%EB%93%9C-Jest#toequal-tostrictequal)

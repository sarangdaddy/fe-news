# 네이버 뉴스 스탠드 클론 - 개인 프로젝트

## 🛠️ 기술 스택

- HTML, CSS, JavaScript

## 🎯 학습 목표

- 웹 컴포넌트 디자인 및 구현에 대한 학습
- Vanilla JS를 이용한 동적 UI 구성 및 이벤트 관리
- Observer 패턴을 이용한 상태 관리 및 UI 업데이트 로직 구현
- Vanilla JS로 캐러셸 기능 구현

## 📘 프로젝트 설명

- 이 프로젝트는 네이버 뉴스 스탠드의 기본 UI 및 기능을 클론하여 만든 웹 페이지입니다.
- Observer 패턴을 활용하여 상태 관리 로직을 구현하였고, 이를 기반으로 사용자의 인터랙션에 따라 동적으로 UI가 업데이트됩니다.

### 주요 구성 요소 및 설명

<img src="https://user-images.githubusercontent.com/109648042/234071829-aed46f60-e9e3-44eb-b8b3-6ba64dfb876e.png" width="50%">

1. JournalListView 컴포넌트

- 기능 : 각각의 저널 view 컴포넌트를 적절하게 관리 및 렌더링합니다.

2. View 컴포넌트

- 종류 : Journal, JournalHeader, JournalTrack
- 기능 :
  - UI를 동적으로 렌더링합니다.
  - 상태 변경을 위해 발생하는 이벤트를 Store에 전달합니다.
  - Store의 상태 변화를 구독하여 UI를 업데이트합니다.

3. Store (상태 관리)

- 종류 : JournalDetailStore, JournalHeaderStore, JournalTrackStore
- 기능 :
  - 애플리케이션 상태를 중앙에서 관리합니다.
  - 상태 변화를 구독하는 View 컴포넌트에게 상태 변화를 통지합니다.

4. Event Handling

- 기능 :
  - View 컴포넌트에서 발생하는 이벤트를 핸들링합니다.
  - 예 : Journal 컴포넌트에서 발생하는 구독/해지 이벤트를 핸들링하여 JournalHeaderStore의 상태를 업데이트합니다.

### 작동 흐름

<img src="https://velog.velcdn.com/images/sarang_daddy/post/305128a2-8c2c-4c21-8f9b-5a9a40e0757b/image.png" width="50%">

1. 상태 초기화 및 렌더링

- 각 Store는 초기 상태를 가지고 있으며, 이를 기반으로 View(UI) 컴포넌트를 렌더링합니다.

2. 이벤트 발생

- 사용자의 인터랙션(버튼 클릭 등)에 의해 이벤트가 발생하면, 이벤트 핸들러가 해당 이벤트를 처리합니다.

3. 상태 변경

- 이벤트 핸들러는 발생한 이벤트에 따라 관련 Store의 상태를 업데이트합니다.

4. View(UI) 업데이트

- 상태가 변경되면, Store는 이를 구독하고 있는 View 컴포넌트에게 알립니다. (옵저버 패턴)
- 구독하고 있는 View 컴포넌트는 새로운 상태를 받아 UI를 업데이트합니다.

## 🚀 구현 결과

![](https://velog.velcdn.com/images/sarang_daddy/post/3cb317ef-22fd-4100-b623-4e147b69955d/image.gif)

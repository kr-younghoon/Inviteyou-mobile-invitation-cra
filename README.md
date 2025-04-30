## 📨 Inviteyou 프로젝트 개요
**축복과 초대를 담은 모바일 초대장 웹 애플리케이션**  
**개발 및 운영 기간: 2023/09/28 ~ 2023/10/05**


<br>

## 🚀 핵심 기능 - 모바일 초대 폼
> 사용자의 입력을 바탕으로, **축복 메시지와 말씀 카드**를 만들어 지인에게 전달하는 **8단계 초대 폼** 제공

- **관계 기반 초대 메세지 생성**: 친구, 가족, 직장 동료 등 관계 설정에 따라 맞춤 초대장 작성
- **축복 키워드 선택 + 랜덤 성경 말씀**: 선택 키워드에 따라 AI가 추천한 말씀 카드 추첨
- **말씀 카드 뷰**: 애니메이션 기반으로 말씀이 펼쳐지는 Lottie 효과 적용
- **이미지 저장 기능**: 완성된 축복 메시지와 말씀 카드를 이미지로 저장 가능 (html-to-image)

<br>

## ✨ 문제 해결 - 초대 효율 & 의미 강화
### [1️⃣ 단계형 폼 UI로 이탈 최소화](#)
직관적인 단계 진행 방식(총 8단계)을 통해 사용자의 입력 몰입도를 향상시키고, 초대장 작성 경험을 향상시켰습니다.

### [2️⃣ 무작위 말씀 추첨으로 신앙적 메시지 강화](#)
축복 키워드에 따른 랜덤 말씀 제공으로 초대장에 영적 의미를 부여함과 동시에, 매번 다른 카드로 **재방문 동기 유도**

<br>

## 🚀 핵심 기능 - 방문 정보 안내 및 후기
> 초대장을 받은 사용자가 **행사 정보를 확인하고**, **후기 메시지를 남기는 경험 제공**

- **시간/장소 안내**: 시간대별 프로그램 나열 + Google Maps 연동 지도 안내
- **방문 후기 (방명록)**: 이름과 한 줄 메시지를 입력하여 댓글처럼 남김
- **실시간 업데이트**: Firestore의 onSnapshot을 통해 댓글 실시간 반영

<br>

## ✨ 문제 해결 - 행사 공유 & 피드백
### [1️⃣ Google 지도 연동으로 길찾기 문제 해결](#)
정확한 행사 장소 시각화를 통해 지인 초대시 동선 안내 편의성 확보

### [2️⃣ 후기 작성 기능으로 반응 수집](#)
단순 초대를 넘어 **쌍방향 피드백 공간** 마련 → 방문자 반응, 감사 인사, 느낌 등을 실시간 수집 가능

<br>

## 🌐 서비스 흐름도
1. 사용자가 초대장 웹앱 접속 → 다단계 폼 입력
2. 축복 메시지/말씀 카드 생성 후 저장 or 공유
3. 행사 정보 페이지에서 위치 및 일정 확인
4. 방문 후 방명록에 댓글 작성

<br>

## 🧩 프로젝트 아키텍처
Firebase Hosting 기반 무서버 구조이며, 모든 로직은 프론트엔드 + Firestore DB로 구현됨

- CRA 기반 React SPA
- Firebase Firestore + Storage 사용
- 실시간 동기화: onSnapshot
- 배포: Firebase Hosting

<br>

## 🚀 기술 스택
<markdown-accessiblity-table data-catalyst=""><table>
  <tbody>
    <tr>
      <td align="center" width="160px">FrontEnd</td>
      <td align="center" width="560px">
        <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/CSS Module-264de4?style=for-the-badge&logo=css3&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/React Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white" height="24px"/>
      </td>
    </tr>
    <tr>
      <td align="center">BaaS</td>
      <td align="center">
        <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/Firestore-FFA000?style=for-the-badge&logo=firebase&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/Storage-3367D6?style=for-the-badge&logo=googlecloud&logoColor=white" height="24px"/>
      </td>
    </tr>
    <tr>
      <td align="center">Deploy</td>
      <td align="center">
        <img src="https://img.shields.io/badge/Firebase Hosting-FFCA28?style=for-the-badge&logo=firebase&logoColor=white" height="24px"/>
      </td>
    </tr>
    <tr>
      <td align="center">Library</td>
      <td align="center">
        <img src="https://img.shields.io/badge/html--to--image-009688?style=for-the-badge&logo=data:image/svg+xml;base64,&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/lottie--react-00BCD4?style=for-the-badge&logo=lottiefiles&logoColor=white" height="24px"/>
        <img src="https://img.shields.io/badge/react--google--maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white" height="24px"/>
      </td>
    </tr>
  </tbody>
</table></markdown-accessiblity-table>

<br>

## 👨‍👨‍👧‍👦 팀원 구성
| 이름   | 역할       | GitHub                                       |
| ------ | ---------- | -------------------------------------------- |
| 이영훈 | FrontEnd   | [GitHub](https://github.com/kr-younghoon)    |
| 김현아    | Design     | 비공개                                      |

<br>

## 🧩 역할 분담
| 이름   | 담당 영역                                              |
| ------ | ------------------------------------------------------ |
| 이영훈 | 전체 구조 설계, 초대장 폼/방명록/지도 기능 개발, Firebase 연동 |
| 김현아    | 디자인 전반, Lottie 애니메이션, 반응형 UI 구성               |

<br>

## 📌 주요 기능
1. **초대장 작성 (8단계 폼)**  
   - 이름/관계 입력 → 축복 키워드 선택 → 말씀 카드 추첨 → 메시지 완성

2. **말씀 카드 생성**  
   - 키워드 기반 랜덤 성경 말씀 제공 (JSON 카드 DB 기반)
   - 애니메이션 효과 (Lottie 사용)

3. **행사 정보 안내**  
   - 시간별 일정 나열
   - Google Maps 위치 삽입

4. **방명록 작성 및 조회**  
   - 이름/후기 입력 → Firestore 실시간 저장
   - onSnapshot을 통한 실시간 갱신

5. **이미지 저장**
   - 완성된 초대 메시지 + 말씀 카드 이미지로 저장 (html-to-image)

<br>

## 🗂 데이터 구조 (Firestore)
- **comments 컬렉션**: 방명록 메시지 저장
  - 필드: writtenBy, text, timestamp
- **invites 컬렉션**: 초대 메시지 저장
  - 필드: inviterName, relationship, tag, verse, userName
- **users 컬렉션 (예정)**: 관리자 여부 판단용 (isAdmin)

> 모든 컬렉션은 Firestore 보안 규칙에 따라 읽기 허용, 쓰기는 제한

<br>

## 🔗 배포 주소
Firebase Hosting 기반 (행사 종료 후 비공개 처리됨)

```
https://side-project-ayoung.web.app
```

> 본 프로젝트는 교회 행사를 위해 제작된 비영리 목적으로 개발되었으며,
> 향후 청첩장/초대장 플랫폼으로 확장될 수 있는 기반 구조를 실험하였습니다.


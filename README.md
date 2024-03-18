# <p align="center">✨ L O A S ✨</p>
<p align="center">
<img width="99%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/1819b6f3-b6ad-4abb-b351-f5be432e63e5">
<br>
<br>
<img width="35%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/5e386e71-63a7-4a96-9570-274c7614cf82"/>

#### <p align="center">LOAS (LostArk States) 는 SmileGate RPG 사의 Lost Ark Open API Developer Program 을 이용하여 만든<br>MMORPG 게임 LostArk 컨텐츠 정보 검색 애플리케이션입니다.<br></br></p>


<p>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/37f0bbc0-2784-47f7-b291-26839669f554"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/7340a696-ccb3-4107-93b3-f426d5fb5593"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/19ac0d1b-1124-47b1-9c58-021abcbb50ac"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/88425c92-e45d-4992-acf9-caefd96d3be2"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/81436fe0-1f3b-4498-8a1a-8ea9892e5a2c"/>
</p>


## 프로젝트 기간 🎀 
2023.09.23 ~ 2023.10.25

## 프로젝트 구분 🎀
1인 개발 애플 앱스토어 출시 프로젝트

## Open API 에 대한 기여 🎊
앱 구현 중 API 에서 받을 수 있는 '각인' 이라는 항목의 아이콘이 캐릭터 스펙 대비 부족한 사항에 대하여 API 디벨로퍼팀 측으로 아이콘 에셋을 확보 할 수 있는 방법에 대하여 문의하였습니다.
그 결과 디벨로퍼팀 측에서 캐릭터 스팩대로 '각인 아이콘' 을 배포하는것으로 API 를 업데이트 하였습니다.
 
## Main Features ✨
- 대표 캐릭터 지정 및 변경
- 캐릭터 검색
- 캐릭터 상세 스팩 조회 (능력치, 아이템 스펙, 스킬, 수집포인트, 해당 캐릭터 계정 내 보유 캐릭터)
- 관심 캐릭터 등록
- 현재 진행중인 로스트아크 이벤트, 공지사항 조회
- 주간 컨텐츠 캘린더 (프로키온의 나침반)
- 주간 컨텐츠 일정 및 보상 조회 (도전 어비스 던전, 도전 가디언 토벌)
- 인게임 아이템 거래소에서 아이템 시세조회

## Sub Features 🌙
- LOAS 개발자 1:1 카카오톡 오픈채팅 연결
- 마이너 버전 업데이트 시 강제 업데이트 요청 기능
- 패치 버전 업데이트 시 사이드메뉴에서 업데이트 가능여부 표시

## Tech Stacks 🛠
- CodeBase UIKit, MVVM Architecture
- RxSwift, RxKeyboard (업데이트 포함)
- Custom Observable
- Alamofire
- Realm Swift
- Kingfisher
- SnapKit
- SideMenu
- Toast
- PanModal
- Compositional Layout, URLRequestConvertible, UISheetPresentationController

## 주요 기술 🌖
- 캐릭터가 달성한 컨텐츠에 따라 다른 유동적인 API 의 HTML 마크다운 응답값에 대응하도록 다이나믹하게 파싱 가능한 모델을 개발하여 로스트아크의 모든 캐릭터 스팩을 보여 줄 수 있도록 기능을 구현하였습니다. 또 이후 게임 컨텐츠 업데이트로 인해 새로운 능력치가 등장 할 경우 유지 보수가 용이하도록 하였습니다.
- Realm Swift를 사용하여 자신이 원하는 캐릭터를 메인 화면에 지정 또는 이후 다른 캐릭터로 변경 할 수 있고 최근 검색한 캐릭터의 히스토리, 관심 캐릭터를 등록하는 기능을 구현하였습니다.
- Kingfisher 를 사용하여 이미지 캐싱과 로드를 간편하게 구현하였습니다.
- ScollView 와 Collection View 를 조합하여 Tab 기능을 구현하여 각각의 정보를 Grouping 였습니다.
- 많은 페이지에서 Compositional Layout 을 구현 시 반복되는 코드를 피하기 위하여 필요한 메서드들을 확장으로 구현해 코드의 중복을 최소화 하였습니다.
- DispatchGroup 을 사용하여 데이터의 로드가 완료 된 이후 안정적으로 화면을 표시 할 수 있도록 하였습니다.
- 추후 API 업데이트에 대응 할 수 있도록 Alamofire 의 URLRequestConvertible 을 사용하여 Network Router 를 추상화 하였습니다.
- 메이저, 마이너, 패치 업데이트에 대해 강제업데이트 또는 선택적 업데이트 기능을 구현하였습니다.
- 강제 업데이트가 필요한 경우 앱이 실행 될 때 SceneDelegate 에서 업데이트 가능 여부를 판단하고 Alert 을 노출해 앱스토어로 유도 하였습니다.
- 디바이스 가로 너비 812 해상도 이하의 작은 화면에 대한 대응처리로 낮은 해상도의 디바이스에서도 자연스러운 UI가 표현 될 수 있도록 하였습니다.

## 개발시 고려 사항 💎

1. 메인 페이지
<p>
<img width="22%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/3b7d3036-e465-4f3d-8cac-c1b8ae7f1d9d"/>
<img width="22%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/357282d4-282c-4233-bfbb-f2ebc2353acd"/>
<img width="22%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/424baef9-ba7f-4b0a-9d2c-df736bb4cda6"/>
<img width="22%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/9490c504-f3af-4ea7-985b-8754322065f1"/>
</p>

- 앱을 처음 설치 했을 때 Realm 에 저장된 대표 캐릭터가 존재하지 않을 경우 대표 캐릭터를 등록하도록 유도하는 셀을 표시하고 캐릭터 이미지 노출영역을 축소하는 로직을 구현했습니다.
- 공지사항에 대한 응답 속성 중 '점검', '공지사항', '상점' 항목을 분리시켜 유저 편의성을 높였습니다.
- 각각의 공지사항을 터치 하면 로스트아크 공식 홈페이지의 해당 WebView 를 통해 공지 페이지로 연결 되도록 하였습니다.
- 점검, 공지사항, Shop 의 헤더에 더보기 아이콘을 터치하면 로스트아크 공식 홈페이지의 최근 공지사항을 항목별 로 모아서 볼 수 있도록 하였습니다.
- 메인 뷰컨트롤러를 싱글톤으로 구성해 앱이 메모리에서 내려가지 않는 한 로딩된 정보는 API 서버에 다시 요청하지 않도록 하고 실시간으로 게임 컨텐츠의 변화가 일어나지 않으므로 Pull to Refresh 기능은 구현하지 않았습니다.
- 각 섹션의 데이터가 비동기로 로드 될 때마다 컬렉션뷰가 리로드되어 화면이 깜빡이는 현상을 방지하기 위해 DispatchGroup 을 사용해 데이터의 로드가 완료 된 이후 Compositional Layout 의 메서드가 동작하도록 로직을 구현하였습니다.

2. 사이드메뉴
<img width="20%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/191aeab5-3e73-4814-b03c-dfe686ca1549"/>

- 좀더 손쉽게 부가 메뉴에 접근하기 위하여 사이드메뉴를 사용했습니다.
- 사이드메뉴의 호출은 네비게이션 영역의 아이콘 터치 또는 오른쪽 스와이프 제스처를 사용했습니다.
- 최신 업데이트 가능 여부를 알 수 있도록 최하단에 부가 메뉴를 배치했습니다.

3. 캐릭터 상세정보
<p>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/be49f6c2-723c-4ff6-aac9-4fcbe0210141"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/eb775656-c528-4368-8d9f-2967d99af8de"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/152b18d0-49fb-4760-b610-2d83260dd4c4"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/141a2220-a8e1-4593-9703-e98938fd18cb"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/7ea1fd53-82a7-482c-abff-5ea625529c16"/>
<br>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/10c15073-de33-4c0d-9827-bd02a19820fb"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/afd26f7d-7916-413a-a75a-3d8bffd79387"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/b9a0d121-4d6b-4e0c-b939-9dc67d4c332c"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/b745c24f-49e1-43bf-8cd2-a5f9314a1f84"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/794adb1b-a7aa-44cd-a80a-c7d907d63e3c"/>
</p>

- 11개의 섹션으로 구성된 캐릭터 상세정보페이지는 캐릭터 스펙에 따라서 접근하는 엔드포인트의 수가 다릅니다. 따라서 상황에 맞게 추가 네트워크 통신을 하고 DispatchGroup 을 사용해 모든 로직이 완료 된 후 컬렉션뷰의 레이아웃을 설정하는 메서드가 동작하도록 하였습니다.
- 각 뷰의 인스턴스를 생성할 때 현재 ViewModel 을 의존성으로 주입하여 생성하였고 ScrollView 컨테이너 안에 각 뷰를 가로로 배치하여 페이징 효과를 구현했습니다. 다만 현재 기능 내에서 횡스크롤이 필요한 섹션이 존재하므로 애플 휴먼인터페이스 가이드라인에서 권장하는 사항에 따라 가로 스와이프로 다른 탭으로 이동하는것은 막았습니다.
- 기본정보 탭의 '장비' 섹션에서 아이템의 부가 옵션을 표시하고 있습니다. 이 옵션들은 API 응답자체가 단순히 파싱 할 수 없는 장문의 JSON 으로 구성되어 있고 컨텐츠 달성도에 따라서 30가지가 넘는 JSON 형식을 가집니다. 따라서 캐릭터 구간별 컨텐츠와 응답을 전부 분석하여 모든 패턴을 구조화 하는 것으로 Decoding 하는 Engine 이 다이나믹하게 Decode 할 수 있도록 LOAS 의 핵심 기능을 구현 하였습니다.
- 기본정보 탭의 '장비' 섹션에서 장착한 아이템을 터치 하면 바텀시트를 통해 상세정보가 올라옵니다. 이 부분은 HTML 마크다운 형식으로 되어있는 응답값을 NSAttributedString을 사용해 표시하였습니다.
- 기본정보 탭의 '장비' 섹션에서 장신구 아이템의 옵션의 API 응답도 HTML 마크다운 언어로 되어있었기 때문에 정규식을 통해 원하는 String 을 추출하여 셀에 표현하였습니다.
- 캐릭터 컨텐츠 달성 스팩에 따라 부가 옵션의 노출 여부가 결정되도록 로직을 구현하였습니다.
- 화면이 아래로 스크롤 될 때 메인화면으로 돌아 갈 수 있는 Tab 영역이 숨겨지도록 하여 화면에 표시되는 컨텐츠의 양을 SuperView 영역까지 확대 되도록 구현하였습니다.
- 캐릭터의 외형을 최상단에 배치하고 기본정보를 오버레이 하는 방식으로 일반 스팩을 확인 할 수 있도록 하였습니다.
- 캐릭터 스테이터스 세가지를 별도의 섹션으로 구분해서 능력치 정보를 한눈에 알 수 있도록 하였습니다.
- 캐릭터 레벨별 달성한 컨텐츠 능력치를 아이템 아이콘과 적절히 배치하여 현재 캐릭터가 어떤 능력을 가지고 있는지 알 수 있도록 하였습니다.
- 장착한 보석 또는 장착한 아바타의 섹션 헤더의 더보기 아이콘을 터치하면 현재 장착한 아이템의 세부 정보와 능력치가 바텀시트를 통해 올라오도록 하였습니다.
- 스킬 탭의 경우 현재 장착한 스킬 이름과 스킬레벨, 부가옵션(트라이포드), 장착한 룬의 옵션과 효과를 나타내도록 하였고 정규식을 사용해 필요한 String 에 컬러를 추가했습니다.
- 수집형 포인트의 달성도를 퍼센테이지로 나타냈으며 각각의 아이콘을 터치하면 바텀시트에서 목록이 등장하고 수집한 아이템의 경우 화이트 컬러로 구분감을 추가했습니다.
- 보유 캐릭터의 탭을 터치하면 해당 계정 내 모든 서버의 모든 캐릭터가 리스팅됩니다. 모티브는 영화의 마지막 엔딩 크레딧에서 얻었으며 캐릭터명을 터치하면 해당 캐릭터를 즉시 검색합니다.
- 네비게이션 영역의 우측 상단의 하트 아이콘을 터치하면 관심 캐릭터로 등록되며 메인화면의 네비게이션 영역의 동일한 아이콘에서 관심 캐릭터를 모아서 볼 수 있습니다.

4. 거래소
<p>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/b3ee4b6d-45d8-44dd-aa76-c4fe7ef0c519"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/fa00f19c-8b07-4a9a-b6fe-a63c5e672043"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/924edd29-7d48-4e27-b5aa-a93023b90564"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/20bd51e4-e6bd-4c38-a990-87e4bf848b38"/>
<img width="19%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/f8b5946a-6da1-41d1-bfee-681914486484"/>
</p>

- 1.4.0 에서 업데이트 된 거래소는 RxSwift 를 사용하였습니다.
- 엔드포인트에서 검색 옵션을 불러오는동안 UIActivityIndicatorView 가 노출되도록 하였습니다.
- 리퀘스트 요청사항에 맞추어 카테고리를 설정하지 않을 경우 토스트 메시지가 출력되도록 하였습니다.
- 각 섹션을 터치하면 검색 할 조건을 선택 할 수 있는 바텀시트가 등장하도록 구현하였습니다.
- 지금까지 바텀시트를 구현 할 때 PanModal 라이브러리를 사용했는데 오래 된 라이브러리이기 때문에 UISheetPresentationController 를 사용하였고 이후 업데이트에서 UISheetPresentationController 를 커스텀하여 다른 뷰의 PanModal 을 제거 할 예정입니다.
- 검색 결과 화면에서 tableView.rx.prefetchRows 를 사용해 Pagination 기능을 구현하였고 API 응답이 느릴 경우 대기시간동안 UIActivityIndicatorView 가 노출되도록 하였습니다.
- API 응답에서 검색된 아이템의 수가 표시된 아이템의 수보다 많은 경우에만 Pagination 기능이 동작하도록 조건을 설정하여 불필요한 엑세스를 방지했습니다.

## Trouble Shooting 🎀
### 1. 선택적인 비동기 데이터 로드와 컬렉션뷰의 리로드 시점
#### Trouble: 다른 엔드포인트의 작업이 완료되지 않았을 때 컬렉션뷰의 레이아웃이 설정되면 데이터가 로드중인 섹션이 캐릭터의 스팩정보를 확인 할 수 없는 셀을 보여주는 현상.
- 데이터가 로드되는 시간동안 캐릭터 스팩 정보가 없어 에러 대응시 보여주는 셀이 노출되었습니다.
- 캐릭터 상세 정보 응답을 받고 필요에 따라 추가 비동기 통신중에 데이터가 전부 완료된것으로 처리되어 원하는 데이터를 화면에 표시 할 수 없거나 out of range 런타임 오류가 발생했습니다.

<img width="50%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/7882de39-6f2b-47a8-932b-24622ba8c164"/>

#### Solution: DispatchGroup 을 사용하여 모든 데이터의 로딩이 완료된 이후 CollectionView 레이아웃 실행
- DispatchGroup 으로 각인 상세 정보에 대한 비동기 통신이 완료된 이후 group.notify 블록에서 completionHandler 를 통해 컬렉션뷰의 레이아웃을 잡을 수 있도록 했습니다.
- 그 결과 장기간 미접속으로 인해 캐릭터 외형이 API에 업데이트 되지 않거나 실제로 캐릭터가 장비를 장착하지 않아서 존재하지 않는 데이터에 대해 훨씬 깔끔하게 대응 할 수 있도록 하였습니다.

### 2. Apple 정책에 따른 업데이트 거절에 대한 대응
#### Trouble: 로스트아크 이벤트 중 '룰렛' 일러스트가 포함된 이미지가 앱 내 노출되어 앱스토어 정책에 위배되는 사유로 업데이트가 거절됨
- 리뷰어에 의해 처음 업데이트 심사가 거절 되었을 때 '룰렛 이벤트'가 현금으로 참여하는것이 아니고 사행성(겜블)과 관련이 없다는 소명을 했음에도 불구하고 다시 업데이트가 거절 되었습니다.

<img width="50%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/3130672c-66d7-4cdf-b8a2-d584068cdc18"/>

#### Solution: 엔드포인트 응답에서 타이틀이 '룰렛' 이라는 단어가 포함된 이벤트 필터링
- 다행이도 엔드포인트의 응답 중 타이블에 이벤트 이름이 포함되어 있어 '룰렛' 이라는 단어가 들어간 이벤트 배너를 노출시키지 않는것으로 애플 앱스토어의 규정을 준수하였습니다.
- 유저 입장에서 해당 이벤트가 보이지 않아 불편 할 수 있겠지만 웹뷰를 통해 앱 내에서 룰렛 이벤트를 확인 할 수 있으므로 큰 지장은 아니라고 판단했습니다.


## 아쉬웠던점
- 바텀 모달 시트를 구현하는데 어려움이 있어서 앱 개발 초기부터 PanModal 이라는 오래된 라이브러리를 사용했습니다. 일단 작동은 하기에 출시 당시까지 문제는 없었으나 지원이 끊긴 라이브러리는 언젠가 문제가 될 수 있기에 업데이트의 필요성을 느끼며 출시를 진행했었습니다. 이후 경매장 업데이트를 하면서 UISheetPresentationController 의 커스텀 방법을 알게 되어 다음 업데이트 때 보다 안정적인 앱 서비스를 도모할 예정입니다.
- Rx 를 다루기 이전에 진행한 프로젝트로 Custom Observable 패턴을 사용했습니다. 셀을 바인딩 하면서 비동기 처리에 어려움이 발생해 Dispatch Group 을 사용하여 해결은 했지만 이후 API 업데이트에 대응하기 어려울 수 있다는 잠재성을 느꼈고 순차적으로 뷰마다 Rx로 리팩토링을 진행하는것으로 코드를 안정화 하려고 합니다.
- 정규식을 학습하는데 많은 어려움이 있었습니다. JSON 이 HTML 마크다운 언어로 오는 응답값 속에서 원하는 데이터를 추출하기 위해 긴 시간이 소비되는 바람에 제가 바라는 앱의 다른 디테일을 챙기지 못한 부분이 많이 아쉽습니다만 먼저 구현은 되어있기에 업데이트를 통해 캐릭터가 착용하고 있는 의상(아바타) 의 상세 정보를 좀더 구체적으로 유저들에게 제공 하려고 합니다.

## 회고 & Future Action

<img width="99%" src="https://github.com/UNICUS-FORTIS/LOAS-Readme/assets/110699030/2b5fc035-8dbc-4968-8f1d-3772292e7015"/>

- 2023년 10월 25일 출시부터 2024년 3월 16일 기준으로 앱 노출 수 4.5만, 페이지 조회수 3200건, 컨버전률 1.82%, 전체 다운로드 수 574 건의 LOAS 는 제 첫 출시 프로젝트로 제가 너무나도 좋아하는 게임과 관련된 앱을 출시함으로서 현재까지 약 10건의 업데이트를 진행했습니다.
- 협업 프로젝트 플랫폼 '렛플' 의 운영자께서 앱 내 1:1 문의를 통해 LOAS 의 소개를 메인 페이지에 게시해주셨고 많은 분들의 긍정적인 피드백을 얻을 수 있었습니다.
- 부산에서 열린 게임 페스티벌 2023 G-Star 기간에는 하루동안 앱 페이지 조회수 3천여건을 기록하며 로스트아크 IP 의 파급력을 체감 할 수 있었고 그것은 제가 앱을 더 발전시키려는 동기가 되었습니다.
- 기술적으로 많이 부족한 상태에서 진행한 프로젝트로 커스텀 옵저버블 패턴을 사용하면서 데이터를 바인딩하는데 많은 어려움을 겪으며 조금씩 성장 할 수 있었고 UI 제작과 앱 출시, 업데이트, 업데이트거절과 같은 출시와 관련된 경험들을 할 수 있었습니다.
- 현재까지는 게임서버점검, API 서버점검과 같은 500번대 에러에 대해서만 핸들링 하고 있습니다만 개발 당시 에러 처리에 대한 미숙함을 지울수가 없었습니다. 이후 게임 컨텐츠의 변화로 API가 업데이트 될 때 앱 업데이트 대응 속도가 느릴 경우를 대비해 앱 클라이언트에서 발생 할 수 있는 에러에 대하여 선제적으로 대응 할 예정입니다.
- 최초 기획안에서는 데이터가 로드되는동안 스켈레톤뷰를 보여주는것을 목표로 하고 있었지만 예상치 못한 변수들에 의해 핵심 기능을 위한 시간이 많이 소요되었습니다. 이 또한 업데이트에서 대응하면서 전체적인 코드를 Rx로 대응하고자 합니다.
- LOAS 를 개발하면서 커밋을 어떤 단위로 해야 할지 모르고 있었습니다. 파일단위, 피처단위, 업데이트단위 이런 컨벤션 없이 말그대로 '저장소' 용도로 원격 레파지토리에 업로드하고 있었던 부분이 다소 후회스럽습니다. Chatify 를 개발하면서도 너무 작은 단위의 커밋에 대해 회고했습니다만 커밋의 컨벤션을 좀더 체계적으로 관리하고 실행할 계획입니다.

## Scene & Interactions ⚡

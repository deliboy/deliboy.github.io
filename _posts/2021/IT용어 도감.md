---
layout: post
title:  "asp.net core graphql with hotchocolate #1"
date:   2021-10-01T11:26:00+09:00
category: book
tags:	[book]
background:  "/img/bg/01.jpg"
---
## 목차
### 제1장 뉴스를 쉽게 이해하는 IT 용어

- [인공지능(AI) | 인간과 같이 현명한 동작을 하는 컴퓨터](https://www.netapp.com/ko/artificial-intelligence/what-is-artificial-intelligence/)
> 인공 지능(AI)은 동적 컴퓨팅 환경에 내장된 알고리즘을 생성하고 적용하여 인간의 지능을 모방하는 기초 지능입니다. 간단히 말해서 AI는 인간처럼 사고하고 행동하는 컴퓨터를 만들려고 합니다.
> 이 목표를 달성하려면 세 가지 핵심 구성 요소가 필요합니다.
> 1. 계산 시스템
> 1. 데이터와 데이터 관리
> 1. 고급 AI 알고리즘(코드)

- [RPA | 사무 처리 업무를 자동화한다](https://www.redhat.com/ko/topics/automation/what-is-robotic-process-automation)
> RPA(로봇 프로세스 자동화)는 이전에는 사람이 하던 반복적인 태스크를 소프트웨어 로봇이 대신하는 것입니다.

> 대부분의 RPA 툴은 개별 워크스테이션에서 실행되며 학습을 통해 데이터베이스에서 스프레드시트로 데이터 행을 옮기는 것과 같은 반복 태스크를 수행합니다. 개별 봇이 엄청난 양의 단순 태스크를 부지런히 처리하는 동안 기업의 이익이 쌓여 갑니다. RPA는 광범위한 BPM(비즈니스 프로세스 관리) 전략에 따라 조직의 운영 효율성을 높이는 데 중요한 역할을 할 수 있습니다.

- [IoT | 사물인터넷](https://www.sas.com/ko_kr/insights/big-data/internet-of-things.html)
> IoT란, 인터넷에 연결되어 IoT 애플리케이션이나 네트워크에 연결된 장치, 또는 산업 장비 등의 다른 사물들과 데이터를 공유할 수 있는 수많은 '사물'을 말합니다.

- [빅데이터 | 기록이나 보관, 해석이 어려운 거대 데이터](https://www.redhat.com/ko/topics/big-data)
> 빅데이터는 전통적인 데이터 프로세싱 방법으로 처리할 수 없을 정도로 대규모이거나 복잡한 데이터입니다. 빅데이터는 흔히 'Three V'로 불리는 볼륨(Volume), 다양성(Variety), 속도(Velocity)라는 특성을 가지고 있습니다. 볼륨은 대규모 크기를 의미하며, 다양성은 비표준 형식의 광범위한 범위를 그리고 속도는 신속하고 효율적으로 처리되어야 하는 특성을 의미합니다.

- [핀테크 | IT와 금융의 융합](https://www.banksalad.com/contents/%ED%95%80%ED%85%8C%ED%81%AC-%EA%B0%9C%EB%85%90-%EC%99%84%EB%B2%BD-%EC%A0%95%EB%A6%AC-9752)
> 핀테크란 금융에 IT를 접목하여 복잡하고 어려웠던 금융을 효율적으로 편리하게 서비스하는 것을 뜻합니다. 10년 전부터 사용하던 온라인 뱅킹도 일종의 '핀테크'라고 할 수 있죠.

- [블록체인 | 거래 데이터를 통합하는 기술](https://www.ibm.com/kr-ko/topics/what-is-blockchain)
> 블록체인은 비즈니스 네트워크에서 트랜잭션을 기록하고 자산을 추적하는 프로세스를 효율화하는 불변의 공유 원장입니다. 자산은 유형 자산(주택, 자동차, 현금, 토지) 또는 무형 자산(지적 재산권, 특허, 저작권, 브랜드)일 수 있습니다. 사실상 가치를 지닌 모든 것들이 블록체인 네트워크 상에서 추적되고 거래됨으로써, 연루된 모든 것들에 대한 리스크를 줄이고 비용을 절감할 수 있습니다.

- [가상화폐 | 국가가 관리하지 않는 암호 기술을 이용한 통화](https://namu.wiki/w/%EA%B0%80%EC%83%81%20%ED%99%94%ED%8F%90)
- 드론 | 원격 조작할 수 있는 무인 항공기
- 셰어링 이코노미 | 타인과 공유·교환하며 이용한다
- 애자일과 워터폴 | 사양의 변경을 전제로 개발한다

- [기술적 특이점 | 인공지능이 인류를 뛰어넘는다](https://m.etnews.com/20150403000059)
> 강력한 인공지능이나 인간 지능증폭이 가능했을 때 출현하는 시점이다.

- [VR, AR, MR | 현실과 가상세계의 융합](https://www.intel.co.kr/content/www/kr/ko/tech-tips-and-tricks/virtual-reality-vs-augmented-reality.html)
> 1. **가상 현실**
VR은 이러한 기술에서 가장 대표적입니다. 완전히 몰입하도록 만들어져 있으며, 실제와는 다르거나 동떨어진 세계에 있다고 생각하도록 감각을 속이는 것입니다. 헤드 마운트 디스플레이(HMD) 또는 헤드셋을 사용하여 컴퓨터가 만든 상상의 세계와 사운드를 체험하며 콘솔이나 PC에 연결된 상태로 물건을 조작하거나 촉각을 사용하는 컨트롤러로 움직일 수 있습니다.
> 2. **증강 현실**
AR은 실제 요소에 디지털 정보를 오버레이합니다. Pokémon GO*가 가장 잘 알려진 사례입니다. 증강 현실은 실제 현실을 바탕으로 하여, 다른 디지털 세부 사항으로 현실을 강화하면서 새로운 인지 계층을 만들고 현실이나 환경을 보완합니다.
>3. **혼합 현실**
MR은 현실과 디지털 요소를 함께 활용합니다. 혼합 현실에서는 차세대 센서 및 이미징 기술을 사용해 실제 물건과 환경, 가상의 물건과 환경을 모두 조작하고 이들과 상호 작용합니다. 혼합 현실에서는 손으로 가상 환경과 상호 작용하면서 헤드셋을 벗지 않은 상태로 주변을 보고 여기에 몰입할 수 있습니다. 한 손이나 한 발은 실제 환경에서, 다른 쪽은 가상의 공간에서 활동할 수 있기 때문에 현실과 가상의 기본적인 개념을 무너뜨리고 오늘날 게임과 업무 방식을 바꿀 수 있는 경험을 선사합니다.

- 롱테일 | 팔리지 않는 제품도 재고를 확보
- 머신러닝 | 인간이 룰을 가르치지 않아도 자동으로 학습
- 딥러닝 | 제3차 인공지능 붐의 주역
- POS | 점포의 매출을 분석한다
- [텔레워크 | 시간과 장소에 구애받지 않고 일하는 방식](https://www.kyongbuk.co.kr/news/articleView.html?idxno=2043479)
> 텔레워크란 멀리 떨어진 장소를 의미하는 ‘tele’과 일하다는 의미의 ‘work’가 결합된 합성어로 정보통신기술(ICT)을 활용하여 시간과 장소에 구애받지 않고 유연하게 일하는 방식이다
- [BYOD | 종업원의 스마트폰을 활용한다](https://www.itworld.co.kr/news/105962)
- [섀도 IT | 기업이 파악할 수 없는 종업원의 IT 활용](https://www.itworld.co.kr/news/105209)
> IT 부서에서 승인하지 않은 클라우드 애플리케이션이나 서비스를 구입하고, 이를IT 관리 부서나 책임자가 파악하지 못하는 현상을 가리켜 섀도우 IT(Shadow IT)라고 합니다
- QR 코드 | 2차원 바코드의 업계 표준
- 테더링과 로밍 | 스마트폰 통신 회선을 사용
- 베스트 에포트 | 통신 회선의 계약에 필수
- 스트리밍 | 다운로드하면서 재생할 수 있다
- 웨어러블 | 착용하고 사용하는 단말기
- 데이터 센터 | 몸에 데이터 관리에 특화한 건물
- [가상화 | 없는 것을 있는 것처럼 보이게 한다](https://www.redhat.com/ko/topics/virtualization/what-is-virtualization)
- [SCM | 복수 기업 간의 물류를 통합 관리](https://www.oracle.com/kr/scm/what-is-supply-chain-management/)
> SCM(Supply Chain Management)은 원자재 조달에서 마지막 단계인 제품 배송에 이르기까지 제품 또는 서비스와 관련된 상품, 데이터 및 재정의 흐름을 관리합니다.
- 시스템 인티그레이터 | 구축에서 운용까지 일괄로 맡는다
- 내부 통제 | 조직의 업무가 적정한지 체크
- [유니버설 디자인 | 누구나 사용할 수 있는 디자인](https://www.043w.or.kr/www/contents.do?key=151)
> 유니버셜디자인이란, ‘모든 사람들을 위한 디자인(DESIGN FOR PEOPLE)’이라고 하며, 연령과 성별, 국적(언어), 장애의 유무 등과 같은 개인의 능력과 개성의 차이와 관계없이 처음부터 누구에게나 공평하고 사용하기 편리한 제품, 건축ㆍ환경, 서비스 등의 구현 (디자인)을 의미합니다.
- 오픈 데이터 | 누구나 자유롭게 사용할 수 있는 데이터
- 메인 프레임 | 기간 시스템에 사용되는 대형 컴퓨터
- GPS | 위치 정보를 취득할 수 있다
- [오프쇼어 | 거점을 해외로 옮긴다](https://m.blog.naver.com/businessinsight/221016897485)


### 제2장 세트로 외우는 IT 용어

- [데이터 마이닝과 데이터 사이언스 | 대량의 데이터에서 새로운 지식을 발견](https://www.oracle.com/kr/data-science/what-is-data-science/)
> 데이터 사이언스는 통계, 과학적 방법, 인공지능(AI) 및 데이터 분석을 포함한 여러 분야를 결합하여 데이터에서 가치를 추출합니다. 데이터 사이언스를 실천하는 사람들을 데이터 사이언티스트라고 하며, 그들은 다양한 기술을 결합해 웹, 스마트폰, 고객, 센서 및 기타 소스에서 수집된 데이터를 분석하고 실행 가능한 통찰력을 도출합니다.
- 인터넷과 인트라넷 | 복수의 컴퓨터와 조직을 연결한다
- 패킷 통신과 회선 교환 | 안정된 통신을 실현한다
- ADSL과 광파이버 | 고속 네트워크
- WAN과 LAN | 네트워크의 범위를 나타낸다
- 프로토콜과 OSI 참조 모델 | 통신의 암호
- IP 어드레스와 포트 번호 | 네트워크의 장소를 나타내는 번호
- 도메인명과 DNS | 컴퓨터에 이름을 붙인다
- 루터와 스위치 | 네트워크의 경로를 결정한다
- 클라이언트 서버와 P2P | 컴퓨터의 역할 분담
- TCP와 UDP | 통신에 요구되는 신뢰성과 속도를 실현한다
- DHCP와 디폴트 게이트웨이 | 컴퓨터를 네트워크에 접속한다
- NAT와 NAPT | 여러 대의 컴퓨터를 같은 주소로 관리한다
- 패킷과 프레임 | 통신의 기본 단위
- 세션과 커넥션 | 접속 상황을 관리한다
- 도메인과 세그먼트 | 네트워크 영역을 식별한다
- CPU와 GPU | 컴퓨터의 두뇌
- 온프레미스와 클라우드 | 시스템 관리자를 바꿨다
- 파일과 확장자 | 애플리케이션과 링크한다
- 폴더와 디렉터리 | 파일을 관리한다
- 절대 경로와 상대 경로 | 파일의 장소를 나타낸다
- 가역 압축과 비가역 압축 | 파일의 용량을 줄인다
- VGA와 HDMI | 영상을 출력한다
- 문자 코드와 특수 문자 | 환경에 따라서 문자가 다르다
- 서체와 폰트 | 문장의 외관을 바꾼다
- 프런트 엔드와 백 엔드 | 시스템의 역할이 다르다
- 임포트와 익스포트 | 다른 소프트웨어와 데이터를 거래
- 아이콘과 픽토그램 | 한눈에 이해할 수 있는 표현
- [저작권과 크레에이티브 커먼즈 | 도작(盜作)을 방지한다](https://blog.naver.com/vegadora/220957918130)
- OS와 애플리케이션 | 소프트웨어의 역할이 다르다
- 텍스트와 바이너리 | 두 종류로 나뉘는 파일 형식
- 해상도와 화소, 픽셀 | 사진과 이미지의 선명도를 결정한다
- 10진법과 2진법, 16진법 | 컴퓨터의 숫자 표현
- 버전과 릴리스 | 같은 소프트웨어의 갱신을 관리한다
- git와 Subversion | 버전 관리 시스템의 정식
- 모듈과 패키지 | 라이브러리를 관리한다
- 표 계산 소프트웨어와 DBMS | 데이터를 묶어서 관리한다
- SMTP와 POP, IMAP | 메일 송수신에 사용된다
- 검색 엔진과 크롤러 | 인터넷상의 데이터를 수집한다
- [시리얼과 패럴렐 | 데이터를 고속으로 송수신한다](http://melonicedlatte.com/2020/06/19/140700.html)
- 물리 ○○ 과 논리 ○○ | 머릿속에서 상상한다
- 스케일 아웃과 스케일 업 | 성능을 높이는 기술
- SE와 프로그래머 | 시스템 개발에 종사하는 직종
- 젠더, 어댑터와 컨버터 | 데이터를 변환하는 기기
> 젠더: 인터페이스는 같으나 모양이 다른 것(USB A, C...,전기 돼지코)

> 어댑터: 인터페이스가 다름(USB, PS2 ...)

> 컨버터: 데이터가 변환됨(AVI->MP4 ...)
- 웹사이트와 웹페이지 | 인터넷상에 공개되어 있는 정보


제3장 교섭 · 비즈니스 사용하는 IT 업계 용어

- 공수와 인/일, 인/월 | 개발 기간의 견적에 사용된다
- 사실상의 표준 | 많은 사람이 사용한다
- 리소스와 커패시티 | 사전 확보가 중요
- 런칭과 릴리스 | 일반에 공개한다
- 컷 오버와 서비스 인 | 시스템 개발 종료와 이용 개시
> 개발완료, 서비스 시작
- 프로젝트 매니지먼트 | 계획대로 작업을 추진한다
- WBS | 필요한 작업을 세세하게 분할한다
- SLA | 서비스의 신뢰성을 나타낸다
- SES | IT 업계의 업무 방식
- 리터러시 | 현대의 일반 상식
- 엔드 유저 | 이용자를 의식한다
- 픽스 | 사양 변경을 허락하지 않는다
- 트레이드오프 | 한쪽을 세우면 다른 한쪽을 달성하지 않는다
- 액세시빌리티 | 누구나 사용할 수 있는 점을 의식한다
- 유저빌리티 | 사용 편의성을 최우선으로 생각한다
- 디폴트 | 많은 사람이 그대로 사용한다
- 임계값 | 판단하는 기준이 되는 값
- 리플레이스 | 새로운 시스템으로 대체한다
- 시뮬레이션 | 몇 가지 조건으로 검증한다
- 프로토타입 | 시험으로 만들어 본다
- 인터페이스 | 다른 기기를 연결한다
- UI와 UX | 이용자의 시선에서 생각한다
- 인시덴트와 장애 | 트러블에 적절하게 대응한다
- 채널 | 효과적으로 집객한다
- 버즈 워드 | 일시적으로 대유행하는 단어
- URL과 URI | 인터넷상 문서 장소
- HTTP와 HTTPS | 콘텐츠를 전송한다
- 액세스 포인트 | 무선 LAN에 접속한다
- 스루풋과 트래픽 | 통신의 혼잡 상황을 안다
- 프록시 서버 | 통신 대리인
- 홈 디렉터리와 커런트 디렉터리 | 계층을 이동하는 기점
- 캐시 | 한 번 사용한 것은 보존해 둔다
- 아카이브 | 오랜 데이터는 소중하게 보관한다
- 캡처 | 데이터를 확보한다
- 콘트라스트 | 명암을 확실히 구분한다
- 옴니채널 | 복수의 판매 경로를 생각한다
- 레거시 마이그레이션 | 구형 시스템을 신형으로 전환한다
- RFP(제안 의뢰서) | 시스템 개발 의뢰에 필수인 문서


제4장 웹사이트 작성과 SNS 운용에서 사용되는 IT 용어

- 전자상거래 | 인터넷상에서의 거래
- 아피리에이트 | 웹사이트에서 광고 수입을 얻는다
- SEO와 SEM | 검색 결과의 상위에 표시한다
- 큐레이션 | 특정 테마에 따라서 통합한다
- 소셜 미디어와 SNS | 사람과 기업이 상호 이어지는 서비스
- CMS | 웹사이트를 간단하게 갱신할 수 있는 구조
- 랜딩 페이지 | 방문자가 최초로 액세스하는 페이지
- 컨버전 | 웹사이트에서의 목표 달성
- 퍼스트 뷰 | 스크롤하지 않고 표시하는 범위
- 임프레션 | 게재되어 있는 광고를 본 횟수
- 페이지 뷰 | 특정 페이지가 열린 횟수
- KPI와 KGI | 목표를 달성하기 위한 평가 지표
- AB 테스트 | 여러 패턴을 비교해서 평가
- 사이트 이동 경로 | 열람하고 있는 페이지의 위치를 파악
- 리스폰시브 디자인 | 화면 크기에 따라 자동으로 레이아웃이 바뀐다
- 섬네일 | 축소한 이미지를 일람으로 표시한다
- 리다이렉트 | 다른 URL로 이동시킨다
- 렌탈 서버 | 사업자의 서버를 빌린다
- 웹사이트 맵 | 웹사이트의 페이지 구성을 정리한다
- HTML | 웹페이지를 작성하기 위한 언어
- CSS(스타일 시트) | 웹페이지를 디자인한다
- 쿠키 | 웹 서버와 브라우저 간에서 상태를 관리한다
- 미니멀 디자인 | 필요 최소한의 기능에 압축한다
- 레이어 | 이미지 처리 소프트웨어 등에서의 계층
- 래스터라이즈 | 이미지를 도트의 표현으로 변환
- 슬라이스 | 이미지를 분할해서 보존
- 와이어 프레임과 디자인 캠프 | 디자인 제작 전에 만드는 견본
- 칼럼 | 웹 디자인의 열 세팅
- 헤더, 사이드바, 메인, 후터 | 웹페이지의 구성 요소
- 콘텐츠 | 웹페이지의 본문
- 매시업 | 복수의 정보를 조합해서 새로운 서비스를 생성
- 오픈 소스 | 소프트웨어의 소스 코드를 공개
- 스크레이핑 | 웹페이지에서 정보를 추출한다
- FTP와 SCP | 안전하게 파일을 수송신한다
- JPEG와 PNG | 이미지 압축 기술
- OGP | SNS 표시를 생각해서 웹페이지에서 수행하는 설정
- 패럴랙스 | 스크롤의 속도로 입체적으로 보이는 효과
- 머티리얼 디자인과 플랫 디자인 | 디자인 트렌드
- CDN | 웹사이트의 전송 속도를 높이는 네트워크


제5장 사이버 공격에 맞서는 시큐리티 용어

- 해커와 크래커 | 컴퓨터와 네트워크 지식을 가진 사람
- 멀웨어와 바이러스, 웜 | 다른 프로그램에 감염된다
- 패턴 파일과 샌드박스 | 바이러스 대책에 필수 기술
- 스팸 메일 | 대량으로 송신되는 스팸 메일
- 스파이웨어와 키 로거 | 소중한 정보를 외부로 송신한다
- 랜섬웨어 | 대금을 요구하는 바이러스
- 표적형 공격 | 특정 조직을 노리는 공격
- DoS 공격 | 과부하 상태를 만들어낸다
- 무차별 대입 공격과 패스워드 리스트 공격 | 패스워드를 노린다
- 소셜 엔지니어링 | 인간의 약점을 노린다
- 2요소 인증과 2단계 인증 | 패스워드가 알려져도 부정 로그인하지 못한다
- 싱글 사인온 | 인증 정보를 계승한다
- 위장 | 다른 이용자로 위장하여 활동한다
- 익명성 | 신원을 감추고 행동한다
- 사이버 범죄 | 매년 증가하는 네트워크상 범죄
- 부정 액세스 | 네트워크를 통해 공격한다
- 취약성과 시큐리티 홀 | 공격자가 노리는 오류
- 제로데이 공격 | 수정되기 전에만 성립하는 공격
- ISP(프로바이더) | 인터넷 접속에 필수인 조직
- 인증과 인가 | 본인 확인에 추가해서 필요한 허가
- 액세스권 | 사람에 따라서 액세스할 수 있는 범위를 결정한다
- 암호화와 복호 | 도청돼도 내용을 알 수 없게 한다
- 하이브리드 암호 | 공통 키 암호와 공개 키 암호의 조합
- 해시 | 개찬의 검출에 사용된다
- 전자서명 | 본인이 작성했는지를 확인한다
- 증명서 | 제3자에 의한 보증
- SSL / TLS | 통신을 암호화한다
- WEP와 WPA | 무선 LAN의 암호화 방식
- VPN | 공중 무선 LAN으로 안전한 통신을 실현
- 패킷 필터링 | 통신 경로상에서 내용을 확인
- 위태화 | 암호의 안전성이 위협받는다
- 디지털 포렌식 | PC에 남겨진 기록을 분석
- 파이어월 | 부정 통신을 차단한다
- 정보 시큐리티(3가지 요소) | 시큐리티의 CIA
- 시스템 감사와 시큐리티 감사 | 내부와 외부의 이중 체크
- 신 클라이언트 | 단말기에 데이터를 보존하지 않는다


제6장 IT 업계 종사자가 알아야 할 기본 용어

- 5대 장치 | 어느 컴퓨터에나 공통되는 장치와 기능
- IC(집적회로) | 작은 부품의 조합
- 디바이스와 디바이스 드라이버 | PC의 주변 기기를 조작
- 스토리지 | 대용량이 요구되는 기억 장치
- 마운트 | 기억 장치를 사용할 수 있는 상태로 한다
- 무정전전원장치 | 낙뢰 등에 의한 정전에 대응한다
- 블레이드 PC | 데이터 센터용 컴퓨터
- 가상 머신 | 소프트웨어상에서 컴퓨터를 움직인다
- 가상 메모리 | 소프트웨어로 실현하는 메모리 관리
- 프로그래밍 언어 | 컴퓨터 프로그램을 만들 때 사용하는 언어
- 소스 코드와 컴파일 | 컴퓨터가 읽을 수 있는 형태로 변환
- 알고리즘과 플로 차트 | 처리 순서를 효율화
- 절차형과 오브젝트 지향 | 소스 코드의 보수성을 높인다
- 함수형과 논리형 | 수순보다 목적을 기술한다
- 버그와 디버그 | 프로그래밍의 오류를 수정한다
- 단위 테스트와 통합 테스트 | 프로그램의 동작을 확인한다
- 블랙박스 테스트와 화이트박스 테스트 | 다른 시점에서 테스트한다
- 커버리지와 몽키 테스트 | 망라성을 확인한다
- 프레임워크 | 개발 효율 향상에 공헌
- 페어 프로그래밍 | 작업 효율과 품질 향상에 도움 된다
- 프로퍼티 | 설정을 변경, 표시한다
- 가비지 컬렉션 | 불필요해진 메모리 영역을 해방
- 리팩터링 | 동작을 바꾸지 않고 소스 코드의 내부 구조를 개선 세련
- 커널 | 운영 체제의 핵심이 되는 컴퓨터 프로그램
- API와 SDK | 개발에 필요한 라이브러리를 호출한다
- MVC와 디자인 패턴 | 오브젝트 지향에서 자주 사용하는 정석
- 데이터형과 널 | 프로그램에서 격납할 수 있는 데이터를 지정
- 큐와 스택 | 데이터를 일렬로 격납
- 함수와 인수, 절차와 루틴 | 한묶음의 작업을 정리
- 재귀 호출 | 자기자신을 호출하는 함수
- 관계형 데이터베이스와 SQL | 복수의 수를 연결해서 관리
- 테이블과 인덱스 | 데이터를 표 형식으로 관리
- 정규화와 주 키 | 취급하기 쉽도록 테이블을 분할
- 트랜잭션과 체크 포인트 | 데이터의 소실을 방지한다
- 데드록과 배타 제어 | 동시 갱신을 피한다
- 저장 프로시저 | 일련의 처리를 묶어서 실행
- 부하 분산 | 여러 대의 기기로 처리를 분담
- 핫 스탠바이와 콜드 스탠바이 | 장애 발생에 대비한다


제7장 IT 업계에서 알아둬야 할 인물

- 앨런 튜링 | 튜링 테스트의 고안자
- 클로드 섀넌 | 정보 이론의 아버지
- 에드가 F. 코드 | 관계 모델을 발명
- 존 폰 노이만 | 노이만형 컴퓨터의 개념을 발표
- 존 배커스 | 배커스 나우어 형식의 고안자
- 존 맥카시 | 프레임 문제 제창자로 LISP 개발자
- 마빈 민스키 | 인공지능의 아버지
- 고든 무어 | 무어의 법칙 제창자
- 에츠허르 데이크스트라 | 구조화 프로그래밍 제창자
- 도널드 커누스 | 문예적 프로그래밍 제창자
- 스티븐 쿡 | NP 완전 문제의 존재를 증명
- 앨런 케이 | 컴퓨터의 아버지
- 래리 앨리슨 | 오라클 공동 창업자
- 리처드 스톨먼 | 프리소프트웨어 활동가
- 폴 앨런 | 마이크로소프트 공동 창업자로 하드웨어에도 조예가 깊다
- 팀 버너스 리 | WWW의 아버지
- 에릭 슈미트 | 구글(현 알파벳사) 전 CEO
- 빌 게이츠 | 마이크로소프트 공동 창업자로 프로그래머로도 유명하다
- 스티브 잡스 | 애플 공동 창업자
- 팀 쿡 | 애플 CEO
- 마이클 델 | 델 창업자
- 리누스 토발즈 | 리눅스 개발자
- 일론 머스크 | 테슬라 CEO | 280
- 래리 페이지, 세르게이 브린 | 구글(현 알파벳사) 공동 창업자
- 마크 저커버그 | 페이스북 공동 창업자
- 제프 베조스 | 아마존 공동 창업자

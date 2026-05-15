# 🌱 반려식물 통합 관리 플랫폼 (Backend-GardenLog)

사용자가 반려식물을 체계적으로 기록하고 관리할 수 있도록 돕는 **가든로그(GardenLog) 서비스의 백엔드 시스템** 구현 프로젝트입니다. <br>
Eclipse 환경에서 Java Servlet과 JSP를 활용하여 웹 서비스를 구축하였으며, 식물의 성장 기록 관리 기능을 제공합니다.
<br>
<br>

## 👥 프로젝트 정보
- **개발자:** 이세연, 이나연, 조혜인
- **프로젝트 기간**: 2025.11 ~ 2025.12 (약 6주)
<br>

## 📂 폴더 구조 (Project Structure)
```text
Backend-GardenLog/
├── src/
│   └── com/
│       └── garden/
│           └── gardenlog/
│               ├── controller/      # Servlet (요청 처리 및 흐름 제어)
│               ├── dao/             # Data Access Object (DB 접근 로직)
│               ├── dto/             # Data Transfer Object (데이터 객체)
│               └── util/            # DB Connection 등 공통 유틸리티
├── WebContent/
│   ├── WEB-INF/
│   │   ├── lib/                     # JDBC Driver 및 외부 라이브러리
│   │   └── web.xml                  # 서블릿 매핑 및 프로젝트 설정
│   ├── css/                         # 스타일시트 파일
│   ├── js/                          # 자바스크립트 파일
│   └── views/                       # JSP 파일 (화면 구성)
└── README.md
```

## 1. 개발 목표 및 특징
- **Servlet 기반 웹 아키텍처:** MVC 패턴을 적용하여 서블릿(Controller), 자바빈즈(Model), JSP(View)를 분리한 구조 설계.
- **동적 웹 페이지 구현:** 사용자 요청에 따라 식물 데이터 및 성장 일기를 실시간으로 처리하여 화면에 출력.
- **데이터 영속성 관리:** JDBC를 활용하여 데이터베이스와 연동하고, DAO(Data Access Object) 패턴을 통한 데이터 처리 로직 구현.
- **성장 기록 관리:** 식물별 일기 작성 및 이력 관리를 통해 반려식물의 성장 과정을 체계적으로 저장.
<br>
<br>

## 2. 주요 기술 스택 및 구성

### 🛠 백엔드 (Back-end)
| 분류 | 기술 스택 | 주요 역할 |
| :--- | :--- | :--- |
| **Tool** | Eclipse IDE | 통합 개발 환경 및 서버 제어 |
| **Technology** | Java Servlet / JSP | 서버 사이드 로직 처리 및 동적 콘텐츠 생성 |
| **Language** | Java | 비즈니스 로직 및 객체 지향 프로그래밍 구현 |
| **Database** | MySQL | 회원 정보, 식물 리스트, 성장 일기 데이터 저장 |
| **Library** | JDBC Driver | 자바 애플리케이션과 데이터베이스 간 통신 연결 |
| **Server** | Apache Tomcat | 웹 애플리케이션 서버(WAS) 구동 및 배포 |

### 💻 프론트엔드 및 협업
- **Frontend:** HTML5, CSS3, JavaScript
- **Version Control:** Git, GitHub
<br>

## 3. 주요 기능 및 엔터티 구조
- **식물 관리 (My Garden):** 사용자가 키우는 반려식물의 종류, 별명, 입양일 등을 등록하고 관리.
- **성장 일기 (Growth Log):** 날짜별 식물 상태 기록, 물 주기 체크, 사진 업로드 기능.
- **회원 시스템:** 일반 로그인 및 소셜 로그인 연동을 통한 개인별 맞춤형 식물 데이터 저장.
- **커뮤니티:** 다른 사용자들의 정원을 구경하고 정보를 공유할 수 있는 게시판 및 댓글 로직.
<br>
<br>

---

## 📂 프로젝트 결과물 확인
* 📄 **결과보고서:** [GardenLog 결과보고서.pdf](./docs/GardenLog%20결과보고서.pdf)

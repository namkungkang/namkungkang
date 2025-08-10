### <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F78731&background=D650FF00&width=435&lines=namkungkang's+GitHub" alt="Typing SVG" /></a>


## 📊 GitHub Stats
<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=namkungkang&show_icons=true&theme=radical"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=namkungkang&layout=compact&theme=radical"/>
</div>


## 💻 Tech Stacks
<p>
<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=C&logoColor=white"/> 
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=C%2B%2B&logoColor=white"/> 
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white"/> 
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/>
<img src="https://img.shields.io/badge/Html5-E34F26?style=flat-square&logo=HTML5&logoColor=white"/> 
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=CSS3&logoColor=white"/> 
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=black"/> 
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/> 
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>   
<img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white"/>   
   
</p>

## 🛠️ **Tools**
<p>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white"/>
<img src="https://img.shields.io/badge/Mysql-003B57?style=flat-square&logo=mysql&logoColor=white"/>


</p>

## 🏆 **Awards**
**＃ UMC 7th Demoday 대상**


<img width="825" alt="Image" src="https://github.com/user-attachments/assets/e35bf514-0866-470d-adcb-96df9a1e24fe" />


# 📌 프로젝트명 (Backend)
> "CHIC-CHIC"  
> 향수 전문 쇼핑과 커뮤니티 서비스를 제공하는 웹 플랫폼

---

## 📖 프로젝트 소개
- Spring Boot 기반 REST API 서버
- 주요 기능:
  - 유저 설문조사 데이터 수집 및 저장
  - OpenAI GPT API 연동하여 맞춤형 건강 점수 및 피드백 제공
  - JWT 인증 기반 로그인/회원가입
  - AWS S3 이미지 업로드
  -   RDS(MySQL) 기반 데이터 영속화

---

## 🌿 브랜치 전략
> Git Flow 전략

- **main** : 배포 브랜치
- **develop** : 개발 통합 브랜치
- **feature/** : 기능별 브랜치 (`feature/auth`, `feature/perfume`)
- **bug/** : 긴급 수정 브랜치
- **release/** : 배포 전 QA 브랜치

## 🛠️ 기술 스택 

| 구분        | 기술 및 라이브러리                      |
|-------------|---------------------------------------|
| **언어**    | Java 17                               |
| **프레임워크** | Spring Boot 3.2.5                      |
| **빌드 도구** | Gradle                               |
| **데이터베이스** | MySQL 8                              |
| **ORM**      | Spring Data JPA (Hibernate)           |
| **API 문서화** | Swagger |
| **보안**     | Spring Security, JWT                   |
| **클라우드 스토리지** | AWS S3                             |
| **배포**     | Docker, AWS EC2                       |
| **CI/CD**    | GitHub Actions                       |
| **기타**     | Lombok                    |

---



## 📂 프로젝트 구조

<details>
  <summary>폴더 구조 펼치기/접기</summary>

```plaintext
chic_chic
└── spring
    ├── Application.java
    │
    ├── apiPayload
    │   ├── ApiResponse.java
    │   ├── code
    │   │   ├── BaseCode.java
    │   │   ├── BaseErrorCode.java
    │   │   ├── ErrorReasonDTO.java
    │   │   ├── ReasonDTO.java
    │   │   └── status
    │   │       ├── ErrorStatus.java
    │   │       └── SuccessStatus.java
    │   └── exception
    │       ├── ExceptionAdvice.java
    │       ├── GeneralException.java
    │       └── handler
    │           ├── CustomException.java
    │           ├── CustomOAuth2SuccessHandler.java
    │           └── MemberHandler.java
    │
    ├── auth
    │   ├── CustomAccessDeniedHandler.java
    │   ├── CustomAuthenticationEntryPoint.java
    │   └── UserDetailsServiceImpl.java
    │
    ├── client
    │   └── AIRecommendClient.java
    │
    ├── config
    │   ├── RestTemplateConfig.java
    │   ├── S3Config.java
    │   ├── SecurityConfig.java
    │   ├── SwaggerConfig.java
    │   ├── jwt
    │   │   ├── JwtAuthenticationFilter.java
    │   │   ├── JwtTokenProvider.java
    │   │   └── JwtUtil.java
    │   └── properties
    │       ├── Constants.java
    │       └── JwtProperties.java
    │
    ├── converter
    │   ├── ConsultPostConverter.java
    │   ├── MemberConverter.java
    │   ├── TestQuestionConverter.java
    │   └── TestResultConverter.java
    │
    ├── domain
    │   ├── Category.java
    │   ├── ConsultPost.java
    │   ├── Member.java
    │   ├── Note.java
    │   ├── Product.java
    │   ├── ProductNote.java
    │   ├── ProductNoteId.java
    │   ├── RefreshToken.java
    │   ├── Scrap.java
    │   ├── TestResult.java
    │   ├── common
    │   │   └── BaseEntity.java
    │   ├── entity
    │   │   ├── Perfume.java
    │   │   ├── PerfumeDiary.java
    │   │   ├── PerfumeDiaryComments.java
    │   │   ├── PerfumeStory.java
    │   │   └── Review.java
    │   ├── enums
    │   │   ├── CategoryType.java
    │   │   ├── Gender.java
    │   │   ├── PostType.java
    │   │   ├── SocialType.java
    │   │   └── mapping
    │   └── repository
    │       ├── CategoryRepository.java
    │       ├── ConsultPostRepository.java
    │       ├── MemberRepository.java
    │       ├── PerfumeDiaryCommentRepository.java
    │       ├── PerfumeDiaryRepository.java
    │       ├── PerfumeStoryRepository.java
    │       ├── ProductRepository.java
    │       ├── RecommendProductRepository.java
    │       ├── RefreshTokenRepository.java
    │       ├── ReviewRepository.java
    │       ├── ScrapRepository.java
    │       └── TestResultRepository.java
    │
    ├── service
    │   ├── AuthService
    │   │   ├── AuthService.java
    │   │   └── AuthServiceImpl.java
    │   ├── category
    │   │   └── CategoryService.java
    │   ├── ConsultPostService
    │   │   ├── ConsultService.java
    │   │   └── ConsultServiceImpl.java
    │   ├── ImageService
    │   │   ├── S3UploaderService.java
    │   │   └── S3UploaderServiceImpl.java
    │   ├── MemberService
    │   │   ├── MemberCommandService.java
    │   │   └── MemberCommandServiceImpl.java
    │   ├── OauthService
    │   │   ├── CustomOAuth2MemberServiceImpl.java
    │   │   ├── Oauth2MemberService.java
    │   │   └── Oauth2MemberServiceImpl.java
    │   ├── perfumediaryservice
    │   │   ├── PerfumeDiaryService.java
    │   │   └── PerfumeDiaryServiceImpl.java
    │   ├── perfumestoryservice
    │   │   └── PerfumeStoryService.java
    │   ├── product
    │   │   ├── HomeProductService.java
    │   │   ├── ProductDetailService.java
    │   │   └── ProductService.java
    │   ├── Review
    │   │   ├── ReviewService.java
    │   │   └── ReviewServiceImpl.java
    │   ├── ScrapService
    │   │   ├── ScrapService.java
    │   │   └── ScrapServiceImpl.java
    │   └── TestSubmitService
    │       └── TestSubmitService.java
    │
    ├── validator
    │   ├── annotation
    │   │   └── PasswordMatch.java
    │   └── validator
    │       └── PasswordMatchValidator.java
    │
    └── web
        ├── controller
        │   ├── AuthController.java
        │   ├── ConsultPostController.java
        │   ├── HomeController.java
        │   ├── MemberController.java
        │   ├── PerfumeDiaryController.java
        │   ├── PerfumeReviewController.java
        │   ├── PerfumeStoryController.java
        │   ├── S3ImageController.java
        │   ├── ScrapController.java
        │   ├── TestQuestionController.java
        │   ├── TestSubmitController.java
        │   ├── category
        │   └── product
        │       ├── ProductController.java
        │       └── ProductDetailController.java
        └── dto
            ├── AIRequestDto.java
            ├── AIResponseDto.java
            ├── AnswerDto.java
            ├── CommentRequest.java
            ├── CommentResponse.java
            ├── ConsultPostRequest.java
            ├── ConsultPostResponse.java
            ├── MemberRequestDTO.java
            ├── MemberResponseDTO.java
            ├── MyDiaryResponse.java
            ├── OptionDto.java
            ├── PerfumeStoryDetailResponse.java
            ├── PerfumeStoryResponse.java
            ├── ProductDetailResponse.java
            ├── ProductListResponse.java
            ├── ProductResponse.java
            ├── QuestionDto.java
            ├── RecommendedPerfumeDto.java
            ├── RecommendProductResponseDto.java
            ├── ReIssueRequestDTO.java
            ├── ReIssueResponseDTO.java
            ├── S3ResponseDto.java
            ├── TestSubmitRequest.java

```
## 👥 백엔드 팀원 정보

| 이름       | 주요 담당 업무                          |
|------------|---------------------------------------|
| 알티 / 남궁강 | 회원/인증/마이홈, JWT 등 공통 설정  |
| 시럽 / 이도훈 | 향수 도메인 ( 메인/카테고리/상세)  |
| 민토리 / 성민주 | 커뮤니티(추천 상담소)  |
| 조이 / 박은서 | 향수 일기장 + 향수 이야기 + 공통 읍답, 예외처리  |



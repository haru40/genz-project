# 젠지표류기 — 현정현 (조장 · 서비스 기획)

![젠지표류기 표지](docs/images/cover.png)

> 낯선 회사에 표류한 신입사원이 **배우고 · 연습하며** 무사히 퇴근하도록 돕는 회사생활 가이드

<table>
  <tr><th align="left" width="130">기간</th><td>2026.09.28 – 11.09</td></tr>
  <tr><th align="left">팀</th><td>4명 · 팀 프로젝트</td></tr>
  <tr><th align="left">내 역할</th><td><b>조장</b> · 서비스 기획 · AI 기능 기획 · UX 설계</td></tr>
  <tr><th align="left">과정</th><td>동아일보 부트캠프 [미디어 프론티어] 생성형 AI 마스터 클래스</td></tr>
  <tr><th align="left">기술</th><td>Next.js · React · TypeScript · Supabase · OpenAI API · Gemini · Vercel</td></tr>
  <tr><th align="left">링크</th><td><a href="https://genz-project-one.vercel.app">서비스 바로가기 ↗</a> · <a href="https://github.com/genz-pyoryugi/genz-project">팀 저장소 (전체 코드) ↗</a></td></tr>
</table>

---

## 목차

<table>
  <tr><th align="left" width="90">기획</th><td><a href="#s1">1. 기획 및 비전</a> — 문제 정의 · 개발 타임라인</td></tr>
  <tr><th align="left">기능</th><td><a href="#s2">2. 핵심 기능 (튜토리얼 → 카드뉴스 → 퀴즈 → AI 팀장)</a> · <a href="#s3">3. AI 팀장 시뮬레이션</a> · <a href="#s4">4. 학습 기능 · 성장 기록</a></td></tr>
  <tr><th align="left">설계</th><td><a href="#s5">5. 서비스 설계</a> · <a href="#s6">6. 작동 구조</a> · <a href="#s7">7. 데이터베이스(ERD)</a></td></tr>
  <tr><th align="left">개발</th><td><a href="#s8">8. 기술 스택 · 의사결정</a> · <a href="#s9">9. 프로젝트 구조</a></td></tr>
  <tr><th align="left">검증</th><td><a href="#s10">10. 피드백 반영</a> · <a href="#s11">11. 사용자 테스트 결과</a></td></tr>
  <tr><th align="left">팀</th><td><a href="#s12">12. 팀 구성</a></td></tr>
</table>

---

<a name="s1"></a>

![1. 기획 및 비전 — 문제 정의 · 개발 타임라인](docs/sections/plan.png)

출발점 기사: [동아일보 「신입사원 첫 출근, ‘이 실수’했다간 첫 단추 잘못 끼운다」 (2026.04.10) ↗](https://www.donga.com/news/Society/article/all/20260410/133715092/2)

---

<a name="s2"></a>

## 2. 핵심 기능

**튜토리얼 → 학습 → 이해 → 실전 연습**

<table>
  <tr>
    <td width="50%" valign="top"><img src="docs/screens/tutorial.jpg" width="100%" alt="튜토리얼"><br><b>0 · 튜토리얼</b><br><sub>걱정되는 주제를 고르면 카드뉴스 → 퀴즈 → AI 팀장 순서로 안내</sub></td>
    <td width="50%" valign="top"><img src="docs/screens/cardnews.jpg" width="100%" alt="카드뉴스 · 학습 전후 체크"><br><b>1 · 카드뉴스 · 학습 전후 체크</b><br><sub>읽기 전과 후에 이해도를 스스로 체크해 변화 확인</sub></td>
  </tr>
  <tr>
    <td width="50%" valign="top"><img src="docs/screens/quiz.jpg" width="100%" alt="퀴즈 · 오답 다시 풀기"><br><b>2 · 퀴즈 · 오답 다시 풀기</b><br><sub>상황별 문제와 해설, 틀린 문제만 골라 다시 풀기</sub></td>
    <td width="50%" valign="top"><img src="docs/screens/ai.jpg" width="100%" alt="AI 팀장 피드백"><br><b>3 · AI 팀장 피드백</b><br><sub>팀장에게 직접 답하고 3가지 기준 · 15점 만점 피드백</sub></td>
  </tr>
</table>

**부가 콘텐츠** — 같은 주제를 다양하게

<table>
  <tr>
    <td width="20%" valign="top"><img src="docs/screens/sos.jpg" width="100%" alt="SOS 상담"><br><sub><b>SOS 상담</b></sub></td>
    <td width="20%" valign="top"><img src="docs/screens/radio.jpg" width="100%" alt="보이는 라디오"><br><sub><b>보이는 라디오</b></sub></td>
    <td width="20%" valign="top"><img src="docs/screens/community.jpg" width="100%" alt="고민상담소"><br><sub><b>고민상담소</b></sub></td>
    <td width="20%" valign="top"><img src="docs/screens/calendar.jpg" width="100%" alt="근태 가이드"><br><sub><b>근태 가이드</b></sub></td>
    <td width="20%" valign="top"><img src="docs/screens/checklist.jpg" width="100%" alt="체크리스트"><br><sub><b>체크리스트</b></sub></td>
  </tr>
</table>

---

<a name="s3"></a>

![3. AI 팀장 시뮬레이션 — 프롬프트 설계 · 개선 과정](docs/sections/ai.png)

---

<a name="s4"></a>

![4. 학습 기능 · 성장 기록](docs/sections/learning.png)

**퇴근길 아웃트로** — 사무실을 나서면 인사 → 스크롤하면 오늘의 성장 기록

<p align="center"><img src="docs/screens/outro.gif" width="70%" alt="퇴근길 아웃트로 영상"></p>

![오늘의 성장 기록 · 학습 기록이 이어지는 흐름](docs/sections/learning-growth.png)

---

<a name="s5"></a>

![5. 서비스 설계 — Use Case](docs/sections/usecase.png)

---

<a name="s6"></a>

![6. 작동 구조 — 입력부터 결과물까지](docs/sections/works.png)

---

<a name="s7"></a>

![7. 데이터베이스 설계 — ERD](docs/sections/erd.png)

---

<a name="s8"></a>

![8. 기술 스택 · 기술적 의사결정](docs/sections/stack.png)

---

<a name="s9"></a>

![9. 프로젝트 구조](docs/sections/tree.png)

---

<a name="s10"></a>

![10. 피드백 반영 — 받은 피드백 → 기능](docs/sections/feedback.png)

---

<a name="s11"></a>

![11. 사용자 테스트 결과 — 2026.10.28](docs/sections/usertest.png)

---

<a name="s12"></a>

## 12. 팀 구성

| 역할 | 담당 |
|---|---|
| **현정현 · 조장** | 서비스 기획 · AI 기능 기획 · UX 설계 — 서비스 방향 · 핵심 기능 기획, 7개 카테고리 콘텐츠 구조 설계, AI 팀장 시뮬레이션 설계, 기능 우선순위 조율 · 협업 리딩 |
| 팀원 · 백엔드 · 데이터 | 퀴즈 · 체크리스트 · 근태 가이드, SOS 상담 API · 학습 기록, Supabase · 서버 API · RLS |
| 팀원 · 커뮤니티 · 라디오 | 고민상담소, 입력 유효성 검사 · 신고, 보이는 라디오(AI 대본 · 음성) |
| 팀원 · 콘텐츠 | 카드뉴스 제작, 기사 · 공식 PDF 조사, 학습 전후 체크 → 퀴즈 흐름 설계 |

---

젠지표류기 · 동아일보 부트캠프 [미디어 프론티어] 생성형 AI 마스터 클래스 2026 · 사용자 테스트 수치는 2026.10.28 익명 학습 기록(개발 중 확인 실행 제외)

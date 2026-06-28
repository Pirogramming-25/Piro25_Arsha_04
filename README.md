# Piro25_Arsha_04
## Piro25_Arsha_04

HTML/CSS를 사용하여 Arsha 페이지를 클론코딩하는 팀 프로젝트입니다.
JavaScript는 사용하지 않고, 반응형 웹 구현을 목표로 합니다.

---

## 역할 분담

| 담당 | 구현 범위                                                     | CSS 파일      |
| -- | --------------------------------------------------------- | ----------- |
| 김유겸 | Preview Bar, Header, Hero, Clients, About, Why Us, Footer | `part1.css` |
| 신예원 | Skills, Services, Work Process, CTA, Contact              | `part2.css` |
| 정승현 | Portfolio, Team, Newsletter                               | `part3.css` |
| 장희원 | Pricing, Testimonials, FAQ, Blog                          | `part4.css` |

---

## 브랜치 전략

* `main`: 최종 제출용 브랜치
* `develop`: 팀원 작업을 합치는 기본 브랜치
* 개인 브랜치: 각자 작업하는 브랜치

작업은 개인 브랜치에서 진행하고, 완료 후 `develop` 브랜치로 PR을 생성
최종 제출 전 `develop` 내용을 확인한 뒤 `main` 브랜치에 병합

---

## PR / Merge 규칙

1. 개인 브랜치에서 작업 후 `develop` 브랜치로 PR을 올립니다.
2. PR을 올리기 전 `develop` 브랜치의 최신 내용을 반영합니다.
3. PR을 올리면 카톡방에 공유합니다.
4. 최소 1명 이상 `Approve`를 받은 뒤 merge합니다.
5. PR 작성자는 승인 확인 후 직접 merge할 수 있습니다.
6. `main` 브랜치는 최종 제출 전까지 직접 수정하지 않습니다.
7. `common.css`, `reset.css`, `index.html`처럼 공통으로 영향이 큰 파일을 수정할 때는 미리 공유합니다.

---

## CSS 파일 구조

```txt
css/
├── reset.css
├── common.css
├── part1.css
├── part2.css
├── part3.css
└── part4.css
```

- `reset.css`: 기본 브라우저 스타일 초기화
- `common.css`: 색상 변수, 공통 섹션 제목, 기본 스타일
- `part1.css`: 김유겸 담당 영역 스타일
- `part2.css`: 신예원 담당 영역 스타일
- `part3.css`: 정승현 담당 영역 스타일
- `part4.css`: 장희원 담당 영역 스타일

공통으로 사용하는 색상 값은 `common.css`의 `:root`에 변수로 저장해서 사용합니다.

<sub>※ 색상, 간격, 폰트 크기 등 세부 디자인 값은 원본 Arsha 페이지를 F12 개발자도구로 확인하여 참고합니다.</sub>

## 커밋 메시지 규칙

| 타입      | 의미                   |
| ------- | -------------------- |
| `feat`  | 새로운 섹션 또는 기능 구현      |
| `style` | CSS 스타일 수정           |
| `fix`   | 오류 수정                |
| `docs`  | README 등 문서 수정       |
| `chore` | 폴더 구조, 파일 정리 등 기타 작업 |

예시:

```txt
feat: portfolio 섹션 구현
style: team 카드 hover 스타일 추가
fix: 이미지 경로 수정
docs: README 역할 분담 추가
chore: CSS 파일 구조 정리
```

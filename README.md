# KSynapse 스킬 설치 안내

## 들어 있는 것 (3개 모두 설치)
| 파일 | 용도 |
|---|---|
| ksynapse-project-design.zip | PDD → KSynapse 과제 설계·개발 절차, SAP GUI 패턴, BRE 설계, 설계서 템플릿 |
| ksynapse-framework.zip | KSynapse 프레임워크 구조 지식 (design 스킬이 참조함) |
| pad-flow-analysis.zip | Horizon 원격 화면의 PAD 편집기를 읽는 절차 |

세 스킬은 서로를 이름으로 참조하므로 하나만 올리면 일부 내용이 빠집니다.

## 1. 사전 조건
- Claude 유료 플랜 (Pro / Max / Team / Enterprise)
- claude.ai → 설정 → 기능(Capabilities) → **코드 실행 및 파일 생성** 켜기 (스킬이 동작하려면 필요)
- Team/Enterprise 조직이면 관리자가 스킬 기능을 막아두지 않았는지 확인

## 2. 설치
1. claude.ai → 설정 → 기능(Capabilities) → **Skills** → **스킬 업로드(Upload skill)**
2. zip 3개를 하나씩 업로드 (압축 풀지 말고 zip 그대로)
3. 목록에서 세 스킬이 **켜짐** 상태인지 확인

웹·데스크톱 앱 모두 같은 계정이면 자동으로 동기화됩니다.

## 3. PAD 화면 작업까지 하려면 (선택)
설계서 작성만 할 거라면 필요 없습니다. Claude가 PAD/SAP 화면을 직접 보고 조작하게 하려면:
- **Claude 데스크톱 앱(Windows)** 설치 → 설정에서 **컴퓨터 사용(Computer use)** 켜기
- 작업 시작 시 Claude가 앱 접근 권한을 물으면 **Omnissa Horizon Client** 를 허용
- Horizon 안에서 PAD·SAP GUI가 열려 있어야 함, 한글 IME는 '가' 상태

## 4. 사용법
- 채팅에서 `/ksynapse-project-design` 입력 후 요청을 이어서 쓰거나,
- 그냥 "이 PDD로 KSynapse 과제 설계해줘"처럼 말해도 자동으로 불러옵니다.
- PDD·운영자매뉴얼·입력 엑셀을 첨부하면 설계서 템플릿대로 정리해 줍니다.

## 주의
- 스킬 원칙상 전표생성·저장 같은 확정 액션은 개발 중 비활성 상태로 둡니다.
- 비밀번호·계정은 채팅이나 Config에 적지 마세요.

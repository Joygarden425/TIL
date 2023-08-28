# Today I Learned

## git 학습

## .md : 마크다운 문법을 쓰는 파일

## 스테이징 영역
- 스테이징 영역은 커밋 전, 커밋에 포함시킬 파일들만 임시로 올려두는 영역
- stage: 무대에 올리다.
- `.gitignore` 파일
- 커밋에 포함되면 안되는 파일들을 관리하는 파일
- 저장소마다 1개씩 세팅되어있는게 일반적임
 - [Toptal의 gitignore generator](https://www.toptal.com/developers/gitignore)를 사용해서 운영체제, 개발환경(IDE), 사용하는 프로그래밍 언어에 맞는 gitignore파일을 생성할 수 있음
    - 이 외에도 VScode에 Extension을 설치해 gitignore 파일을 관리하기도 함

## 브랜치
- branch: (영한사전 정의) 나뭇가지
- (일반적으로) 일감을 해결할 때 일감에 해당하는 이슈를 만들고, 이슈를 해당하는 브랜치를 생성함

### 브랜치 병합
- 이슈에 해당하는 브랜치에서 작업을 끝내고 주요 브랜치인 `main`, `development` 등에 병합 요청을 하게 됨

### 충돌
- 두 브랜치에서 같은 코드를 수정한 후, 병합하려고 할 때 발생
- 충돌이 발생하면, 충돌이 발생한 파일을 열어서 최종적으로 남기고 싶은 코드만 남긴다(특수 문자는삭제)
- `git add`, `git commit`으로 병합을 마무리 한다.

### 명령어
- 브랜치 생성: `git branch 브랜치명`
- 생성된 브랜치 확인: `git branch`
- 브랜치 전환
 1. `git switch 브랜치명`
 2. `git checkout 브랜치명`
 - 브랜치 생성 및 전환
 1. `git checkout -b 브랜치명`
 - 브랜치 병합: `git merge`
  - 주의: `A` 브랜치를 `B` 브랜치로 병합하려고 할 때, `B` 브랜치가 체크아웃 되어있는 상태에서 `git merge A`을 입력해야 한다.

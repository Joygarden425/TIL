# git 학습

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

2024-1-Beginner-Study WIL1
=======================

*  GitHub를 사용하는 이유
    * 코드 수정 및 파일 관리
    * 팀 단위 프로젝트 시, 해당 프로젝트 관리
        * 여러 개발자들이 동시에 작업할 경우 동기화 필요
        * 배포 이후 버전 관리 용이
        * 누가, 언제,  어떻게 파일을 수정했는지 확인하기 용이함

* 파일의 생명주기
    * Untracked
    * Unmodified
    * Modified
    * Staged

* Git을 이용한 GitHub 업로드 절차
    1. Directory에 Git 저장소 만들기
        > git init
    2. Git으로 관리할 대상 등록
        > git add
        * 모든 파일을 한번에 등록
            > $ git add .
        * 한 가지 파일만 등록
            > $ git add "FILENAME"
        * unstage로 되돌리기
            > $ git rm --cached "file"
    3. 파일 수정 후  로컬 저장소로 옮기기
        > $ git commit -m "commit message"
    4. GitHub에 push하기
        >  $ git push origin main

* Commit 메시지 작성 요령
    * "type : subject" 양식으로 작성

    * Commit Message type
        * feat
            * 새로운 기능 추가
        * refactor
            * 기존 코드 개선
        * fix
            * 버그 수정
        * chore
            * 코드 외의 설정 변경
        * docs
            * 문서화
        * test
            * 테스트 코드
        

* 실습 Repository 링크   
    > (https://github.com/nockbeet/nockbeet)

2024-1-Beginner-Study WIL2
=======================
* ## GitHub의 Fork / Star
    * ### Fork
        * 다른 사용자의 Repository를 자신의 계정으로 가져와 독립적으로 수정 및 관리
    * ### Star
        * 관심 있는 Repository나 프로젝트에 star를 지정하여 "북마크"와 같이 관리
        * Repository URL 끝에 `\stargazers`를 추가하면, star를 지정한 모든 사용자를 확인할 수 있다.

* ## Issue
    * Repository에서 작업 계획, 토론 및 추적을 위해 활용

* ## Branch
    * 동일한 Repository 내에서, 독립적으로 서로 다른 작업을 진행하기 위한 별도의 작업 공간
    * 각 Branch는 병합 등 별도의 조정이 없으면 서로 영향을 받지 않기 때문에, 필요에 따라 여러 작업을 동시에 수행 가능하다.

* ## Pull Request
    * 분기된 Branch를 다시 병합하기 위한 절차
    * 공동 작업자 등의 사람들의 리뷰를 통해, 서로 의견을 주고받거나 Branch를 Merge할지 결정할 수 있다.
    * Merge 옵션
        * Merge Commit : 두 Branch를 공통 부모로 하는 새 commit을 만듦.
        * Sqash and Merge : 각 commit을 하나의 commit으로 뭉쳐 하나의 Branch로 병합
        * Rebase and Merge : 각 commit의 base를 재설정하여, 모두 새로운 commit으로 변경. commit conflict 발생 시 Merge하려는 모든 commit에서 conflict가 발생할 수 있다.


* Pull Request 페이지 링크
    >[https://github.com/nockbeet/2024-1-Beginner-Study/pull/2](https://github.com/nockbeet/2024-1-Beginner-Study/pull/2) 
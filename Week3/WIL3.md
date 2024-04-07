2024-1-Beginner-Study WIL3
=======================
* ## git log 둘러보기
    * ### git log
        * commit history를 확인할 수 있다.
        * `--oneline` 옵션을 사용하여 각 commit을 한 줄로 요약 가능하다
    * ### commit id
        * commit 식별을 위해 사용하는 40자 길이의 16진수
        * SHA-1 해시 함수를 사용
    * ### HEAD
        * 현재 작업 중인 위치를 가리킴
        * 현재 작업 중인 브랜치의 가장 최근 commit으로, 다음 commit의 base가 되는 commit이기도 하다.
        * 새 commit이 생기면 HEAD도 변경됨

* ## commit 되돌리기
    * ### commit --amend
        * 마지막 commit의 내용에 변경이 있을 시 사용
        * 완전히 새 commit으로 대체되며, commit id가 바뀜
        * 주의사항: 다른 사람이 작업 기반으로 삼는 commit을 amend하면 안된다. 기존 commit이 브랜치에서 사라지고 완전히 새로운 commit이 생성되기 때문에, 실수였을 경우 복구가 어렵기 때문이다.
    * ### reset
        * commit을 제거하는 데 사용하고, 3가지 옵션이 존재함.
            * reset --soft
                * commit 취소
                * 변경 사항이 Staged Area로 돌아감. 즉, `add` 명령어 없이 바로 commit 가능
            * reset --mixed
                * commit 취소
                * 변경 사항이 working directory로 돌아감. 변경 사항 반영하려면 `add` 명령어 사용
            * reset --hard
                * commit 취소
                * 변경 사항을 모두 제거하고 이전 commit으로 되돌아감.
    * ### revert
        * commit을 제거하지 않고 되돌림
        * 되돌리기 위한 새 commit 생성
        * `--edit` 옵션이 default

    * ### reset과 revert 비교
        * reset은 commit을 삭제하므로 위험
            * commit을 공유하는 다른 branch에도 영향을 줄 수 있음
        * commit을 삭제하기보단, 새로 생성하여 되돌리는 revert가 안전
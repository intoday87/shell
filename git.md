# git


- 트래킹하는 파일을 임시적으로 변경분 무시하기
  ```
  $ git update-index --assume-unchanged path/to/file
  ```
  - 다시 되돌리기
    ```
    $ git update-index --no-assume-unchanged path/to/file
    ```
  - 해당 목록 조회. `ls-files`에서 `h /path/to/file` 소문자 `h`로 시작함
    ```
    $ git ls-files -v | grep '^[[:lower:]]'
    ```
    

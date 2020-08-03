# shell
shell script에 필요한 내용 정리

- exit code 알아내는 방법
  - ```zsh
    $ ls /var/ready
    $ echo $?
    0 // 정상
    ```
    
- stdout 파일로 기록
  - `$ [command] &>[filename]
  

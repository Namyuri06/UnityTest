Assets > Scripts 폴더에 들어가시면 UnityTest.cs 파일이 들어있습니다. 이 파일을 다운로드 받으셔서 이름과 클래스 이름을 본인 이름으로 바꾸시고
(파일과 클래스 이름이 동일해야함) 똑같이 Assets > Scripts 폴더에 해당 파일을 넣은 다음 깃허브에 푸쉬해보세요.

<간단한 순서 정리>
1. 빈폴더 생성
2. 해당 폴더에 git bash here로 git 창 열기
3. git clone https://github.com/Namyuri06/UnityTest.git
4. cd UnityTest
5. unityhub에서 add로 열기
6. asset > scripts 폴더 내의 UnityTest.cs "복사"해서 파일명과 클래스 이름을 본인 이름으로 바꾸기(파일과 클래스 이름이 동일해야함)
7. git checkout -b 브랜치이름 (브랜치이름은 확인하기 편하도록 본인 이름으로)
8. git branch(브랜치가 제대로 변경됐는지 확인) ← *이 붙어있는 브랜치가 현재 브랜치
9. git status
10. git add 파일명(경로까지 써야 함)<br>
    예) git add Assets/Scripts/UnityTest.cs
11. git commit -m "커밋 설명"
12. git push origin 브랜치이름 (main 말고 본인 브랜치에 푸쉬하세요)
13. 깃허브 레포지토리 UnityTest에 접속해서 Pull requests 클릭
14. base: main ← 합쳐질 곳<br>
    compare: 내 브랜치 ← 내가 작업한 브랜치<br>
    이대로 생성
15. Create Pull Request 클릭
16. Merge pull request 클릭 → Confirm merge (머지하고 나서도 본인 브랜치 삭제는 하지 마세요!)

Q. 왜 바로 메인에 푸쉬하지 않고 본인 브랜치에 푸쉬했다가 메인에 머지하나요?<br>
A. 여러 사람이 동시에 작업하면 코드 충돌(conflict)이 발생할 수 있어서 브랜치에서 먼저 작업하고 검토 후 main에 합칩니다.

Q. 매번 클론해야 하나요?<br>
A. 아닙니다. 처음 한 번만 clone 하면 됩니다. 한 번 클론한 후로는<br>
git checkout main<br>
git pull origin main<br>
명령어로 로컬 메인 브랜치를 최신화해주기만 하면 됩니다.
(이후 다시 작업을 위해 checkout 명령어로 본인 브랜치로 돌아오면 됨)

<주의점>
브랜치에서 작업을 시작하기 전 항상 메인 브랜치를 먼저 최신화해주는 것을 잊지 마세요!<br>
git checkout main<br>
git pull origin main

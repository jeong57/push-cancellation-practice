< push 지울 때 >
1. `$ git reset --mixed (commit ID)`
  * soft, hard도 있긴 하지만 soft는 add된 상태로 되돌려줘서 불편하고 hard는 위험하다
2. `$ git add (새로 넣을 파일)`
3. `$ git commit -m ""`
  * 여기서 만약 commit 이름 잘못 했으면
  `$ git commit --amend`
4. git push
  * 에러 뜨면 `$ git push -f origin master`

***
gitlab에서도 이거랑 똑같이 했는데, 내 로컬 저장소에서는 지워지고 원격 저장소에서는 그대로 남아있었다.
계속 해보다가 원격 저장소에 있는 파일 지우기를 성공했는데, commit이 되돌아간 게 아니라 새로 쌓였다.
뭐가 문제인지 아직 모르겠다.
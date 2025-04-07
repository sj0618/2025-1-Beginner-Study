#### git log
log를 사용하면 commit 기록을 최신순으로 확인한다 
commit id 라는게 있는데 거의 중복 안됨. 

## HEAD 
head는 현재작업중인 위치를 알려준다.  
현재 작업중인 브랜치의 가장 최근 commit = head  
다음 commit 의 베이스임.  
새로운 coomit이 생기면 head 도 변경  

## git status
세가지 상태가 있어요. 
# commit --amend
vim으로 진입해서 커밋 메시지를 수정 가능함. 마지막 commit의 내용에 변경 있을때 사용함. 새로운 commit으로 덮어씌우기.  
### 다른사람꺼 commit amend하지 않기 ###

# reset  
commit을 제거함. 밀어버림. 다른사람과 협업할때 쓰면 굉장히 골치아파짐. 
# revert 
commit을 제거하지 않고 되돌리기;  
새로운 커밋 추가 후 거기다가 고침.  안전함.

## ! [rejected]        main -> main (non-fast-forward)
이런 오류가 자꾸 뜨는데 , 
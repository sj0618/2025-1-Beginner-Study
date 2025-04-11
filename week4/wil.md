#### 마지막 시간이에요 ㅠ
### 복습. 
다른사람 커밋을 amend하지 않기. 
reset. commit 제거에 사용.  
revert: commit을 제거하지 않고 복구함.  

### 오늘 할거.
### 브랜치 전략.
서로의 작업에 영향주지않기 위해 브랜치를 분리해서 사용해야함.  
main브랜치를 건드리지 않는게 목표.  
# 브랜치 보호 규칙.   
승인 없이 Pull Request를 병합할 수 없도록 제한.  
= 브랜치를 안전하게 관리 .  
## git Flow 
브랜치를 관리하기위한 전략.  
메인브랜치: main(master),develop.  
서포팅브랜치: feature, release, hotfix . 
# main 브랜치
프젝 생성시 기본 브랜치, 절대 없어지지않는 브랜치 .  
# develop 브랜치
영원히 존재하는 두번째 브랜치, feature 브랜치의 기반.  
# feature
develop이랑 같이 작업함 , 기능 개발 완료 후 develop으로 흡수, 대부분의 이름으로 설정가능.  
# release
배포 준비를 위한 브랜치, 자잘한 버그를 수정하고 QA작업을 함.  (잘안쓰는듯,,)
# hotfix
긴급수정, main,develop 모두에 병합 필요.  

**git flow는 흐름이 너무 길다**

## github flow
수시로 배포되는 상황이 git flow와 어울리지 않아서 만듬.  
# main , feature
두가지 브랜치만 사용해욧 .  
# main
항상 배포 가능 상태로 유지시킴.  
병합전에 충분한 테스트 필요.  
# feature 
브랜치 구분 X. main에서 분기하여 다시 main으로 병합 .  
브랜치의 목적을 잘 생각해서 이름을 지어야함...코드리뷰가 더 중요함.  

## 그래서 뭐써야함???
**둘다 써라**
git 쓰다보면 github을 자동으로 쓸 수 있게된다..  

## **개발 attitude..**

# convention 만들어.
긴 시간이 지난 이후에도 convention 덕에 의도를 파악할 수 있다.

# **핑프짓 하지 말고 구글링 하라고**
초등학교 4학년 개발자입니다 어쩌구저쩌구

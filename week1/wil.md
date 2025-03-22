#확통
cdf, pdf, pmf 등등을 학습하였다.
cdf를 미분하면 pdf가 된다 . 

#수치해석
컴 제약을 고려하여 수치를 오차를 줄이며 계산하는 방법을 배웠다. 
1에 비해서 2^-23 은 오차가 생기지 않지만 2^-24는 오차가 생긴다.
왜냐면 IEEE754가 2^-23 까지 계산할수잇기 때문이더.


#논회
논리회로 개요: 컴퓨터의 기본 개념과 논리회로의 역할
	2.	불대수: 논리회로의 기본 이론인 불 대수의 기초, 정리와 간략화 절차
	3.	기본 논리 게이트: AND, OR, NOT, XOR, NAND, NOR, XNOR, BUFFER 등의 동작과 진리표
	4.	조합논리회로: 현재 입력에 따라 출력이 결정되는 회로
	•	가산기, 비교기, 디코더, 인코더, 멀티플렉서, 디멀티플렉서 등
	5.	순차논리회로: 현재 입력뿐만 아니라 이전 입력의 영향도 함께 받는 회로
	6.	논리회로 간소화: 카르노맵 등을 이용한 논리회로 최적화


    기본 법칙
	1.	교환법칙(Commutative Law)
	•	A + B = B + A
	•	A · B = B · A
	2.	결합법칙(Associative Law)
	•	(A + B) + C = A + (B + C) = A + B + C
	•	(A · B) · C = A · (B · C) = A · B · C
	3.	분배법칙(Distributive Law)
	•	A · (B + C) = A · B + A · C
	•	A + (B · C) = (A + B) · (A + C)
	4.	항등법칙(Identity Law)
	•	A + 0 = A
	•	A · 1 = A
	5.	무효법칙(Annulment Law)
	•	A + 1 = 1
	•	A · 0 = 0
	6.	멱등법칙(Idempotent Law)
	•	A + A = A
	•	A · A = A
	7.	보수법칙(Complement Law)
	•	A + A’ = 1
	•	A · A’ = 0
	8.	이중부정법칙(Involution/Double Negation Law)
	•	(A’)’ = A
고급 정리
	9.	드모르간의 제1정리(De Morgan’s First Theorem)
	•	(A · B)’ = A’ + B’
	10.	드모르간의 제2정리(De Morgan’s Second Theorem)
	•	(A + B)’ = A’ · B’
	11.	흡수법칙(Absorption Law)
	•	A + (A · B) = A
	•	A · (A + B) = A
	12.	합의정리(Consensus Theorem)
	•	AB + A’C + BC = AB + A’C
	•	(A + B) · (A’ + C) · (B + C) = (A + B) · (A’ + C)
	13.	중복법칙(Redundancy Law)
	•	(X + Y) · (X + Y’) = X
	•	XY + XY’ = X
	14.	쌍대성 정리(Duality Theorem)
	•	불 대수식에서 AND와 OR, 0과 1을 서로 바꾸면 다른 유효한 대수식이 된다는 정리
	•	f(X₁, X₂, …, Xₙ, 0, 1, +, ·)ᴰ = f(X₁, X₂, …, Xₙ, 1, 0, ·, +)


GIT 사용법

기본 설정 및 시작하기
	•	git init: 새로운 Git 저장소를 초기화합니다
	•	git clone URL: 원격 저장소를 로컬에 복제합니다
	•	git config –global user.name “이름”: Git 사용자 이름을 설정합니다
	•	git config –global user.email “이메일”: Git 이메일을 설정합니다
변경사항 작업
	•	git status: 작업 디렉토리의 상태를 확인합니다
	•	git add 파일명: 특정 파일의 변경사항을 스테이징 영역에 추가합니다
	•	git add .: 모든 변경사항을 스테이징 영역에 추가합니다
	•	git commit -m “메시지”: 스테이징된 변경사항을 설명과 함께 커밋합니다

원격 저장소 작업
	•	git remote -v: 원격 저장소를 나열합니다
	•	git remote add 이름 URL: 새 원격 저장소를 추가합니다
	•	git push 원격이름 브랜치명: 로컬 커밋을 원격 저장소에 푸시합니다
	•	git pull 원격이름 브랜치명: 원격 저장소의 변경사항을 가져와 병합합니다
	•	git fetch 원격이름: 병합하지 않고 원격 저장소에서 새 커밋을 가져옵니다      
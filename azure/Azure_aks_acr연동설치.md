# ACR 연동해서 AKS 설치

1. azure container registry(ACR) 생성 (mbioStudyGroup내에)
![Alt text](../images/aks_acr1.png)

2. ACR에 로그인
![Alt text](../images/aks_acr2.png)

3. Login 되어있는 ACR 확인
![Alt text](../images/aks_acr3.png)

4. ACR 서버명으로 도커 이미지 만들고 push 테스트 (mbiostudyregistry.azurecr.io)
![Alt text](../images/aks_acr4.png)

5. AKS와 ACR의 연동을 위한 service principal 생성
![Alt text](../images/aks_acr5.png)

6. 만들어 놓은 ACR (도커 레지스트리) id 추출 -> AKS랑 연동하기 위해 필요
![Alt text](../images/aks_acr6.png)

7. 생성할 AKS에서 만들어 놓은 ACR에서 도커 이미지 땡길수 있게 role 생성
![Alt text](../images/aks_acr7.png)

8. service-principal 정보를 추가해 AKS 클러스터 생성
![Alt text](../images/aks_acr8.png)

9. kubectl 설치
![Alt text](../images/aks_acr9.png)

10. 클러스터 정보 로컬에 설치
![Alt text](../images/aks_acr10.png)

참고 : https://docs.microsoft.com/ko-kr/azure/aks/tutorial-kubernetes-prepare-app
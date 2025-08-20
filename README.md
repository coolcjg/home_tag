home_tag

1. 프로젝트 소개
   - home프로젝트를 AWS와 CI/CD연동을 하기 위한 버전관리 소스
  
2. CI/CD절차
   - home프로젝트에 커밋이 될 경우 Github Action에 의해, kustomization.yaml파일의 newTag값이 변경
   - AWS EKS의 ArgoCD가 현재 레포지토리의 kustomization.yaml파일의 변경된것을 조회하여 docker이미지를 재배포한다.

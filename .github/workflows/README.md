# Backend DevSecOps

## SonarQube
- [SonarQube 개념1](https://techblog.tabling.co.kr/%EA%B8%B0%EC%88%A0%EA%B3%B5%EC%9C%A0-%EC%A0%95%EC%A0%81-%EC%BD%94%EB%93%9C-%EB%B6%84%EC%84%9D-sonarqube-6b59fa9b6b85)
- [SonarQube 개념2](https://brunch.co.kr/@joypinkgom/207)

### Clean Code Attribute
<p align="center">
![image](https://github.com/user-attachments/assets/e27a23f0-79d2-4b1d-bdc3-9e75349dfaf9)
</p>
[SonarQube Docs](https://docs.sonarsource.com/sonarqube/latest/user-guide/clean-code/definition/)
- **Consistency** (일관성)
   - 코드 스타일, 명명 규칙, 패턴 등이 일관되지 않은 부분
   
- **Intentionality** (의도성)
   - 의도성 문제는 코드가 무엇을 하는지 논리적으로 명확하지 않거나, 코드의 목적과 사용 의도가 불명확한 부분을 포함

- **Adaptability** (적응성)
   - 코드가 확장이나 재사용 가능한 구조인지 그리고 변화하는 요구 사항이나 환경에 적절하게 대응하지 못하는 부분을 포함
   
- **Responsibility** (책임)
   - 데이터와 사용자의 신뢰를 보장하고 있는지

### Software Quality
<p align="center">
![image](https://github.com/user-attachments/assets/35cd5c62-2d8b-4902-86f0-f787ab1dc78a)
[SonarQube Docs](https://docs.sonarsource.com/sonarqube/latest/user-guide/clean-code/software-qualities/)
</p>
- **Securtiy**
   - 무단 접근, 사용, 또는 파괴로부터 보호되는 정도입니다. 이는 소프트웨어의 기밀성, 무결성, 가용성을 보장하는 것
- **Reliability**
   - 특정 조건 하에서 특정 기간 동안 성능을 유지할 수 있는 능력입니다. 이는 소프트웨어가 예상대로 작동하며 오류가 발생하지 않는 정도
- **Maintainability**
   - 코드를 수리, 개선, 이해하기 쉬운 정도를 나타냅니다. 이는 코드의 수정 및 개선이 용이하고, 새로운 기능 추가나 버그 수정을 쉽게 할 수 있는지

### Issue Type
<p align="center">
![image](https://github.com/user-attachments/assets/4bab669d-1250-4f86-8c6b-a1070ca66446)
</p>
- Bug
   - Domain: Reliability
   - 코드가 잘못 작동하게 만들거나 예기치 않은 동작
   - 반드시 해결해야함
- Vulnerability
   - Domain: Security
   - 보안 위험을 초래할 수 있는 문제 - 보안 취약점 
- Code Smell
   - Domain: Maintainability
   - 코드의 가독성, 이해도, 유지보수성을 떨어뜨리는 요소

### Issues
<p align="center">
![Screenshot from 2024-08-09 12-19-34](https://github.com/user-attachments/assets/ca8cc26b-c4be-46de-bc50-d4e9b444474d)
</p>

## CVE
- [CVE 개념](https://www.redhat.com/ko/topics/security/what-is-cve)
- [US Cert](https://www.cisa.gov/news-events/bulletins)

## Trivy 
### Install Trivy
<p align="center">
![Screenshot from 2024-08-09 11-33-10](https://github.com/user-attachments/assets/b5c77b96-df1b-4daa-b0ab-5b0f01ea7e77)
</p>
### Image Scan
<p align="center">
![Screenshot from 2024-08-09 11-35-54](https://github.com/user-attachments/assets/67c9d9d6-806d-4f7f-a2dd-4cc85ded7818)
</p>
### Column
- **LIBRARY**
   - 이미지에 포함된 라이브러리나 패키지

- **VULNERABILITY ID**
   - 취약점 식별 ID

- **SEVERITY**
   - 심각도
   - **UNKNOWN** : 심각도를 알 수 없음
   - **LOW** : 낮은 위험 수준
   - **MEDIUM** : 중간 위험 수준
   - **HIGH** : 높은 위험 수준
   - **CRITICAL** : 매우 높은 위험 수준, 즉시 해결 필요

- **INSTALLED VERSION**
   - 설치 버전 

- **FIXED VERSION**
   - 수정된 버전

**TITLE**
   - 간단 설명 

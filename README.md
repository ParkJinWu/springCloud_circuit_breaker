# Microservice Architecture(MSA)
### Resilience4j를 활용한 서킷 브레이커의 상태 변화와 Fallbck 메커니즘 확인

----

- **@PathVariable 어노테이션**을 사용하여 변수(id)를 받아, 지정한 ID라면 Fallback가 호출되도록 로직 구성.


- 서킷 브레이커의 동작 확인


- 서킷 브레이커의 상태 변화 확인
![서킷 브레이커의 상태](https://github.com/user-attachments/assets/7deb97a4-595d-458e-9c19-503fdeee328e)
> 1. 서킷 브레이커의 상태: **Close** ➡️ **Open** 변환 확인
> 2. **Open**상태에서의 모든 요청 실패 확인
> 3. **Open** ➡️ **Half-Open**을 통한 시스템의 복구 여부 확인
> 4. **Half-Open**에서 성공 요청 시 **Close**상태로의 변환 확인




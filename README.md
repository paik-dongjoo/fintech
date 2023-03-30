# fintech Project

<h3> 🔥 Goal </h3>
<ul>
  <li> 간소화시킨 절차를 통해 사용자가 대출심사를 요청하고 그에 대한 결과를 확인하는 API 서비스 개발 </li>
</ul>

<h3> 📌 Summary </h3>
<img width="986" alt="스크린샷 2023-03-30 오후 12 25 35" src="https://user-images.githubusercontent.com/113086103/228720960-a31a1203-55e4-4687-8e57-de6f339bcf49.png">

<h3> 📚 Tech Stack </h3>

<div align="center">
	<img src="https://img.shields.io/badge/Spring%20Boot-32cd32?style=flat&logo=Spring%20Boot&logoColor=white" />
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=Kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-9400d3?style=flat&logo=JPA&logoColor=white" />
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat&logo=Apache%20Kafka&logoColor=white" />
	<img src="https://img.shields.io/badge/nginx-009639?style=flat&logo=NGINX&logoColor=white" />
  <img src="https://img.shields.io/badge/JUnit5-84B135?style=flat&logo=JUnit5&logoColor=white" />	
  <img src="https://img.shields.io/badge/Swagger-151F5D?style=flat&logo=Swagger&logoColor=white" />	
  <br>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=MySQL&logoColor=white" />	
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=Redis&logoColor=white" />	
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=Docker&logoColor=white" />	
</div>

<h3> 📜 Final Implementation List </h3>

1. 대출 심사 요청 : {domain}/fintech/api/v1/review  <br>
<ul>
  <li> val userRegistrationNumber: String, </li>
  <li> val userName: String, </li>
  <li> val userIncomeAmount: Long </li>
  <br>
  <li> val userKey: String </li>
</ul>
<br>

2. 대출 결과 요청 : {domain}/fintech/api/v1/result/{userKey}  <br>
<ul>
  <li> val userKey: String </li>
  <br>
  <li> data class LoanResultResponseDto(
    val userKey: String,
    val loanResult: LoanResult
    )
  </li>
  <li> data class LoanResult(
    val userLimitAmount: Long,
    val userLoanInterest: Double
    ) </li>
  
</ul>



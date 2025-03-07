<template>
  <div>
    <h1>회사 소개</h1>
    <p>저희는 2010년에 설립된 IT 솔루션 전문 기업으로, 고객의 성공을 최우선으로 생각합니다.</p>
    <h2>우리의 팀</h2>
    <div class="team">
      <div class="member">
        <img src="https://via.placeholder.com/150" alt="팀원 1" />
        <p>홍길동 - CEO</p>
      </div>
      <div class="member">
        <img src="https://via.placeholder.com/150" alt="팀원 2" />
        <p>김철수 - CTO</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.team {
  display: flex;
  gap: 1rem;
}
.member {
  text-align: center;
}
</style>
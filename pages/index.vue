<template>
  
  
  <div>
    <h1>환영합니다!</h1>
    <ServiceCard 
      title="웹 개발" 
      description="최신 기술을 활용한 맞춤형 웹사이트 제작" 
    />
    <ServiceCard 
      title="모바일 앱" 
      description="안드로이드와 iOS 모두 지원하는 앱 개발" 
    />
  </div>
  <div>
    <h1>환영합니다!</h1>
    <p>저희는 여러분의 꿈을 현실로 만드는 혁신적인 서비스를 제공합니다.</p>
    <img src="https://via.placeholder.com/800x400" alt="메인 이미지" />
    <h2>우리의 서비스</h2>
    <ul>
      <li>웹 개발: 최신 기술로 빠르고 멋진 웹사이트 제작</li>
      <li>모바일 앱: 안드로이드와 iOS 모두 지원</li>
      <li>클라우드 솔루션: 안전하고 확장 가능한 데이터 관리</li>
    </ul>
    <h2>고객 후기</h2>
    <blockquote>
      "정말 빠르고 친절한 서비스였어요. 강력 추천합니다!" - 고객 A
    </blockquote>
  </div>
  <div>
    <section>
      <h2>소개</h2>
      <img src="~/assets/welcome.jpg" alt="환영 이미지" style="max-width: 100%; height: auto;" />
      <p>Sunbind는 세상을 바꾸는 멋진 아이디어를 실현하는 회사예요. 기술과 열정으로 가득 찬 팀이 여러분을 기다리고 있습니다!</p>
    </section>
    <!-- 나머지 섹션 -->
    <!-- 소개 섹션 -->
    <section>
      <h2>소개</h2>
      <p>Sunbind는 세상을 바꾸는 멋진 아이디어를 실현하는 회사예요. 기술과 열정으로 가득 찬 팀이 여러분을 기다리고 있습니다!</p>
    </section>

    <!-- 서비스 섹션 -->
    <section>
      <h2>우리의 서비스</h2>
      <ul>
        <li>최신 트렌드에 맞춘 웹사이트 제작</li>
        <li>사용자 친화적인 모바일 앱 개발</li>
        <li>빠르고 안전한 클라우드 서비스</li>
        <li>미래를 예측하는 AI 솔루션</li>
      </ul>
    </section>

    <!-- 팀 섹션 -->
    <section>
      <h2>우리 팀</h2>
      <p>저희는 개발자, 디자이너, 꿈꾸는 사람들로 이루어진 팀이에요. 매일 새로운 도전을 즐기며 성장하고 있습니다.</p>
    </section>

    <!-- 연락처 섹션 -->
    <section>
      <h2>연락처</h2>
      <p>궁금한 게 있으면 언제든 <a href="mailto:hello@sunbind.com">hello@sunbind.com</a>으로 연락 주세요!</p>
    </section>
    
  </div>
</template>

<script>
import Section from '~/components/Section.vue';

export default {
  components: {
    Section,
  },
};
</script>

<style>
ul {
  list-style-type: square;
  margin-left: 1.5rem;
}

a {
  color: #3498db;
  text-decoration: none;
}
</style>


<style>
section {
  margin-bottom: 2rem;
  padding: 1rem;
  background-color: #f5f5f5;
  border-radius: 10px;
}

h2 {
  color: #2c3e50;
}

ul {
  list-style-type: square;
  margin-left: 1.5rem;
}

a {
  color: #3498db;
  text-decoration: none;
}
</style>
<template>
  <section class="event-card">
    <!-- LEFT SIDE -->
    <div class="left-panel">
      <div class="content">
        <h2>Panel Discussion</h2>
        <h1>
          THE FUTURE OF <span class="highlight">FUNDRAISING</span><br />
          IN VIETNAM
        </h1>

        <div class="event-info">
          <p>
            <strong>DATE & TIME</strong><br />
            WEDNESDAY<br />
            MAY 7TH 2025<br />
            6PM - 9:30PM
          </p>
          <p>
            <strong>LOCATION</strong><br />
            THE SENTRY SAIGON<br />
            Sonatus Building, 15 Le Thanh Ton,<br />
            Ben Nghe, District 1, HCMC
          </p>
          <p>
            <strong>TICKET:</strong> 200,000 VND<br />
            <small>Includes welcome drink</small>
          </p>
        </div>

        <div class="main-content">
  <div class="speaker-section">
    <h3>SPEAKERS</h3>
    <div class="speakers">
      <div class="speaker">
        <img src="@/assets/VN is awesome/nguyen.jpg" alt="Charles Phan" />
        <p class="name">SHARK LOUIS NGUYEN</p>
        <p class="title">Chairman and CEO, Saigon Asset Management (SAM)</p>
      </div>
      <div class="speaker">
        <img src="@/assets/VN is awesome/phuong.jpg" alt="Phuong Trieu" />
        <p class="name">MS. PHUONG TRAN</p>
        <p class="title">Principal, Wavemaker Partners Vietnam and SEA</p>
      </div>
      <div class="speaker">
        <img src="@/assets/VN is awesome/GISZ.jpg" alt="Justin Gisz" />
        <p class="name">MR. JUSTIN GISZ</p>
        <p class="title">Partner at Asia Counsel Vietnam</p>
      </div>
      <div class="speaker">
        <img src="@/assets/VN is awesome/PAOLO.jpg" alt="Paolo" />
        <p class="name">MR. PAOLO MARCO RESTITUTO</p>
        <p class="title">Senior BD Manager, Frasers Law Company</p>
      </div>
      <div class="speaker">
        <img src="@/assets/VN is awesome/DICKENS.jpg" alt="Mark" />
        <p class="name">MARK DICKENS</p>
        <p class="title">Saigon Young Professionals (SYP) Founder</p>
      </div>
    </div>
  </div>
</div>

        <div class="sponsor-logos">
  <img src="@/assets/VN is awesome/dau.jpg" alt="Vietkieu logo" />
  <img src="@/assets/VN is awesome/2.jpg" alt="Vietnam is Awesome logo" />
  <img src="@/assets/VN is awesome/3.jpg" alt="The Sentry logo" />
  <img src="@/assets/VN is awesome/4.jpg" alt="Bananas for Peace logo" />
  <img src="@/assets/VN is awesome/5.jpg" alt="Mixtape logo" />
</div>


      </div>
    </div>

    <!-- RIGHT SIDE -->
    <div class="right-panel">
  <ul class="topics">
    <li>
      Investment Trends
      <span class="desc">Understanding the current funding climate in Vietnam</span>
    </li>
    <li>
      Types of Funding
      <span class="desc">Angel investors, venture capital, institutional funding</span>
    </li>
    <li>
      Investor Expectations
      <span class="desc">What investors look for, financial projections, traction</span>
    </li>
    <li>
      Pitching & Negotiation
      <span class="desc">How to pitch compellingly and secure funding</span>
    </li>
    <li>
      Success Stories & Pitfalls
      <span class="desc">Real-life case studies and lessons from the field</span>
    </li>
  </ul>
</div>

  </section>
</template>

<script>
export default {
  name: 'EventCard'
}
</script>

<style scoped>
.event-card {
  background-color: black;
  color: white;
  padding: 60px 30px;
  text-align: left;
  font-family: 'Helvetica Neue', Arial, sans-serif;
  min-height: 100vh;
  display: flex;
  align-items: flex-start;
  justify-content: center;
}



.content {
  max-width: 1000px;
  width: 100%;
}

h1 {
  font-size: 70px; /* Giữ kích thước chữ ban đầu */
  font-weight: 600; /* Đổi từ 800 sang 300 để làm chữ mỏng lại */
  line-height: 1.2; /* Giữ chiều cao dòng như cũ */
  letter-spacing: 10px; /* Tăng khoảng cách giữa các ký tự */
  margin: 20px 0;
  white-space: nowrap; /* Ngăn không cho chữ xuống dòng */
  width: 100%; /* Đảm bảo chữ chiếm toàn bộ chiều rộng màn hình */
}

.highlight {
  color: yellow;
  font-weight: 20; 
  font-style: italic;
  display: inline-block;
  text-transform: uppercase; /* Làm chữ in hoa để nổi bật hơn */
  transform: skewX(-10deg)
}

h2 {
  font-size: 18px;
  font-weight: normal;
  color: #cccccc;
}

.event-info {
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  gap: 20px;
  font-size: 16px;
}

.event-info strong {
  color: #ffffff;
}

.event-info small {
  font-size: 13px;
  color: #cccccc;
}

.speaker-section {
  text-align: center;
  max-width: 1100px;
  margin: 0 auto;
  margin-top: -370px; 
  position: relative;   /* Bắt buộc để left hoạt động */
  Right: -260px;  
}

.speaker-section h3 {
  font-size: 24px;
  color: #e6e4de;
  text-transform: uppercase;
  margin-bottom: 30px;
  position: relative; /* Đặt position để left hoạt động */
  Right: 320px; /* Dịch chuyển phần tử 50px sang trái */
}


/* Dùng Grid cho 3 hình trên – 2 hình dưới */
.speakers {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center;
}



.speaker {
  width: 160px;
  text-align: center;
}

.speaker img {
  width: 90px;
  height: 90px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 10px;
}

.speaker .name {
  font-size: 14px;
  font-weight: bold;
  color: #ffcc00;
  margin-bottom: 5px;
  text-transform: uppercase;
}

.speaker .title {
  font-size: 13px;
  color: #ffffff;
  line-height: 1.3;
}

/* Speaker 4: nằm thẳng hàng dưới Speaker 3 (cột 3) */
.speaker:nth-child(4) {
  grid-column: 3;
  grid-row: 2;
}

/* Speaker 5: nằm xéo (lệch trái) hình 3 (cột 2) */
.speaker:nth-child(5) {
  grid-column: 2;
  grid-row: 2;
  transform: translateX(30px);
}

.topics {
  list-style: none;
  padding: 70px;
  position: relative;
  right: -90px; /* Di chuyển sang phải */
}

.topics li {
  font-size: 26px;
  margin-bottom: 50px;
  font-weight: 500;
  padding-left: 10px;
  font-weight: bold;
}
.right-panel {
  text-align: center;
  color: white;
  font-family: Arial, sans-serif;
  padding: 50px 20px;
  margin-top: 250px;
}
.topics li {
  margin-bottom: 24px;
  font-size: 18px;
  font-weight: bold;
}

.topics li .desc {
  display: block;
  font-size: 14px;
  color: #ccc;
  margin-top: 8px;
  font-weight: normal;
  line-height: 1.4;
}
.sponsor-logos {
  margin-top: 50px;
  padding-top: 30px;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 40px;
  flex-direction: row;
  text-align: center;
}

.sponsor-logos span {
  color: white;
  opacity: 0.9;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 1px;
}

/* Kiểu riêng cho từng logo chữ */
.vietkieu {
  font-family: 'Arial Black', sans-serif;
  text-transform: uppercase;
}

.awesome {
  font-family: 'Brush Script MT', cursive;
  font-size: 18px;
  font-style: italic;
}

.sentry {
  font-family: 'Helvetica', sans-serif;
  font-weight: bold;
  font-size: 15px;
}

.bananas {
  font-family: 'Courier New', monospace;
  font-weight: bold;
  text-transform: uppercase;
}

.mixtape {
  font-family: 'Impact', sans-serif;
  font-size: 16px;
  text-transform: uppercase;
}




</style>
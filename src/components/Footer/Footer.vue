<template>
    <footer class="footer">
      <div class="footer-content">
        <div class="footer-text">
          <h2>PISTONS</h2>
          <h3>STAY CONNECTED</h3>
        </div>
        <div class="social-icons">
          <a href="#" class="icon">
            <img src="@/images/facebook.png" alt="Facebook">
          </a>
          <a href="#" class="icon">
            <img src="@/images/youtube.png" alt="YouTube">
          </a>
          <a href="#" class="icon">
            <img src="@/images/instagram.png" alt="Instagram">
          </a>
          <a href="#" class="icon">
            <img src="@/images/twitter.png" alt="Twitter">
          </a>
          <a href="#" class="icon">
            <img src="@/images/mail.png" alt="Mail">
          </a>
        </div>
      </div>
    </footer>
  </template>
  
  <style scoped>
  .footer {
    background-color: #000;
    width: 100%;
    /* height: 254px; */
    padding: 26px 0 53px 0;
    color: #fff;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  
  .footer-content {
    text-align: center;
  }
  
  .footer-text {
    text-align: center;
  }
  
  .footer-text h2 {
    font-size: 24px;
    margin: 0;
    font-weight: 500;
  }
  
  .footer-text h3 {
    font-size: 18px;
    margin: 0;
    font-weight: 400;
  }
  
  .social-icons {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .icon {
    margin: 0 10px;
  }
  
  .icon img {
    width: 24px;
    height: 24px;
    cursor: pointer;
  }
  
  .icon img:hover {
    opacity: 0.8;
  }
  </style>
  
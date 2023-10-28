<template>
    <h2 class="heading">Testimonials</h2>
    <div
      class="container1"
      @mouseenter="hovering = true"
      @mouseleave="hovering = false"
    >
      <div class="overlay" :class="{ active: hovering }">
        <div class="items" style="padding: 10%">
            I stumbled upon this shop, and their selection blew me away. The user-friendly website made my shopping experience a breeze!
        </div>
      </div>
    </div>
    <div
      class="container2"
      @mouseenter="hovering = true"
      @mouseleave="hovering = false"
    >
      <div class="overlay" :class="{ active: hovering }">
        <div class="items" style="padding: 10%">
            The checkout process was seamless, and the responsive design worked flawlessly on my mobile device. I'll definitely be coming back!
        </div>
      </div>
    </div>
    <div
      class="container3"
      @mouseenter="hovering = true"
      @mouseleave="hovering = false"
    >
      <div class="overlay" :class="{ active: hovering }">
        <div class="items" style="padding: 10%">
            Their site's intuitive navigation made finding the perfect pen a joy. Five stars for both their products and web design!
        </div>
      </div>
    </div>
    <div
      class="container4"
      @mouseenter="hovering = true"
      @mouseleave="hovering = false"
    >
      <div class="overlay" :class="{ active: hovering }">
        <div class="items" style="padding: 10%">
            I appreciate the attention to detail in both their pens and website. A visually stunning and user-focused online shop.
        </div>
      </div>
    </div>


  </template>
  
  <script>
  export default {
    data() {
      return {
        hovering: false,
      };
    },
  };
  </script>
  
  <style scoped>
  .heading{
    text-align: center;
    /* width: 342px; */
    height: 45px;
    top: 38px;
    left: 549px;
    font-family: Oxygen;
    font-size: 36px;
    font-weight: 700;
    line-height: 45px;
    letter-spacing: 0.22em;
    
  }
  .container1 {
    display: inline-block;
    z-index: 5;
    width: 277px;
    height: 277px;
    right: 0;
    left: 0;
    bottom: 0;
    margin: 2%;
    background: url("C:\Users\advai\Desktop\project\pistons\src\images\Alex.png");
    background-color: black;
    background-size: cover;
    cursor: pointer;
    -webkit-box-shadow: 0 0 5px #000;
    box-shadow: 0 0 5px #000;
    border-radius: 25px;
  }
  .container2 {

    display: inline-block;
    z-index: 5;
    width: 277px;
    height: 277px;
    right: 0;
    left: 0;
    bottom: 0;
    margin: 2%;
    background: url("C:\Users\advai\Desktop\project\pistons\src\images\Emily.png");
    background-color: black;
    background-size: cover;
    cursor: pointer;
    -webkit-box-shadow: 0 0 5px #000;
    box-shadow: 0 0 5px #000;
    border-radius: 25px;
  }
  .container3 {

display: inline-block;
z-index: 5;
width: 277px;
height: 277px;
right: 0;
left: 0;
bottom: 0;
margin: 2%;
background: url("C:\Users\advai\Desktop\project\pistons\src\images\David.png");
background-color: black;
background-size: cover;
cursor: pointer;
-webkit-box-shadow: 0 0 5px #000;
box-shadow: 0 0 5px #000;
border-radius: 25px;
}
.container4 {

display: inline-block;
z-index: 5;
width: 277px;
height: 277px;
right: 0;
left: 0;
bottom: 0;
margin: 2%;
background: url("C:\Users\advai\Desktop\project\pistons\src\images\Lisa.png");
background-color: black;
background-size: cover;
cursor: pointer;
-webkit-box-shadow: 0 0 5px #000;
box-shadow: 0 0 5px #000;
border-radius: 25px;
}
  
  .overlay {
    border-radius: 25px;
    width: 100%;
    height: 100%;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 2fr 2fr 1fr;
    background: rgba(77, 77, 77, 0.9);
    color: #fef5df;
    opacity: 0;
    transition: all 0.5s;
    font-family: "Playfair Display", serif;
  }
  
  .items {
    padding-left: 20px;
    letter-spacing: 3px;
  }
  
  .head {
    font-size: 30px;
    line-height: 40px;
    transform: translateY(40px);
    transition: all 0.7s;
  }
  
  .head hr {
    display: block;
    width: 0;
    border: none;
    border-bottom: solid 2px #fef5df;
    position: absolute;
  
    bottom: 0;
    left: 20px;
    transition: all 0.5s;
  }
  
  .price {
    font-size: 22px;
    line-height: 10px;
    font-weight: bold;
    opacity: 0;
    transform: translateY(40px);
    transition: all 0.7s;
  }
  
  .price .old {
    text-decoration: line-through;
    color: lighten(rgb(77, 77, 77), 40%);
  }
  
  .cart {
    font-size: 12px;
    opacity: 0;
    letter-spacing: 1px;
    font-family: "Lato", sans-serif;
    transform: translateY(40px);
    transition: all 0.7s;
  }
  
  .cart i {
    font-size: 16px;
  }
  
  .cart span {
    margin-left: 10px;
  }
  
  .container:hover .overlay {
    opacity: 1;
  }
  
  .container:hover .overlay .head {
    transform: translateY(0px);
    transition-delay: 0.4s;
  }
  
  .container:hover .overlay .head hr {
    width: 75px;
    transition-delay: 0.4s;
  }
  
  .container:hover .overlay .price {
    transform: translateY(0px);
    transition-delay: 0.3s;
    opacity: 1;
  }
  
  .container:hover .overlay .cart {
    transform: translateY(0px);
    transition-delay: 0.6s;
    opacity: 1;
  }
  
  .overlay.active {
    opacity: 1;
    background-image: none;
    background-color: black;
  }
  
  .overlay.active .head {
    transform: translateY(0px);
    transition-delay: 0.4s;
  }
  
  .overlay.active .head hr {
    width: 75px;
    transition-delay: 0.4s;
  }
  
  .overlay.active .price {
    transform: translateY(0px);
    transition-delay: 0.3s;
    opacity: 1;
  }
  
  .overlay.active .cart {
    transform: translateY(0px);
    transition-delay: 0.6s;
    opacity: 1;
  }
  </style>
  
  <!-- {
    "testimonials": [
      {
        "name": "Alex P.",
        "message": "I stumbled upon this shop, and their selection blew me away. The user-friendly website made my shopping experience a breeze!",
        "image": "https://i.ibb.co/vmYY6tY/img1.png"
      },
      {
        "name": "Emily S.",
        "message": "The checkout process was seamless, and the responsive design worked flawlessly on my mobile device. I'll definitely be coming back!",
        "image": "https://i.ibb.co/k29V4KN/img2.png"
      },
      {
        "name": "David R.",
        "message": "Their site's intuitive navigation made finding the perfect pen a joy. Five stars for both their products and web design!",
        "image": "https://i.ibb.co/Mcz1SWT/img3.png"
      },
      {
        "name": "Lisa M.",
        "message": "I appreciate the attention to detail in both their pens and website. A visually stunning and user-focused online shop.",
        "image": "https://i.ibb.co/94fW8xZ/img4.png"
      }
    ]
  } -->
  

<template>
<div>
  
  <div id="navbar">
    <div id="free-shipping-bar">
        Free Shipping On All Orders
    </div>

    <div class="navbar-container">
  
    <div id="brand">{{ brandName }}</div>

    <ul id="links">
      <li class="nav-link"><router-link to="/">NEW</router-link></li>
      <li class="nav-link"><router-link to="/brands">BRANDS</router-link></li>
      <li class="nav-link"><router-link to="/collections">COLLECTIONS</router-link></li>
      <li class="nav-link"><router-link to="/accessories">ACCESSORIES</router-link></li>
      <li class="nav-link">
        <a href="#" class="icon">
        <a href="#about">ABOUT</a>
      </a>
      </li>
    </ul>
    
    <div id="image-container">
      <img src="@/images/vector.png" alt="Vector Image">
      <a href="#" class="icon">
        <img src="@/images/magnifier.png" alt="Magnifier Image" @click="openOverlay">
      </a>
  </div>
  
  <div v-if="showSearchBar" class="search-container">
      <img src="@/images/searchbar.png" alt="Search Bar" class="search-bar">
      <a @click="closeOverlay" class="close-icon"></a>
    </div>
  
  </div>
  </div>
</div>
</template>

<script>
export default {
  data() {
    return {
      brandName: 'PISTONS',
      showSearchBar: false // showSearchBar data property
    };
  },
  methods: {
    openOverlay() {
      this.showSearchBar = true;
    },
    closeOverlay() {
      this.showSearchBar = false;
    }
  }
};
</script>
export default {
  methods: {
    openOverlay() {
    },
  },
};
<style scoped>
.close-icon {
  width: 20px;
  height: 20px;
}

/* styles for the navbar component */
#free-shipping-bar {
  background-color: gray;
  text-align: center;
  color: white; /* Text color */
  top:0;
  /* position:fixed; */
  width:100%;
  padding: 5px;
}
#navbar {
  /* display: flex; */
  justify-content: space-between;
  align-items: center; /* Vertically center the brand name */
  background-color: #fff; /* Set background to white */
  color: #000; /* Set text color to black */
  /* padding: 10px 20px; */
  width: 100%; 
  height: 83px;
  /* left: 50%; */
  /* top:41px; */
  /* transform: translateX(-50%); */
  background-color: #fff; /* Set background to white */
  color: #000; /* Set text color to black */
  z-index: 100; /* Ensure the navbar is above other content */

}

.navbar-container {
  display: flex;
}

.nav-link {
  display: flex;
  justify-content: center;
  align-items: center;
  align-self: center;
}

#navbar {
  width: 100%;
  height: 83px;
  position: relative;
  /* left: 50%; */
  /* transform: translateX(-50%); */
  background-color: #fff; /* Set background to white */
  color: #000; /* Set text color to black */
  z-index: 100; /* Ensure the navbar is above other content */
}

#brand {
  font-family: 'Pridi', sans-serif;
  font-size: 40px;
  font-weight: 400;
  line-height: 62px;
  letter-spacing: 0;
  text-align: left;
}

#navbar a {
  color: #000; /* Set text color to black */
  text-decoration: none;
  margin: 0 10px;
}

#links {
  list-style: none; /* Remove list bullets */
  display: flex; /* Display items side by side */
  justify-content: center;
  margin: 0 auto;
  padding: 0;
}

#links li {
  margin: 0 10px; /* Add spacing between list items */
}
#image-container {
  display: flex;
  align-items: center;
  margin-right: 20px; /* Adjust the margin as needed */
}

#image-container img {
  margin-left: 10px; /* Add spacing between the images */
}
.search-container {
  position: absolute;
  top: 83px; /* Adjust the top position as needed */
  right: 50px; /* Adjust the right position to move it to the right side */
  z-index: 1; /* Place it above other content */
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #fff; /* Background color for the search bar */
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  box-sizing: border-box;
}
.close-icon {
  cursor: pointer;
  position: absolute;
  top: 15px;
  left: 410px;
}
</style>

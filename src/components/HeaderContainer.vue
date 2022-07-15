<template>
  <header>
    <div id="top-bar"></div>

    <nav class="navbar navbar-expand-lg navbar-light">
      
      <div class="container">
        <div>
          <a href="https://www.dccomics.com/"><img id="logo" src="../assets/img/dc-logo.png" alt="dclogo" /></a>
        </div>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav text-uppercase">
            <a class="nav-link text-dark" href="#">Characters</a>
            <a class="nav-link text-dark" href="#">Comics</a>
            <a class="nav-link text-dark" href="#">Movies</a>
            <a class="nav-link text-dark" href="#">Tv</a>
            <a class="nav-link text-dark" href="#">Games</a>
            <a class="nav-link text-dark" href="#">Collectibles</a>
            <a class="nav-link text-dark" href="#">Videos</a>
            <a class="nav-link text-dark" href="#">Fans</a>
            <a class="nav-link text-dark" href="#">News</a>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle text-dark"
                href="#"
                id="navbarDropdown"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Shop
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li>
                  <a class="dropdown-item" href="#">Something else here</a>
                </li>
              </ul>
            </li>
          </div>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>

header {
  height: 150px;

  #top-bar {
    background-color: #212121;
    height: 20px;
  }

  nav {
    height: 130px;
    background-color: white;
    font-family: "Yanone Kaffeesatz", sans-serif;
  }

  #logo {
    width: 70px;
    height: 70px;
  }

  a,
  li {
    font-size: 17px;
    font-weight: bolder;
    padding-left:15px;
    
  }

  // .ms_container_nav {
    
  // }
}
</style>
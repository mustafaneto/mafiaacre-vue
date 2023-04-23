<script>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
<header>
    <nav class="navbar navbar-expand-md navbar-dark bg-dark">
        <div class="container-fluid container-fluid">
            <RouterLink to="/"><img class="navLogo" src="./assets/img/logo.png" alt=""></RouterLink>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse justify-content-md-between" id="navbarScroll">
                <ul class="navbar-nav my-2 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 100px;">
                    <!-- <li class="nav-item">
                        <RouterLink to="/" class="nav-link active">Home</RouterLink>
                    </li> -->
                    <li class="nav-item">
                        <RouterLink to="/historia" class="nav-link active">História</RouterLink>
                    </li>
                    <!-- <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Link
                        </a>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#">Action</a></li>
                            <li><a class="dropdown-item" href="#">Another action</a></li>
                            <li>
                                <hr class="dropdown-divider">
                            </li>
                            <li><a class="dropdown-item" href="#">Something else here</a></li>
                        </ul>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link disabled">Link</a>
                    </li> -->
                </ul>

                <form class="d-flex" role="search">
                    <input class="inputUser form-control me-2" type="search" placeholder="Fala..." aria-label="Search">
                    <button class="btn btn-outline-warning" type="submit">Pesquisar</button>
                </form>
            </div>
        </div>
    </nav>

</header>

<RouterView />

<footer>
</footer>

</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300;400;700&display=swap');

  .nav-link:hover{
    color: #ffc107;
  }
  .navLogo {
    width: 60px;
  }
  .inputUser {
    border: none;
  }
  .inputUser:focus {
    border: none;
    box-shadow: none;
  }

</style>

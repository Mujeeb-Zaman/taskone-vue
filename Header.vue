<template>
    <!-- Navigation bar start -->
        <nav class="navbar navbar-light bg-light">
        <div class="container-fluid">
          <a class="navbar-brand mx-5">Navbar</a>
          <form class="d-flex">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">Search</button>
          </form>
        </div>
        </nav>
    <!-- Navigation bar end -->
</template>

<script>
    export default{
        name: 'Header'
    }
</script>
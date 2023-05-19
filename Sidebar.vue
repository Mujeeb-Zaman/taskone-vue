<template>
    <label for="opensidebar" class="sidebartoggle"></label>

    <input type="checkbox" name="" id="opensidebar">
    <!-- Side Bar Start -->
      <div class="sidebar">
        <ul class="menu">
            <li>Home</li>
            <li>About</li>
            <li>Gallery</li>
            <li>Products</li>
            <li>Contact Us </li>
        </ul>
      </div>
    <!-- Side Bar Start -->
</template>

<script>
    export default{
        name: 'Sidebar'
    }
</script>

<style>
.sidebar{
    height: 100%;
    position: fixed;
    left: 0;
    top: 0;
    width: 250px;
    margin-top: 60px;
    background-color: #21ac21;
    transform: translateX(-250px);
    transition: transform 250ms ease-in-out;
}
.menu{
    list-style: none;
    padding: 0;
    margin: 0;
}
.menu li{
    color: #fff;
    border-bottom: 1px solid green;
}
.menu li a{
    color: #fff;
    display: block;
    text-decoration: none;
    text-transform: uppercase;
    padding: 20px;
}
.sidebartoggle{
    background: #fff;
    width: 22px;
    height: 22px;
    position: absolute;
    z-index: 1000;
    top: 22px;
    left: 15px;
    cursor: pointer;
}
#opensidebar:checked ~ .sidebar{
    transform: translateX(0px);
}

</style>
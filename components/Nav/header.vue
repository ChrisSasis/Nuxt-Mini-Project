<template>
    <div>
        <header class="header py-3 px-3 lg:px-10 relative">
            <a href="/" class="inline-block align-middle text-logo text-3xl md:text-3xl font-bold tracking-tight">Parenta</a>
            <nav class="menu hidden md:inline-block align-middle pl-5" v-bind:class="{ show : toggleMenu }">
                <ul class="md:flex">
                    <li>
                        <a href="/" class="nav-link px-3 block font-bold text-sm roboto tracking-wide">
                            Home
                        </a>
                    </li>
                    <li>
                        <a href="#" class="nav-link px-3 block font-bold text-sm roboto tracking-wide">
                            Rent
                        </a>
                    </li>
                    <li>
                        <a href="#" class="nav-link px-3 block font-bold text-sm roboto tracking-wide">
                            About
                        </a>
                    </li>
                    <li>
                        <a href="#" class="nav-link px-3 block font-bold text-sm roboto tracking-wide">
                            Contact
                        </a>
                    </li>
                    <li>
                        <a href="#" class="nav-link px-3 block font-bold text-sm roboto tracking-wide">
                            FAQ
                        </a>
                    </li>
                </ul>
            </nav>
            <div class="auth-search">
                <a href="/login" class="nav-link inline-block text-sm font-bold roboto tracking-wide pr-2">Sign In</a> <span>/</span>
                <a href="/register" class="nav-link inline-block text-sm font-bold roboto tracking-wide pl-2 pr-5 md:pr-0">Register</a>
                <button class="burger inline-block md:hidden align-middle" @click="showMenu">
                    <div class="burger-bar"></div>
                    <div class="burger-bar"></div>
                    <div class="burger-bar"></div>
                </button>
            </div>
        </header>
    </div>
</template>

<script>
export default {
    name: "headerMain",
    data() {
        return {
            toggleMenu: false,
        }
    },
    methods: {
        showMenu() {
            if(this.toggleMenu == false) {
                this.toggleMenu = true;
            } else {
                this.toggleMenu = false;
            }
        }
    }
}
</script>

<style>
.text-logo {
    color:#56D2DA;
    font-family: 'Roboto',sans-serif;
}
</style>

<style scoped>
.show {
    display: inline-block;
}
.hide {
    display: none;
}
.auth-search {
    position:absolute;
    top:50%;    
    right:2.5rem;
    transform:translateY(-50%);
}
.nav-link:hover {
    color:#56D2DA;
}
.burger {
    width:30px;
    margin-left:10px;
    outline:none;
    text-align: right;
}
.burger-bar {
    width:100%;
    height:4px;
    margin-bottom:4px;
    background:#000;
    border-radius:100px;
}
.burger-bar:nth-child(2) {
    width:80%;
    margin:4px 0px 4px auto;
}
@media screen and (max-width: 1023px) {
    .auth-search {
        right:0.75rem;
    }
}
@media screen and (max-width: 760px) {
    .menu {
        position:absolute;
        top:69px;
        left:0;
        width:100%;
        background:#fff;
        z-index: 100;
    }
    .nav-link {
        padding:1rem;
    }
}
</style>
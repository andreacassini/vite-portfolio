<script>
export default {
    data(){
        return{
            menuItems:[
                {
                    label: 'about'
                },
                {
                    label: 'skills'
                },
                {
                    label: 'projects'
                },
                {
                    label: 'contacts'
                }
            ],
            isScrolled: false
        }
    },
    created() {
        window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            this.isScrolled = window.scrollY > 20;
        },
    }  
}
</script>

<template>
    <div>
        <div class="container">
            <div class="fixed-bar" :class="{ 'scrolled': isScrolled }">
                <div class="row align-items-center justify-content-between p-1">
                    <div class="col inside">
                        <a href="#">
                            LOGO
                        </a>
                    </div>
                    <!-- NAVBAR RX -->
                    <div class="col inside">
                        <nav class="navbar navbar-expand-lg">
                            <div class="container-fluid">
                                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                                    <span class="navbar-toggler-icon"></span>   
                                </button>
                                <div class="collapse navbar-collapse justify-content-end" id="navbarTogglerDemo01">
                                    <ul class="navbar-nav ml-auto">
                                        <li class="nav-item mx-2">
                                            <a class="nav-link active" aria-current="page" href="">Home</a>
                                        </li>
                                        <li class="nav-item mx-2">
                                            <a class="nav-link" href="#about">About</a>
                                        </li>
                                        <li class="nav-item mx-2">
                                            <a class="nav-link" href="#skills">Skills</a>
                                        </li>
                                        <li class="nav-item mx-2">
                                            <a class="nav-link" href="#">Projects</a>
                                        </li>
                                        <li class="nav-item mx-2">
                                            <a class="nav-link" href="#">Contacts</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </nav>
                    </div>
                </div>
                <!-- LOGO SX -->
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .fixed-bar{
        position: fixed;
        left: 0;
        width: 100%;
        top: 0;
        background-color: transparent;
        transition: background-color 0.3s ease;
        z-index: 100;
    }

    li {
      a {
        font-size: 20px;
      }
    }

    .fixed-bar.scrolled {
        background-color: lightgray;
    }

    .inside{
        margin: 0 240px;
    }
</style>
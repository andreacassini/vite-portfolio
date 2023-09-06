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
            ]
        }
    }
}
</script>

<template>
    <div>
        <div class="container">
            <div class="fixed-bar">
                <div class="row align-items-center justify-content-between bg-secondary">
                    <div class="col">
                        <a href="#">
                            LOGO
                        </a>
                    </div>
                    <!-- NAVBAR RX -->
                    <div class="col">
                        <nav class="navbar navbar-expand-lg">
                            <div class="container-fluid">
                                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                                    <span class="navbar-toggler-icon"></span>   
                                </button>
                                <div class="collapse navbar-collapse justify-content-end" id="navbarTogglerDemo01">
                                    <ul class="navbar-nav ml-auto">
                                        <li class="nav-item">
                                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                                        </li>
                                        <li class="nav-item">
                                            <a class="nav-link" href="#">About</a>
                                        </li>
                                        <li class="nav-item">
                                            <a class="nav-link" href="#">Skills</a>
                                        </li>
                                        <li class="nav-item">
                                            <a class="nav-link" href="#">Projects</a>
                                        </li>
                                        <li class="nav-item">
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
        left: 25%;
        top: 0;
        right: 25%;
    }
</style>
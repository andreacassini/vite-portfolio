<script>
export default {
    data(){
        return{
            menuItems:[
                {
                    label: 'about'
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

<template lang="">
    <div>
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col-6">
                    <img src="../assets/logo-light-png.png" alt="logo" width="300">
                </div>
                <div class="col-6">
                    <nav class="navbar navbar-expand-lg bg-body-tertiary">
                        <div class="container-fluid">
                            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                                <span class="navbar-toggler-icon"></span>   
                            </button>
                            <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                                <li class="nav-item">
                                    <a class="nav-link active" aria-current="page" href="#">About</a>
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
        </div>
        <!-- LOGO SX -->
        
    </div>
</template>
<style lang="">
    
</style>
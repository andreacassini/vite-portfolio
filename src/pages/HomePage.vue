<script>
export default {
    name:"HomePage"
}
</script>

<template lang="">
    <div>
        <div class="container">
            <!-- JUMBOTRON -->
            <div class="row align-items-center" id="jumbotron">
                <div class="col-6">
                    <h3>Hi, my name is</h3>
                    <h1 class="fw-bold">Andrea Cassini.</h1>
                    <h4>I write <span class="fw-bold">&ltscript> </span>for the web.</h4>
                    <h5>I'm a Full-Stack Developer based in Bordighera, Italy. I enjoy 
                        learning new ways of coding keep up with technology.
                    </h5>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #jumbotron{
        height: calc(100vh - 100px);
        margin-top: 100px;
            h3{
                font-size: 50px;
            }
            h1{
                font-size: 80px;
            }
            h4{
                font-size: 40px;
                margin-bottom: 20px;
            }
            h5{
                font-size: 28px;
            }
        }

</style>
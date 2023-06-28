<template>
    <section class="bg-copy">
        <section class="my_container d-flex justify-content-between align-items-center">
            <div class="d-flex align-items-center">
                <p class="m-0">Copyright 2022 tophive. All Rights Reserved.</p>
            </div>
            <div>
                <ul class="d-flex align-items-center py-3">
                    <li>
                        <a href="#">Privacy</a>
                    </li>
                    <li><a href="#">Terms</a>
                    </li>
                    <li><a href="#">Cookie Policy</a>
                    </li>
                    <li><a href="#">Sitemap</a>
                    </li>
                </ul>
            </div>

        </section>
    </section>
</template>
<script>
export default {
    name:"Copyrights"
}
</script>
<style lang="scss" scoped>
p{
    font-size: 0.7rem;
    color: #a3b5ca;
}
ul{
    margin: 0;
    padding: 0;
}
li{
    margin-right: 1rem;
    
}
a{
    font-size: 0.8rem;
    color:#a3b5ca ;
}
a:hover{
    color: #d74d52;
}
.bg-copy{
    width: 100%;
    background-color: #15222e;
}
    
</style>
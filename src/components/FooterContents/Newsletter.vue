<template>
    <section class="newsletter d-flex justify-content-between mb-5">
        <div class="input-group my_input pt-2 ps-4 w-50 me-5 ">
                <input type="text" class="form-control rounded-0 h-50" placeholder="Subscribe to our newsletter" aria-label="" aria-describedby="basic-addon2">
                <span class="input-group-text rounded-0 bg-danger border-0 px-4 h-50" id="basic-addon2">Register</span>
        </div>
        <div class="w-50">
            <p><a href="#">Insights is Picwik </a>University's thought leadership publication for sharing knowledge on management, technology and innovation.</p>
            <a class="take-me" href="#">Take me there <i class="fa-solid fa-chevron-right me-1"></i></a>
        </div>
    </section>
</template>
<script>
export default {
    name: "Newsletter"
}
</script>
<style lang="scss" scoped>
.newsletter{
    
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}
.my_input{
    width: 40%;
    input{
        font-size: 0.8rem;
    }
    span{
        font-size: 0.8rem;
        color: white;
    }
}
    p{
        color: white;
        font-size: 0.8rem;
    }
    a{
        color:#d74d52;
        text-decoration: underline;
    }
    .take-me{
        color: white;
        font-size: small;
        font-weight: 600;
        text-decoration: none;
    }
</style>
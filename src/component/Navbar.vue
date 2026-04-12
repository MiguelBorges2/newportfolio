<script setup>

</script>
<template>
    <div class="d-flex w-100 justify-content-center tam  align-items-center">
        <ul class="nostyle w-100 d-flex justify-content-around">
            <li><p class="text-light"><span class="hash">#</span>home</p></li>
            <li><p class="text-light"><span class="hash">#</span>projetos</p></li>
            <li><p class="text-light"><span class="hash">#</span>sobre</p></li>
            <li><p class="text-light"><span class="hash">#</span>contatos</p></li>
        </ul>
    </div>
</template>
<style>
    .hash {
        color: rgba(199, 120, 221, 1);
    }
    .nostyle {
        font-size: 1vw;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
    }
    .tam {
        margin: 0;
        padding: 0;
    }
    @media(max-width: 1024px){
        .nostyle {
        font-size: 1.6vw;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
    }

    }
    @media(max-width: 600px){
        .nostyle {
        font-size: 2.5vw;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
    }
}
</style>
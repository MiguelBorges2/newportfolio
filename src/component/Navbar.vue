<script setup>

</script>
<template>
    <div class="d-flex w-100 justify-content-center tam  align-items-center">
        <ul class="nostyle w-100 d-flex justify-content-between">
            
            <a class="nem" href="#projetos"><li><p class="col"><span class="hash">#</span>projetos</p></li></a>
            <a class="nem" href="#skills"><li><p class="col"><span class="hash">#</span>skills</p></li></a>
            <a class="nem" href="#sobre"><li><p class="col"><span class="hash">#</span>sobre</p></li></a>
            <a class="nem" href="#contatos"><li><p class="col"><span class="hash">#</span>contatos</p></li></a>
            
        </ul>
    </div>
</template>
<style>
.nem {
    text-decoration: none;
}
    .hash {
        color: rgba(199, 120, 221, 1);
         margin-bottom: 0;
        margin-left: 0;
        margin-right: 0;
    }
    .nostyle {
        width: 100%;
        font-size: 1vw;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
        margin-left: 0;
        margin-right: 0;
    }
    .col {
        color: white !important;
        margin-left: 0;
        margin-right: 0;
    }
    .col:hover {
        color:  rgba(199, 120, 221, 1) !important;
    }
    .tam {
        margin: 0;
        padding: 0;
    }
    @media(max-width: 1024px){
        .nostyle {
        font-size: 1.8vh;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
    }

    }
    @media(max-width: 600px){
        .nostyle {
        font-size: 3vw;
        list-style: none;
        margin-top: 1%;
        margin-bottom: 0;
    }
}
</style>
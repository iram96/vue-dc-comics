<template>
  <div class="col-2">
      <div class="song-card ">
            <figure class="pos-rel transition-1s">
                
                <img  :src="comic.thumb" :alt="comic.series">
            </figure>
            <span class="font-white">{{ comic.series}}</span>
            <span class="font-14">{{comic.price}}</span>
        </div>
    
        
    
   
  </div>
</template>

<script>
export default {
    name: 'Content',
    props: ['comic']
}
</script>

<style>
img{
    display: block;
}

.content-div{
    background: black;
    color: white;
    min-height: 150px;
}

.ln-150{
    line-height: 150px;
}

</style>
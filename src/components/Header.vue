<template>
  <div>
      <header>
          <div  class="container">
              <div class="row-mine space-between-mine">
                  <div class="hm-col">
                <img  src="../assets/dc-logo.png" alt="">

                  </div>
                 <nav  class="hm-col align-baseline">
                <ul class="list-cl">
                     <li v-for='(item, index) in navbarList' :key='index' :class='{ active: item.active}'>
                         <a :href="item.url"  class="no-txtdec" :class="{ 'active-text': item.active}">{{item.text}}</a>
                     </li>
                     
                  
                 </ul>

              </nav>

              </div>
          </div>
      </header>
  </div>
</template>

<script>
export default {
    data(){
    return {
      navbarList: [
          {text: 'Comics', url: '#', active: false},
          {text: 'Movies', url: '#', active: false},
          {text: 'TV', url: '#', active: false},
          {text: 'Games', url: '#', active: true},
          {text: 'Collectibles', url: '#', active: false},
          {text: 'Video', url: '#', active: false},
          {text: 'Fans', url: '#', active: false},
          {text: 'News', url: '#', active: false},
          {text: 'Shop', url: '#', active: false},
          ]
    }
  }

}
</script>

<style lang='scss'>
$active_blue: dodgerblue;

img{
    
    max-height: 100%;
    max-width: 100%;
}

#logo{
    max-width: 50px;
}
header{
    max-height: 150px;
    width: 100%;
}



.hm-col{
    display: flex;
    flex-direction: column;
    
}

.list-cl{
    list-style-type: none;
    margin: 0
}

header .list-cl li{
    display: inline-block;
    margin: 10px;
    font-weight: 600;
    margin-top: 0;
    margin-bottom: 0
}
.no-txtdec{
    text-decoration: none;
    color: black
}

.active-text{
    color: $active_blue;
}

.active{
    
    border-bottom:  5px solid $active_blue;
     
}

.align-baseline{
    line-height: 150px;
    
}

</style>
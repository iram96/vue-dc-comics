<template>
  <div class="whole-footer ">
      <div class="main-footer ">
          <div class="container">
                  <div class="row-mine space-between-mine">
              <nav  class="hm-col">
                  <div class="row-mine">

                <ul class="list-cl hm-col">
                     <li><h4 class="txt-white">TITOLO</h4></li>
                     <li v-for='(item, index) in navbarList' :key='index' class=" txt-white">
                         <a :href="item.url" :class="{ 'active-text': item.active}" class="no-txtdec">{{item.text}}</a>
                     </li>
                     
                  
                 </ul>

                <ul class="list-cl hm-col">
                     <li><h4 class="txt-white">TITOLO</h4></li>
                     <li>Comics</li>
                     <li>Movies</li>
                     <li>TV</li>
                     <li>Games</li>
                     <li>Collectibles</li>
                     <li>Videos</li>
                     <li>Fans</li>
                     <li>News</li>
                     <li>Shop</li>
                  
                 </ul>

              
             
                <ul class="list-cl hm-col">
                     <li><h4 class="txt-white">TITOLO</h4></li>
                     <li>Comics</li>
                     <li>Movies</li>
                     <li>TV</li>
                     <li>Games</li>
                     <li>Collectibles</li>
                     <li>Videos</li>
                     <li>Fans</li>
                     <li>News</li>
                     <li>Shop</li>
                  
                 </ul>
                  </div>

              </nav>
          <img class="hm-col align-center" src="../assets/dc-logo-bg.png" alt="">
                  </div>

          </div>
              

              
      </div>
      <div class="side-footer">
          <div class="container h-100">
            <div class="row-mine  space-between-mine h-100">

              <div  class="hm-col align-center">
                  <div class="button">
                      SIGN-UP NOW!
                  </div>
              </div>
              <div class="hm-col  align-center">

              <div class="row-mine" > 
                <span class="clr-db  align-center">FOLLOW US</span>
                <img class="hm-col" src="../assets/footer-facebook.png" alt="">
                <img class="hm-col" src="../assets/footer-periscope.png" alt="">
                <img class="hm-col" src="../assets/footer-pinterest.png" alt="">
                <img class="hm-col" src="../assets/footer-twitter.png" alt="">
                <img class="hm-col" src="../assets/footer-youtube.png" alt="">
              </div>
              </div>
            </div>
          </div>

      </div>
  </div>
</template>

<script>
export default {
    name: 'Footer',
    
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

<style>

.whole-footer{
    height: 400px;
}

.main-footer{
    background-image: url('../assets/footer-bg.jpg');
    height: 70%;
    color: lightgray;
    overflow: hidden;
}

.side-footer{
    background: #303030;
    height: 150px;
    
}

.row-mine{
    display: flex;
    flex-direction: row;
   
}



.align-center{
    align-self:center;
    
}

.txt-white{
    color: white;
}

.button{
    border: 5px solid dodgerblue;
    line-height: 40px;
    color: white;
    
}

.clr-db{
    color: dodgerblue;
}

.va-middle{
    vertical-align: middle;
    
}

.space-between-mine{
    justify-content: space-between;
}

.h-100{
    height: 100%;
}

.side-footer img{
    margin: 0 10px;
}
</style>
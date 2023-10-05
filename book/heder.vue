<template>
        <header class=" bg-white">
        <div class="nav1 ml-2" >
            <form action="http://127.0.0.1:5500/aslo.html#" class="flex fo">
                <svg  style="margin-right: 0%;" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search mt-2.5" viewBox="0 0 16 16"> <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/> </svg>
                <input class="in" type="text" placeholder="search">
            </form>
        </div>
        <div class="nav2">
            <h1 class="fic">Online</h1>
            <h1 class="fan">Book</h1>
        </div>
        <div class="nav3 mr-2">
 <div><router-link to="/login" class="text-black">
 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 m-2">
  <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
</svg></router-link>
<div v-if="user==='t'" class="w-6 h-1  bg-violet-700 mym" style="box-shadow: -2px -2px 5px blueviolet;"></div>
</div>
       
<div>
  <router-link to="/librali" class="text-black">
  <svg xmlns="http://www.w3.org/2000/svg" fill="none" iewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 m-2 ">
  <path stroke-linecap="round" stroke-linejoin="round" d="M16.5 3.75V16.5L12 14.25 7.5 16.5V3.75m9 0H18A2.25 2.25 0 0120.25 6v12A2.25 2.25 0 0118 20.25H6A2.25 2.25 0 013.75 18V6A2.25 2.25 0 016 3.75h1.5m9 0h-9" />
</svg></router-link>
<div v-if="librali==='t'"  class="w-6 h-1 bg-violet-700 mym" style="box-shadow: -2px -2px 5px blueviolet;"></div>
</div>

<div>
  <router-link to="/fan" class="text-black">
<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 m-2">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
</svg></router-link>
<div v-if="home==='t'" class="w-6 h-1 bg-violet-700 mym" style="box-shadow: -2px -2px 5px blueviolet;"></div>
        </div>
      </div>
      
    </header>
</template>
<style scoped>
.mym{margin: 0 auto; margin-top: -7px;}
header{display: flex;
    flex-flow: row;
     justify-content: space-between;
    height:42px;
    
}
    .nav1 i{ color: gray; margin-left: 10px;}
   .in{border:solid 2px white;
     text-decoration: underline gray;
    vertical-align:middle;
    padding: 5px;
    width: 170px;
    display: inline-block;}
     .nav2{display: flex; vertical-align: middle;
     text-align: center;}
     .fic{color: gray;
       
        margin-top: 5px ; 
        font-size: 1.9rem; 
          } 
        .fan{color: blueviolet;
          margin-top: 5px;
        font-weight:500px;
        font-size: 1.9rem ; 
         }
        .nav3{ display: flex;}
        .nav3 i { margin-top: 15px;
            font-size: medium;
        margin-left: 5px;
        margin-right: 3px;
        color: gray;
        
        }
        .nav3 h2{ color: gray;font-weight: 200;}
        .nav3 img{ border-radius: 50%;
             border: solid 1px gray;
              width: 35px;
            height: 36px;
            margin-right: 15px; 
           margin-left: 200px;}
            .meno{color: rgb(61, 60, 59); 
                font-size: medium
                ;height: fit-content;
                margin-top: 10px;
            
            }

</style>
<script>




export default {
    name:'HeDer',
    props:{user:String,
        home:String,
        librali:String}
    ,
    data(){
        return{
            u:'t',
            h:'f',
            l:'t'
        }
    }
}
</script>
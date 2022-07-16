<template>
  <div class="kard-container">
    <div class="kard-bg"  v-bind:class="{ redgr: red, greengr:green, purplegr:purple }">
        <div class="kard">
            <div class="kard-icon">
                <img :src="getUrl(iconData)" alt="people">
            </div>

            <div class="kard-content">
                <h2>{{titleData}}</h2>
                <p style="text-align:start">{{textData}}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    props:{titleData:'',textData:'',iconData:'',red:false,green:false,purple:false},
    methods:{
        getUrl (img)  {
            return require(`~/assets/icons/${img}.svg`);
        }
    }
}
</script>

<style>

.purplegr{
    background-image: radial-gradient( circle farthest-corner at 10% 20%,  rgba(171,102,255,1) 0%, rgba(116,182,247,1) 90% );
}

.greengr{
    background-image: radial-gradient( circle 1259px at 2.8% 48.8%,  rgba(255,243,110,1) 0%, rgba(30,204,214,1) 45.6%, rgba(5,54,154,1) 65.9% );
}

.redgr{
    background-image: linear-gradient( 102.4deg,  rgba(253,189,85,1) 7.8%, rgba(249,131,255,1) 100.3% );
}

.kard-container{
    height: 400px;
    width: 400px;
}



.kard-bg{
    height: 300px;
    width: 300px;
    border-radius: 20px;
}

.kard{
    height: 300px;
    width: 300px;
    border-radius: 20px;
    background-color: white;
    transform: translate(50px,50px);
    box-shadow: 1px 1px 18px 1px rgba(0, 0, 0, 0.18);
    transition: 0.4s;
    cursor: pointer;
}

.kard:hover{
    transform: scale(1.2);
}

.kard-icon{
    display: flex;
    justify-content: center;
    align-items: center;
    border: 3px black solid;
    width: 70px;
    height: 70px;
    background-color: aquamarine;
    border-radius: 100rem;
    position: fixed;
    transform: translate(-20px,-20px);
}

.kard-icon img{
    width: 50px;
    height: 50px;
}

.kard-content{
    display: flex;
    flex-flow: column;
    height: 100%;
    width: 100%;
    padding-top: 50px;
    padding: 60px 10px 10px 10px;
    align-items: flex-start;
}

.kard-content h2{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 35px;
    font-weight: bolder;
    margin-bottom: 10px;
}
</style>
<template>
  <div class="kard-container" v-bind:class="{longc: long}">
    <div class="kard-bg"  v-bind:class="{ redgr: red, greengr:green, purplegr:purple, longr: long }">
        <div class="kard" v-bind:class="{longr: long}">
            <div class="kard-icon">
                <img :src="getUrl(iconData)" alt="people">
            </div>

            <div class="kard-content">
                <h2 style="text-align:start">{{titleData}}</h2>
                <p style="text-align:start">{{textData}}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    props:{titleData:'',textData:'',iconData:'',red:false,green:false,purple:false,long:false},
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
    border: 5px #ffffff solid;
    width: 70px;
    height: 70px;
    /* background-color: aquamarine; */
    /* background-image: radial-gradient( circle farthest-corner at 10% 20%,  rgba(62,133,238,1) 1.1%, rgba(227,137,240,1) 43.7%, rgba(243,193,124,1) 89.7% ); */
    background-image: linear-gradient( 103.3deg,  rgba(252,225,208,1) 30%, rgba(255,173,214,1) 55.7%, rgba(162,186,245,1) 81.8% );
    /* background-image: radial-gradient( circle farthest-corner at 10% 20%,  rgba(255,94,247,1) 17.8%, rgba(2,245,255,1) 100.2% ); */
    border-radius: 100rem;
    position: fixed;
    transform: translate(-20px,-20px);
}

.kard-icon img{
    width: 35px;
    height: 35px;
}

.kard-content{
    display: flex;
    flex-flow: column;
    height: 100%;
    width: 100%;
    padding-top: 50px;
    padding: 50px 10px 10px 10px;
    align-items: flex-start;
}

.kard-content h2{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 35px;
    font-weight: bolder;
    margin-bottom: 10px;
    text-align: start;
}

.longr{
    height: 450px;
}

.longc{
    height: 600px;
}

@media screen and (max-width: 800px){
    .kard{
        transform: translate(30px,50px);
    }

    .kard-container{
        width: 330px;
    }

}
</style>
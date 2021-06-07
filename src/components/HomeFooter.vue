<template>
<div id="homeFooter">
    <div id="footerMain1" class="rounded">
        <div id="footMain1Div1">
            <button class="btn btn-outline-secondar" id="FootText1">오시는길</button>
        </div>
    </div>
    <div id="footerMain2" class="rounded">
        <div id="footMain2Div1">
           <div id="footMain2Div2"></div>
           <button class="btn btn-danger" id="FootText2">실시간예배 바로가기</button>
        </div>
    </div>
    <div id="footerMain3" class="rounded">
        <button class="btn btn-outline-secondar" id="FootText3">오늘의말씀 Today's words</button>
        <textarea v-model="msg" class="form-control col-sm-5" id="FootText4" readonly></textarea>
    </div>
    <div id="footerMain4" class="rounded" >
        <button id="FootText5" class="btn btn-warning border border-warning" @click="openKakaoTalk">하늘영광교회 오픈카톡</button>
        <div id="kakaoTalkQRcode"><p style="margin-left:100px;width:100px;">QR코드로<br>하늘영광교회 단톡방 접속!</p></div>
       
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            msg : "너는 마음을 강하게 하고 담대히 하라 그들을 두려워 말라 그들 앞에서 떨지 말라 이는"
            + "네 하나님 여호와 그가 너와 함께 행하실것임이라 반드시 너를 떠나지 아니하시며 버리지 아니하시리라 하고 (신명기 31장 6절)"
        }
    },
    methods : {
   openKakaoTalk() {
     window.open('https://open.kakao.com/o/g9u76Ahd');
   }
 }
}
</script>


<style>
    #homeFooter {
        height:170px;
        width: 100%;
        margin-top: 600px;
    }

    #footerMain1 {
        border-style: ridge;
        margin-top: 10px;
        height:150px;
        width:400px;
        float:left;
        background-image: url("../assets/maps.png");
        background-repeat: no-repeat;
        background-size: 100% 100%;
    }

    #footerMain2 {
        border-style: ridge;
        margin-top: 10px;
        margin-left: 67px;
        height:150px;
        width:400px;
        float:left;
        background-image: url("../assets/footerPink.png");
        background-size: cover;
        background-color: #FFB6C1;

    }

    #footerMain3 {
        border-style: ridge;
        margin-top: 10px;
        margin-left: 64px;
        height:150px;
        width:400px;
        float:left;
        background-color: white;
        background-image: url("../assets/player.jpg");
        background-size: 100% 100%;
        
    }

     #footerMain4 {
        border-style: ridge;
        margin-top: 10px;
        float:right;
        height:150px;
        width:400px;
        background-color: white;
        background-image: url("../assets/kakaoTalk.png");
        background-repeat: no-repeat;
        background-size: 50% 108%;
    }

    #footMain1Div1 {
        height:148px;
        width:200px;
        margin-left:200px;
        background-image: url("../assets/wayToChurch.png");
        background-repeat: no-repeat;
        background-size: 100% 100%;
    }

    #FootText1 {
        margin-top:25px;
        margin-left:48px;
        transform: rotate(8deg);
        color:black;
        width:100px;
    }

    #footMain2Div1 {
        border-style: ridge;
        height:146px;
        width:250px;
        background-image: url("../assets/youtubeLogo.png");
        background-repeat: no-repeat;
        background-size: 100% 100%;
    }

    #FootText2 {
        margin-left:260px;
        width:120px;
    }

     #footMain2Div2 {
        height:50px;
        width:100px;
        background-image: url("../assets/youtube.png");
        background-repeat: no-repeat;
        background-size: contain;
        margin-left:250px;
    }

    #FootText3 {
        font-weight:bold;
    }

    #FootText4 {
        margin-top:10px;
        margin-left:15px;
        width:370px;
        resize:none;
        height:90px;
        font-size:0.8em;
    }

    #FootText5 {
        float: right;
        margin-right: 20px;
        margin-top:10px;
    }
    
    #kakaoTalkQRcode {
        margin-left: 182px;
        margin-top:52px;
        width: 90px;
        height: 90px;
        background-image: url("../assets/qrcode.png");
        background-repeat: no-repeat;
        background-size: 100% 100%;
    }


</style>
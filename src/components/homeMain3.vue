<template>
    <div class="main3 rounded">
        <div id="main3Title">
            <div class="bg-info" style="font-weight:bold">ל하늘영광교회 예배시간ל</div>
        </div>
        <div id="main3Body">
            <div id="main3Body1">
                <div id="main3Line"></div>
                <div style="margin-top:50px"></div>
                 <span style="color:red;margin-left:10px;font-weight:bold">주일</span>
                 <p style="margin-left:20px;font-weight:bold">주일학교:<span style="float:right;margin-right:10px;">9시30분</span></p>
                 <p style="margin-left:20px;font-weight:bold">중고등부:<span style="float:right;margin-right:10px;">9시30분</span></p>
                 <p style="margin-left:20px;font-weight:bold">연합예배:<span style="float:right;margin-right:10px;">11시00분</span></p>
                 <p style="margin-left:20px;font-weight:bold">찬양예배:<span style="float:right;margin-right:10px;">1시30분</span></p>
                 <div style="margin-top:80px"></div>
                 <span style="color:red;margin-left:10px;font-weight:bold">새벽</span>
                 <p style="margin-left:20px;font-weight:bold">새벽기도:<span style="float:right;margin-right:10px;">5시30분</span></p>
                 <div id="main3Image1" style="margin-top:30px"></div>
            </div>
            <div id="main3Body2">
                 <div id="main3Image2" style="margin-top:30px"></div>
                 <div style="margin-top:80px"></div>
                 <span style="color:red;font-weight:bold">수요일</span>
                 <p style="margin-left:10px;font-weight:bold">수요예배:<span style="float:right;margin-right:10px;">7시30분</span></p>
                 <div style="margin-top:100px"></div>
                 <span style="color:red;margin-left;font-weight:bold">금요일</span>
                 <p style="margin-left:10px;font-weight:bold">금요기도:<span style="float:right;margin-right:10px;">9시00분</span></p>
             
            </div>
        </div>
    </div>
    
</template>

<style>
    #main3Title {
        margin-top:30px;
        margin-left:30px;
        margin-right:30px;
        text-align:center;
    }

    #main3Body {
        height: 500px;
        margin-left:30px;
        margin-right:30px;
        
    }
    
    #main3Line {
        border: 1px solid #D3D3D3;
        width: 1px;
        float: right;
        height:475px;
        margin-top:15px;
    }

    #main3Body1 {

        margin-top:10px;
        width:50%;
        height:470px;
        float:left;
    }

    #main3Body2 {
    
        margin-top:10px;
        width:45%;
        height:470px;
        float:right ;
    }

    #main3Image1 {
        margin-left:40px;
        height: 100px;
        background-image: url("../assets/pray.png");
        background-repeat: no-repeat;
        background-size: contain;
    }

    #main3Image2 {
        margin-left:20px;
        height: 100px;
        background-image: url("../assets/pray2.png");
        background-repeat: no-repeat;
        background-size: contain;
    }
</style>
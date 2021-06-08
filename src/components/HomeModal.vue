<template>
    <div class="black-bg" v-if="selectData.modal">
        <div class="white-bg">
            <h4 style="text-align:center;color:#191970">{{selectData.text}}<button style="float:right;position:relative;top:-5px" class="btn btn-danger" @click="clickClose()">X</button></h4>
            <textarea v-model="selectData.content" id="homeModalText" disabled ></textarea>
  

        
        </div>
    </div>    
</template>

<script>
export default {
    props: {
        selectData : {
            type: Object,
            required: true
        }
    },
    methods : {
        clickClose() {
            this.selectData.modal = false;
        }

    }
}
</script>

<style>

.black-bg {
    left:550px;
    width:800px; height:68%;
    background: rgba(0,0,0,0,5);
    position : fixed; padding: 20px;
}

.white-bg {
    border-style: ridge;
    height:600px;
    background: white;
    border-radius: 8px;
    padding: 20px;
    background-image: url("../assets/mainbody2.png");
    background-repeat: no-repeat;
    background-size: 100% 100%;
}

#homeModalText {
    font-size:0.9em;
    font-weight:bold;
    color:#191970;
    margin-top:30px;
    margin-left:150px;
    height:447px;
    width:400px;
    resize:none;
    border-style:ridge;
    background-image: url("../assets/paper.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}
    
</style>
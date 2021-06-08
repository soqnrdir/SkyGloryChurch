<template>
    <div class="main2 rounded">
        <HomeModal :news="newsList" :selectData="selectData"/>
        <div id="main2Title" draggable="true">
            <h5 style="margin-left:10px;line-height:38px;">교회소식<button style="float:right;" class="btn btn-info">+</button></h5>
        </div>
        <ul>
            <li v-for="news in newsList" :key="news.id"  @click="newsClick(news)" @mouseover="doMouseOver()"><a class="nav-link" href="javascript:return false" rel="noopener">{{ news.text }}
                <span style="float:right;color:black">{{ news.day }}</span></a></li>

        </ul>
    </div>
</template>

<script>
import HomeModal from "@/components/HomeModal"
export default {
     components :{
        HomeModal
    },
    data() {
        return {
            selectData : {
                modal : false,
                id : 0,
                text : '',
                day : '',
                content : ''
            },
            newsList: [
                { id: 1, text: "test1" , day: '2021-06-04' ,content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 2, text: "test2" , day: '2021-06-03',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 3, text: "test3" ,day: '2021-06-03',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 4, text: "test4" ,day: '2021-06-01',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 5, text: "test5" ,day: '2021-05-31',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 6, text: "test6" ,day: '2021-04-27',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 7, text: "test7" ,day: '2021-03-25',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 8, text: "test8" ,day: '2021-03-05',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 9, text: "test9" ,day: '2021-02-15',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 10, text: "test10" ,day: '2021-01-28',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 11, text: "test11" ,day: '2021-01-12',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 12, text: "test12" ,day: '2020-12-28',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 13, text: "test13" ,day: '2020-11-15',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'},
                { id: 14, text: "test14" ,day: '2020-11-02',content:'소선민 목사가 6월 10일부터 7월 20일까지 라오스 선교에 참여합니다. 중보기도 부탁드립니다.'}

            ]
        }
    },
    methods: {
        newsClick(news) {
          this.selectData.modal = true;
          this.selectData.id = news.id;
          this.selectData.text = news.text;
          this.selectData.day = news.day;
          this.selectData.content = news.content;
        },
        doMouseOver() {
            
        }
    }
}
  
</script>

<style>
    #main2Title {
        background-color:#DCDCDC;
        height:38px;
    }
</style>
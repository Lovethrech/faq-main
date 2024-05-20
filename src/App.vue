<script setup>
import { ref } from "vue";
import quests from "@/data/quests.json";
import ChallengeAsset from "@/components/ChallengeAsset.vue";

const firstIcon = ref("<i class='bx bx-minus'></i>");
const firstAnswer = ref("flex");
const firstIconBg = ref("hsl(0, 2%, 44%)");
const secondIcon = ref("<i class='bx bx-plus'></i>");
const secondAnswer = ref("none");
const secondIconBg = ref("hsl(281, 83%, 54%)");
const thirdIcon = ref("<i class='bx bx-plus'></i>");
const thirdAnswer = ref("none");
const thirdIconBg = ref("hsl(281, 83%, 54%)");
const fourthIcon = ref("<i class='bx bx-plus'></i>");
const fourthAnswer = ref("none");
const fourthIconBg = ref("hsl(281, 83%, 54%)");

const firstIconInteract = () => {
  if (firstIcon.value === "<i class='bx bx-plus'></i>") {
    secondAnswer.value = "none";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    firstIconBg.value = "hsl(281, 83%, 54%)";
    firstAnswer.value = "flex";
    firstIcon.value = "<i class='bx bx-minus'></i>";
    firstIconBg.value = "hsl(0, 2%, 44%)";
    thirdAnswer.value = "none";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "none";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    fourthIconBg.value = "hsl(281, 83%, 54%)";
  }
}

const secondIconInteract = () => {
  if (secondIcon.value === "<i class='bx bx-plus'></i>") {
    firstAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-plus'></i>";
    firstIconBg.value = "hsl(281, 83%, 54%)";
    secondAnswer.value = "flex";
    secondIcon.value = "<i class='bx bx-minus'></i>";
    secondIconBg.value = "hsl(0, 2%, 44%)";
    thirdAnswer.value = "none";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "none";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    fouthIconBg.value = "hsl(281, 83%, 54%)";
  }
  else {
    firstAnswer.value = "flex";
    firstIconBg.value = "hsl(0, 2%, 44%)";
    secondAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-minus'></i>";
    secondIconBg.value = "hsl(281, 83%, 54%)";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    thirdAnswer.value = "none";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "none";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    fouthIconBg.value = "hsl(281, 83%, 54%)";
  }
}

const thirdIconInteract = () => {
  if (thirdIcon.value === "<i class='bx bx-plus'></i>") {
    firstAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-plus'></i>";
    firstIconBg.value = "hsl(281, 83%, 54%)";
    thirdAnswer.value = "flex";
    thirdIcon.value = "<i class='bx bx-minus'></i>";
    thirdIconBg.value = "hsl(0, 2%, 44%)";
    secondAnswer.value = "none";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    secondIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "none";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    fourthIconBg.value = "hsl(281, 83%, 54%)";
  }
  else {
    firstAnswer.value = "flex";
    firstIconBg.value = "hsl(0, 2%, 44%)";
    thirdAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-minus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    secondAnswer.value = "none";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    secondIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "none";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    fourthIconBg.value = "hsl(281, 83%, 54%)";
  }
}

const fourthIconInteract = () => {
  if (fourthIcon.value === "<i class='bx bx-plus'></i>") {
    firstAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-plus'></i>";
    firstIconBg.value = "hsl(281, 83%, 54%)";
    fourthAnswer.value = "flex";
    fourthIcon.value = "<i class='bx bx-minus'></i>";
    fourthIconBg.value = "hsl(0, 2%, 44%)";
    secondAnswer.value = "none";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    secondIconBg.value = "hsl(281, 83%, 54%)";
    thirdAnswer.value = "none";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
  }
  else {
    firstAnswer.value = "flex";
    firstIconBg.value = "hsl(0, 2%, 44%)";
    fourthAnswer.value = "none";
    firstIcon.value = "<i class='bx bx-minus'></i>";
    fourthIconBg.value = "hsl(281, 83%, 54%)";
    fourthIcon.value = "<i class='bx bx-plus'></i>";
    secondAnswer.value = "none";
    secondIcon.value = "<i class='bx bx-plus'></i>";
    secondIconBg.value = "hsl(281, 83%, 54%)";
    thirdAnswer.value = "none";
    thirdIcon.value = "<i class='bx bx-plus'></i>";
    thirdIconBg.value = "hsl(281, 83%, 54%)";
  }
}
</script>

<style scoped>
.app-main-colored{
  position:fixed;
  z-index:-1;
  width:100%;
  height:100%;
}
.app-first-color{
  background: url("/public/background-pattern-desktop.svg") hsl(292, 42%, 14%) left top/auto no-repeat;
  width:100%;
  height:30%;
}
.app-second-color{
  background-color:hsl(275, 100%, 97%);
  width:100%;
  height:70%;
}
.app-main{
  width:100%;
  height:100%;
  display:flex;
  place-items:center;
  justify-content:center;
}
.app-main-semi-ctn{
  background-color: hsl(0, 0%, 100%);
  width:40%;
  padding:40px;
  border-radius:20px;
}
.app-main-semi-ctn-content-ctn{
  
}
.head{
  display:flex;
}
.head-title{
  font-size:4vh;
  font-weight:700;
}
.content{
  margin:30px 0;
}
.first-content-question, .second-content-question, .third-content-question,.fourth-content-question{
  display:flex;
  justify-content:space-between;
  font-weight:600;
}
.first-content-question:hover, .second-content-question:hover, .third-content-question:hover,.fourth-content-question:hover{
  cursor: pointer;
  color: hsl(281, 83%, 54%);
}
.first-content-question-text, .second-content-question-text, .third-content-question-text, .fourth-content-question-text{
  font-size:16px;
  margin: auto 0;
}
.first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
  color:hsl(0, 0%, 100%);
  padding:5px;
  border-radius:50%;
  display:flex;
  place-items:center;
}
.first-content-question-icon:hover, .second-content-question-icon:hover, .third-content-question-icon:hover, .fourth-content-question-icon:hover{
  cursor:pointer;
  transform:scale(0.95);
  transition: all .4s;
}
.first-content-answer, .second-content-answer, .third-content-answer, .fourth-content-answer{
  color: hsl(0, 2%, 44%);
  line-height:2;
  margin:10px 0;
}

@media screen and (max-width:1300px) and (min-width:951px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:2px;
  }
  .app-main-semi-ctn{
    width:55%;
  }
}
@media screen and (max-width:950px) and (min-width:831px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:2px;
  }
  .app-main-semi-ctn{
    width:65%;
  }
}
@media screen and (max-width:830px) and (min-width:651px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:2px;
  }
  .app-main-semi-ctn{
    width:80%;
  }
}
@media screen and (max-width:650px) and (min-width:591px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:2px;
    display:flex;
    place-items:center;
  }
  .app-main-semi-ctn{
    width:90%;
  }
}
@media screen and (max-width:590px) and (min-width:361px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:10px;
  }
  .app-main-semi-ctn{
    width:90%;
  }
}
@media screen and (max-width:360px){
  .first-content-question-icon, .second-content-question-icon, .third-content-question-icon, .fourth-content-question-icon{
    padding:px 10px;
    display:flex;
    place-items:center;
  }
  .app-main-semi-ctn{
    width:90%;
  }
}
</style>


<template>
  <div class="app-main-colored">
    <div class="app-first-color"></div>
    <div class="app-second-color"></div>
  </div>
  <div class="app-main">
    <div class="app-main-semi-ctn">
      <div class="app-main-semi-ctn-content-ctn">
        <div class="head">
          <div class="head-img">
            <img src="/public/icon-star.svg" alt="icon-star">
          </div>
          <div class="head-title">
            <p>FAQs</p>
          </div>
        </div>
        <div class="content">

          <div class="first-content">
            <div class="first-content-question">
              <div class="first-content-question-text">
                <p> {{ quests[0].text }} </p>
              </div>
              <div v-html="firstIcon" class="first-content-question-icon" :style="{ backgroundColor:firstIconBg}" @click="firstIconInteract"></div>
            </div>
            <div class="first-content-answer" >
              <p :style="{display:firstAnswer}"> {{ quests[0].answer }} </p>
            </div>
          </div><br/>

          <div class="second-content">
            <div class="second-content-question">
              <div class="second-content-question-text">
                <p> {{ quests[1].text }} </p>
              </div>
              <div v-html="secondIcon" class="second-content-question-icon" :style="{ backgroundColor:secondIconBg}" @click="secondIconInteract"></div>
            </div>
            <div class="second-content-answer">
              <p :style="{display:secondAnswer}"> {{ quests[1].answer }} </p>
            </div>
          </div><br/>

          <div class="third-content">
            <div class="third-content-question">
              <div class="third-content-question-text">
                <p> {{ quests[2].text }} </p>
              </div>
              <div v-html="thirdIcon" class="third-content-question-icon" :style="{ backgroundColor:thirdIconBg}" @click="thirdIconInteract"></div>
            </div>
            <div class="third-content-answer">
              <p :style="{display:thirdAnswer}"> {{ quests[2].answer }} </p>
            </div>
          </div><br/>

          <div class="fourth-content">
            <div class="fourth-content-question">
              <div class="fourth-content-question-text">
                <p> {{ quests[3].text }} </p>
              </div>
              <div v-html="fourthIcon" class="fourth-content-question-icon" :style="{ backgroundColor:fourthIconBg}" @click="fourthIconInteract"></div>
            </div>
            <div class="fourth-content-answer">
              <p :style="{display:fourthAnswer}"> {{ quests[3].answer }} </p>
            </div>
          </div>
          <br/>
        </div>
      </div>
      <ChallengeAsset></ChallengeAsset>
    </div>
  </div>
</template>
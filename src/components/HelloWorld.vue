<template>
   <div class="grid-container">
  <div class="headd">
    <span>Hello.</span>
  </div>
  <div class="logo"></div>
  <div class="mained">
    <div class="mainhead">
      <span>My name is Daniel Olabemiwo.</span>
    </div>
    <div class="mainbody">
      <p>I am a Software Developer with interest in Web related programming. 
        I am fascinated by the ability of various technologies being deployed to the growth of web.
        Most of my personal projects are available on <i><a href="https://github.com/D-Lite" class="genlink">GitHub</a></i>. 
        Currently working on Vue related projects. You can follow me on <i><a href="https://twitter.com/fikkyman1" class="genlink">Twitter</a></i> where
        I tweets about issues I am of good opinions. 
      </p>
      <p>
         Currently ennrolled at the 
         <i><a href="https://www.unilorin.edu.ng/" class="genlink">University of Ilorin</a></i> for a Bachelor of Science degree in Information and Communication Science.
         Aside that, I am studying Data Structure and Algorithm online on <i><a href="https://www.coursera.org/specializations/data-structures-algorithms" class="genlink">COURSERA</a></i>.
      </p>
      <p>
        Aside programming, I read books, not restricted to any area. I can recommend John Grisham's <i>THE LITIGATORS</i>. 
        His collections are top-notch 👍 . I am learning how to express my code actions in words. Practising writing to improve myself.
        I enjoy video games always.
      </p>
      <p>
        Connect with me and see my contributions on <a href="https://www.linkedin.com/in/theolabemiwodaniel/" class="genlink">LinkedIn</a>, <a href="https://twitter.com/fikkyman1" class="genlink">Twitter</a>, <a href="" class="genlink">GitHub</a>.
      </p>
    </div>
  </div>
  <div class="mainright">
    <div>
      <p>Download <a href="" class="genlink">Resume</a></p>
    </div>
    <div>
      <p><a href="mailto:olabemiwodaniel@gmail.com" class="genlink">olabemiwodaniel@gmail.com</a></p>
    </div>
  </div>
</div>
</template>

<script>
export default {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,500;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@600;700&display=swap');

html {
  scroll-behavior: smooth;
}


 .grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 100px 1fr 1fr;
  gap: 10px 10px ;
  padding-left:20px;
  padding-right:20px;
  margin-top: -30px;
  grid-template-areas:
    "headd headd headd logo"
    "mained mained mained mainright"
    "mained mained mained mainright";
}

.headd { grid-area: headd; 
}

.headd span {
  font-family: 'Cairo', sans-serif;
  font-size: 50px;
  font-weight: 800;
  color: #022;
  display: flex;
  justify-content: left;
  align-items: flex-end;
}

.logo { grid-area: logo; 
}

.mained { grid-area: mained;
  font-family: 'Karla', sans-serif;
  margin-top: -20px;
}

.mainhead {
  font-family: 'Karla', sans-serif;
  font-size: 30px;
  font-weight: 700;
  color: #022;
  display: flex;
  justify-content: left;
  align-items: flex-end;
  padding-bottom: 10px;
}

.mainbody {
  text-align: left;
  margin-top: -30px;
}

.mainbody p {
  font-family: 'Karla', sans-serif;
  font-size: 20px;
  font-weight: 300;
  color: #022;
  justify-content: left;
  max-width: 60ch;
  
}
p {
    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;

}


.mainright { grid-area: mainright; 
  margin-top: -20px;
}

 .genlink {
   height: 10px;
   text-decoration: none;
   color: #121314;
   cursor: pointer;
   position: relative;
   padding: 0.1em;
 }

 .genlink:after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 35%;
    transition: top 200ms cubic-bezier(0, 0.8, 0.13, 1);
    background-color: rgba(79, 192, 141, 0.5);
    -webkit-transition: top 200ms cubic-bezier(0, 0.8, 0.13, 1);
        -moz-transition:  top 200ms cubic-bezier(0, 0.8, 0.13, 1);

  }

p i a:hover {
  cursor: pointer;
}
p i .genlink:hover:after {
  background-color: #fde575;
}

@media (max-width: 900px) {
  .grid-container { grid-template-columns: repeat(2, 1fr); 
    display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 100px 1fr 1fr 1fr;
  gap: 10px 10px ;
  padding-left:20px;
  padding-right:20px;
  /* margin-top: -30px; */
  grid-template-areas:
    "headd headd logo"
    "mained mained mained"
    "mained mained mained"
    "mainright mainright mainright"
    ;
  text-align: left;
  
  }
  .mainhead {
  font-family: 'Karla', sans-serif;
  font-size: 25px;
  font-weight: 700;
  color: #022;
  display: flex;
  justify-content: left;
  align-items: flex-end;
  padding-bottom: 10px;
}
}
</style>

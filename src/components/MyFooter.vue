<template>
    <div class="my-footer">
        <div class="left">
            <h1 class="create">Lets Create Cool things together</h1>
            <address>
                <a class="email" href="mailto:jordantanaliga@gmail.com?subject=Hello%20Jordan ~? ">
                    <h4 class="email">jordantanaliga@gmail.com </h4> 
                </a>
            </address>
        </div>
        <div class="right">
   
                <!-- <a href="mailto:jordantanaliga@gmail.com?subject=Hello%20Jordan ~?"> 
                Contact Me
                <a/> -->
                <button class="resume">
                    <a href="require('../src/assets/TanaligaCV.pdf')" download > Download Resume</a>
                </button>
            <!-- <Contact/> -->
        </div>
    </div>

</template>

<script>
    export default {
        name: 'MyFooter',
        data() {
            return {

            }
        }
    }
</script>

<style scoped>
.my-footer {
    width: 100%;
    background: white;
    text-align: center;
    color: black;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    justify-content: center;
    align-items: center;
    height: 300px;
}
.create {
    font-weight: 700;
    font-size: xx-large;
    color:rgba(56, 42, 42, 0.897);
    justify-content: space-around;
}
.left {
    margin: 0px 30px;
}
.right {
    margin: 0px 10px;
}
a {
    text-decoration: none;
  font-weight: 900;
  word-spacing: 5px;  
  font-size: 20px;
  color: white;
}
.right button{
    text-decoration: none;
    padding: 10px;
    margin:20px;
}
.email {
    text-decoration-line: none;
    color: crimson;
    font-size: small;
    font-style: normal;
 
}
.resume {
    background-color: crimson;
    color: white;
    padding:10px 40px;
    border: none;
    border-radius: 5px;
    box-shadow: .5px 3px 1px .4px;
    text-decoration: none;
}
.resume:hover{
      background: rgba(0, 0, 0, 0.761);
  color: white;
}

@media all and (max-width:520px) {

    .my-footer {
    width: 100%;
    background: white;
    text-align: center;
    color: black;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 300px;
}
.create {
    font-size: large;
}
.resume a:hover {
    /* background-color: crimson;
    color: white; */
    padding:5px 10px;
    border: none;
    border-radius: 10px;
    text-decoration: none;
    font-size: 15px;
    transform: translate(5px);

}

}


</style>
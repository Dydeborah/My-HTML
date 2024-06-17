<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Form</title>
</head>
<style>
    @import url('https://fonts.googleapis.com/css?family=poppins:200,300,400,500,600,700,800,900&display=swap');
*
{
    margin:0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins', sans-serif;
}
body{
    overflow: hidden;
}
section{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: linear-gradient(to bottom, #7de6e2, #cc7293);
}
section .color{
    position: absolute;
    filter: blur(150px);
}
section .color:nth-child(1){
    top:-350px;
    width: 600px;
    height: 600px;
    background: #ff359b;
}
section .color:nth-child(2){
    bottom:-150px; 
    left: 100px; 
    width: 500px;
    height: 500px;
    background: #fffd87;
}
section .color:nth-child(3){
    bottom:50px; 
    right: 100px; 
    width: 300px;
    height: 300px;
    background: #00d2ff;
}
.box{
    position: relative;
}
.box .square{
    position: absolute;
    backdrop-filter: blur(5px);
     box-shadow: 0 25px 45px rgba(0, 0, 0, 0.1);
     border: 1px solid rgba(255, 255, 255, 0.5);
     border-right: 1px solid rgba(255, 255, 255, 0.2);
     border-bottom: 1px solid rgba(255, 255, 255, 0.2);
     background: rgba(255, 255, 255, 0.1);
     border-radius: 10px;
     animation: animate 10s linear infinite;
     animation-delay: calc(-1s * var(--i));
}
@keyframes animate{
    0%,100%{
        transform: translateY(-40px);
    }
    50%{
        transform: translateY(40px);
    }
}
.box .square:nth-child(1){
    top: -50px;
    right: -60px;
    width: 100px;
     height: 100px;
}
.box .square:nth-child(2){
    top: 150px;
    left: -100px;
    width: 120px;
     height: 120px;
     z-index: 2;
}
.box .square:nth-child(3){
    bottom: 50px;
    right: -60px;
    width: 80px;
     height: 80px;
     z-index: 2;
}
.box .square:nth-child(4){
    bottom: -80px;
    left: 100px;
    width: 50px;
     height: 50px;
}
.box .square:nth-child(5){
    top: -80px;
    left: 140px;
    width: 60px;
     height: 60px;
}
.container{
    position: relative;
    width: 400px;
     min-height: 400px;
     background: rgba(255, 255, 255, 0.1);
     border-radius: 10px;
     display: flex;
     justify-content: center;
     align-items: center;
     backdrop-filter: blur(5px);
     box-shadow: 0 25px 45px rgba(0, 0, 0, 0.1);
     border: 1px solid rgba(255, 255, 255, 0.5);
     border-right: 1px solid rgba(255, 255, 255, 0.2);
     border-bottom: 1px solid rgba(255, 255, 255, 0.2);
}
.form{
    position: relative;
     width: 100%;
     height: 100%;
     padding: 40px;
}
.form h2{
    position: relative;
    color: #fff;
    font-size: 24px;
    font-weight: 600;
    letter-spacing: 1px;
    margin-bottom: 40px;
}
.form h2::before{
    content: '';
    position: absolute;
    left: 0;
    bottom: -10px;
    width: 80px;
    height: 4px;
    background: #fff;
}
.form .inputBox{
    width: 100%;
    margin-top: 20px ;
}
.form .inputBox input{
    width: 100%;
    background: rgba(255, 255, 255, 0.2);
    border: none;
    outline: none;
    padding: 10px 20px;
    border-radius: 35px;
    border: 1px solid rgba(255, 255, 255, 0.5);
     border-right: 1px solid rgba(255, 255, 255, 0.2);
     border-bottom: 1px solid rgba(255, 255, 255, 0.2);
     font-size: 16px;
     letter-spacing: 1px;
     color: #fff;
     box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
}
.form .inputBox input::placeholder{
    color: #fff;
}
.form .inputBox input[type="submit"]{
    background: #fff;
    color: #666;
    max-width: 100px;
    cursor: pointer;
    margin-bottom: 20px;
    font-weight: 600;
}
.forget{
    margin-top: 5px;
    color: #fff;
}
.forget a{
    color: #fff;
    font-weight: 600;
}
</style>
<body>
    <section>
        <div class="color"></div>
        <div class="color"></div>
        <div class="color"></div>
        <div class="box">
            <div class="square" style="--i:0;"></div>
            <div class="square" style="--i:1;"></div>
            <div class="square" style="--i:2;"></div>
            <div class="square" style="--i:3;"></div>
            <div class="square" style="--i:4;"></div>
            <div class="container">
                <div class="form">
                    <h2>Login Form</h2>
                    <form>
                        <div class="inputBox">
                            <input type="text" placeholder="Username">
                        </div>
                        <div class="inputBox">
                            <input type="password" placeholder="Password">
                        </div>
                        <div class="inputBox">
                            <input type="submit" value="Login">
                        </div>
                        <p class="forget">Forgot password? <a href="https://youtu.be/sVCadTCAfLs?si=qltPejGfqD8jzSGq">Click here</a></p>
                        <p class="forget">Don't have an account? <a href="https://youtu.be/9yA084piAgc?si=wH4AKSQEpp4IWzxy">Sign up</a></p>
                    </form>
                </div>
            </div>
        </div>
    </section>
</body>
</html>

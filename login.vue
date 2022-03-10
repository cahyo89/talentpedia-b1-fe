<template>
    <div class="centered">
        
        <h3 class="h">Masuk ke Akun Anda</h3>
        <form>
            <div class="txt_field">
                <input type="text" class="inp" required>
                <label>Alamat Email</label>
            </div>
            <div class="txt_field">
                <input type="text" class="inp" required>
                <label>Password</label>
            </div>
            <div class="pass">Forgot Password</div>
            <input type="submit" value="Masuk">
            
            <div class="signup-link">
                Not a member? <a href="/signup">Sign Up</a>
            </div>
        </form>
    </div>
</template>


<style>
body {
    margin: 0;
    padding: 0;
    line-height: 1.6;
    font-family: Apercu,Gill Sans MT,Gill Sans,Arial,sans-serif;
    letter-spacing: .05em;
    background: #F5FFFA;
    height: 100vh;
    overflow: hidden;
}

.centered {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 500px;
    background: white;
}

.centered .h {
    text-align: center;
    padding: 0 0 20px 0;
    border-bottom: 1px solid silver;
     font-family: Apercu,Gill Sans MT,Gill Sans,Arial,sans-serif;
}

.centered form{
    padding: 0 40px;
    box-sizing: border-box;
}
form .txt_field{
    position: relative;
    border-bottom: 2px solid #adadad;
    margin: 30px 0;
}
.txt_field .inp {
    width: 100%;
    padding: 0 5px;
    height: 40px;
    font-size: 16px;
    border: none;
    background: none;
    outline: none;
}
.txt_field label{
    position: absolute;
    top: 50%;
    left: 5px;
    color: #adadad;
    transform: translateY(-50%);
    font-size: 16px;
    pointer-events: none;
    transition: .5s;
}
.txt_field span::before{
    content:'';
    position: absolute;
    top: 40px;
    left: 0;
    width: 0;
    height: 2px;
    background: #2691d9;
    transition: .5s;
}
.txt_field .inp:focus ~ label,
.txt_field .inp:valid ~ label{
    top: -5px;
    color: #2691d9;
}
.txt_field .inp:focus ~ span::before,
.txt_field .inp:valid ~ span::before{
    width: 100%;
    color: #2691d9;
}
.pass{
    margin: -5px 0 20px  5px;
    color: #a6a6a6;
    cursor: pointer;
}
.pass:hover{
    text-decoration: underline;
}
input[type="submit"]{
    width: 100%;
    height: 50px;
    border: 1px solid;
    background: black;
    font-size: 18px;
    color: #e9f4fb;
    font-weight: 700;
    cursor: pointer;
    outline: none;
}
input[type="submit"]:hover{
    border-color:#2691d9;
}
.signup-link{
    margin: 30px 0;
    text-align: center;
    font-size: 16px;
    color: #6666;
}
.signup-link a{
    color: #2691d9;
    text-decoration: none;
}
</style>
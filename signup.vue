<template>
    <div class="centered">
        <form>
            <h3>Sign Up</h3>
            <p>Please fill in this form to create an account.</p>
            <hr>

           <div class="txt_field">
               <label>Alamat Email</label>
                <input type="text" class="inp" > 
            </div>

            <div class="txt_field">
               <label>Nama Lengkap</label>
                <input type="text" class="inp" > 
            </div>

            <div class="txt_field">
                <label>Password</label>
                <input type="text" class="inp">
            </div>

             <div class="txt_field">
               <label>Alamat</label>
                <input type="text" class="inp" > 
            </div>

            <div class="txt_field">
               <label>Nomor Telefon</label>
                <input type="text" class="inp" > 
            </div>

            <div class="control">
                <label>Gender</label> <br>
                <label class="radio">
                    <input type="radio" name="answer">
                    Wanita
                </label>
                <label class="radio">
                    <input type="radio" name="answer">
                    Pria
                </label>
            </div>

            <label>
            <input type="checkbox" checked="checked" name="remember" style="margin-bottom:15px"> Remember me
            </label>
    
             <p>Dengan membuat atau mendaftar akun, Anda menyetujui isi <a href="/term" style="color:dodgerblue">Persyaratan dan Ketentuan</a>.</p>

            <div class="clearfix">
                <input type="submit" class="signupbtn" href="/login" value="DAFTAR">
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
    height: 165vh;
    overflow: hidden;
}

.centered {
    position: absolute;
    top: 73%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 500px;
    background: white;
    padding: 40px;
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
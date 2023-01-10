<template>
    <div>
        <div class="signup-header">
            <b> MOKA</b>
        </div>

        <div class="main">
            <div class="wave">
                <div class="content">
                    <p>
                        "Perencanaan keuangan yang benar, seperti membuat anggaran, menabung untuk dana darurat, berinvestasi, menyiapkan biaya untuk masa pensiun dapat membantu
                        Anda hidup lebih sejahtera, meskipun ada badai keuangan."
                    </p>
                    <h3>Bern Bernanke</h3>
                </div>
            </div>
            <div class="container">
                <div class="SignUp">
                    <form action="">
                        <h2>Daftar</h2>
                        <label for="">Nama Pengguna*</label>
                        <input class="input" type="text" placeholder="nama pengguna" />
                        <label for="">Email*</label>
                        <input class="input" type="text" placeholder="moka@gmail.com" />
                        <label for="">Kata Sandi*</label>
                        <input class="input" type="password" placeholder="Kata Sandi" />
                        <label for="">Ulang Kata Sandi</label>
                        <input class="input" type="password" placeholder="Ulangi Sandi" name="psw-repeat" required />

                        <div class="regis">
                            <center>
                                <NuxtLink to="/dashboard" class="btn">Daftar</NuxtLink>
                            </center>
                        </div>
                        <p style="text-align: center; margin-top: 15px; margin-bottom: 0px">atau</p>
                    </form>
                    <form class="signup-form">
                        <div class="signup-form-footer">
                            <a href="google.com"> <img src="@/assets/img/google.jfif" alt="google" />Google </a>
                            <br />
                            <a href="facebook.com"> <img src="@/assets/img/fb.png" alt="facebook    " />Facebook </a>
                        </div>
                    </form>
                    <div class="info">Sudah punya akun? <NuxtLink to="/masuk">Masuk</NuxtLink></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.main {
    display: flex;
    gap: 4em;
    justify-content: center;
    margin-bottom: 2em;

}

.container {
    width: 100%;
    display: flex;
    max-width: 480px;
    background: #fff;
    border-radius: 15px;
    padding: 2em;
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}
.wave {
    width: 100%;
    display: flex;
    max-width: 480px;
    background: rgb(174, 226, 178);
    border-radius: 15px;
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
    padding: 2em;
}
.content {
    width: 480px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    font-size: var(--text-md);
}

.content h3 {
    font-size: var(--text-lg);
}

.SignUp {
    width: 480px;
}

h2 {
    margin: 20px;
    text-align: center;
    font-weight: bolder;
    text-transform: uppercase;
}

hr {
    border-top: 2px solid #60615c;
}

form label {
    display: block;
    font-size: 18px;
    font-weight: 600;
    padding: 5px;
}

.signup-form-footer {
    gap: 20px;
    display: flex;
    justify-content: center;
}

.signup-form a {
    border: 2px solid rgb(119, 116, 116);
    width: 150px;
    height: 40px;
    padding: 0.6rem;
    justify-content: center;
    display: flex;
    align-items: center;
    color: black;
    box-shadow: 0 10px 15px rgba(9, 9, 9, 0.1);
    border-radius: 5px;
    margin-top: -30px;
    margin-bottom: 1em;
}

.signup-form img {
    width: 25px;
    margin-right: 5px;
}

.signup-header {
    font-size: 45px;
    text-align: center;
    color: rgb(174, 226, 178);
    margin-bottom: 20px;
    margin-top: 20px;
}
.info {
    text-align: center;
    font-size: 18px;
}
@media screen and (max-width: 1080px) {
    .wave {
        max-width: 390px;
        margin-left: 40px;
        margin-right: 40px;
    }
    .container {
        max-width: 380px;
    }

    .content {
        width: 380px;
        font-size: 23px;
    }

    .SignUp {
        width: 380px;
    }

    .login-form a {
        width: 100px;
        font-size: 12px;
        margin-top: -25px;
    }
}

@media screen and (max-width: 770px) {
    .signup-header {
        font-size: 30px;
    }
    .wave {
        display: none;
    }
    .container {
        max-width: 510px;
    }

    .content {
        font-size: 18px;
    }

    .SignUp label {
        width: 200px;
        font-size: 13px;
    }
    .SignUp h2 {
        font-size: 20px;
        margin-bottom: 10px;
        margin-top: -10px;
    }

    .signup-form a {
        width: 100px;
        font-size: 11px;
        margin-top: -25px;
    }
    .signup-form img {
        width: 15px;
    }
    .info {
        font-size: 13px;
    }
}
</style>
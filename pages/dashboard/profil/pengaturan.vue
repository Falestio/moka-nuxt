<template>
    <div>
        <Drawer>
            <a class="tittle">Pengaturan</a>

            <div class="main-content">
                <div class="sub-tittle"><a>Tampilan</a></div>

                <div class="content">
                    <div class="baris-content">
                        <div class="content-kiri">
                            <a>Format Waktu</a>
                        </div>
                        <div class="content-kanan">
                            <a>23/11/2022</a>
                        </div>
                    </div>
                    <div class="baris-content">
                        <div class="content-kiri">
                            <a>Pilih Bahasa</a>
                        </div>
                        <div class="content-kanan">
                            <a>Bahasa Indonesia</a>
                        </div>
                    </div>
                    <div class="baris-content">
                        <div class="content-kiri">
                            <a>Mata Uang</a>
                        </div>
                        <div class="content-kanan">
                            <a>IDR</a>
                        </div>
                    </div>
                    <div class="baris-content">
                        <div class="content-kiri">
                            <a>Format Waktu</a>
                        </div>
                        <div class="content-kanan">
                            <a>23/11/2022</a>
                        </div>
                    </div>
                    <div class="sub-tittle"><a>Sistem</a></div>
                    <div class="baris-content">
                        <div class="content-kiri">
                            <a>Privasi</a>
                        </div>
                        <!-- <div class="content-kanan">
              <a>23/11/2022</a>
          </div> -->
                    </div>
                </div>
            </div>
        </Drawer>
    </div>
</template>

<style scoped>

.tittle{
    font-size: 40px;
    margin-left: 30px;
}

.sub-tittle {
    font-style: normal;
    font-weight: 700;
    font-size: 30px;
    line-height: 39px;
    margin-top: 40px;
    margin-left: 35px;
    margin-bottom: 20px;
}

.baris-content {
    width: 100%;
    height: 65px;
    justify-content: space-between;
    align-items: center;
    display: flex;
    border-top: 1px solid;
    border-bottom: 1px solid;
    border-color: #bababb;
}

.baris-content a {
    margin-left: 35px;
    font-weight: 400;
    font-size: 20px;
    line-height: 29px;
    margin-left: 60px;
}

.content-kanan a {
    color: green;
    font-weight: 700;
    font-size: 22px;
    line-height: 29px;
    margin-right: 60px;
}

/* @media only screen and (max-width: 450px) {
    .baris-content {
        font-size: 15px;
    }
} */
</style>
<template>
    <div>
        <Drawer>
            <div class="main">
                <div id="isi">
                    <nav class="main-nav">
                        <div class="main-nav-wrapper">
                            <div class="flex aic">
                                <NuxtLink to="/dashboard/transaksi" class="card__header--back btn-ghost-circle">
                                    <svg width="32" height="32" viewBox="0 0 24 24"><path fill="currentColor" d="m13.3 17.3l-4.6-4.6q-.15-.15-.212-.325q-.063-.175-.063-.375t.063-.375q.062-.175.212-.325l4.6-4.6q.275-.275.7-.275q.425 0 .7.275q.275.275.275.7q0 .425-.275.7L10.8 12l3.9 3.9q.275.275.275.7q0 .425-.275.7q-.275.275-.7.275q-.425 0-.7-.275Z" /></svg>
                                </NuxtLink>
                                <div class="main-nav-wrapper-a">
                                    <b> Detail Transaksi </b>
                                </div>
                            </div>
                            <div class="dropdown">
                                <div class="dropdown-trigger">
                                    <svg width="32" height="32" viewBox="0 0 256 256"><path fill="currentColor" d="M116 64a12 12 0 1 1 12 12a12 12 0 0 1-12-12Zm12 52a12 12 0 1 0 12 12a12 12 0 0 0-12-12Zm0 64a12 12 0 1 0 12 12a12 12 0 0 0-12-12Z"/></svg>
                                </div>
                                <div class="dropdown-menu">
                                    <NuxtLink to="/dashboard/transaksi/tambah">Edit</NuxtLink>
                                    <NuxtLink to="/dashboard/transaksi/">Delete</NuxtLink>
                                </div>  
                            </div>
                        </div>
                    </nav>
                    <div id="detail">
                        <div id="subjudul-detail">
                            <div id="isi-detail">
                                <div id="isi-detail-1">
                                    <b>Makanan dan Minuman</b>
                                </div>
                                <div id="isi-detail-2">Main</div>
                                <div id="isi-detail-3">Rabu 23/11/2022</div>
                                <br />
                                <hr>
                                <div id="isi-detail-4">-Rp 60.000,00</div>
                            </div>
                        </div>
                    </div>
                </div>
                <br /><br />
            </div>
        </Drawer>
    </div>
</template>

<style scoped>
/* DROPDOWN */
.dropdown {
    position: relative;
}
.dropdown-trigger {
    cursor: pointer;
    padding: .4em;
    border-radius: 50%;
}

.dropdown:hover {
    background-color: var(--super-light-grey);
}
.dropdown-menu {
    position: absolute;
    display: flex;
    flex-direction: column;
    border: 1px solid var(--light-grey);
    background-color: #fff;
    display: none;
}

.dropdown:hover .dropdown-menu {
    display: flex;
}

.dropdown-menu a {
    padding: 1em;
}

.dropdown-menu a:hover {
    background-color: var(--super-light-grey);
}

#isi {
    max-width: 800px;
    background-color: white;
    margin: 0 auto;
    border-radius: 20px;
    padding: 1em;
    border: 2px solid var(--light-grey);
}

.main {
    align-items: center;
}

.main-nav {
    width: 100%;
    height: 60px;
    display: flex;
    align-items: center;
    padding: 20px;
    border-bottom: 1px solid rgb(223, 223, 223);
}

.main-nav-wrapper {
    padding-bottom: 1em;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.main-nav-wrapper-a {
    font-size: 20px;
}

.main-nav__account {
    display: flex;
    gap: 1em;
}

#detail {
    display: flex;
    padding: 2em;
    width: 100%;

}

#subjudul-detail {
    display: flex;
    width: 100%;

}

#isi-detail {
    width: 100%;
}


#isi-detail-1 {
    font-size: 30px;
    margin-bottom: 15px;
}

#isi-detail-2 {
    font-size: 20px;
}

#isi-detail-3 {
    font-size: 15px;
    color: rgb(119, 119, 115);
}

#isi-detail-4 {
    font-size: 40px;
    color: rgb(237, 73, 13);
    margin-top: 30px;
}

#tolbul-detail {
    /* float: right;
    margin-left: 700px; */
    font-size: 18px;
    text-align: right;
}

@media screen and (max-width: 1080px) {
    #isi-detail-1 {
        font-size: 22px;
    }
    #isi-detail-2 {
        font-size: 17px;
    }
    #isi-detail-3 {
        font-size: 12px;
    }
    #isi-detail-4 {
        font-size: 30px;
        margin-top: 20px;
    }
    .main-nav-wrapper-a {
        font-size: 17px;
    }
}

@media screen and (max-width: 750px) {
    #isi-detail-1 {
        font-size: 18px;
    }
    #isi-detail-2 {
        font-size: 15px;
    }
    #isi-detail-3 {
        font-size: 12px;
    }
    #isi-detail-4 {
        font-size: 25px;
        margin-top: 20px;
    }
    .main-nav-wrapper-a {
        font-size: 15px;
    }
}
@media screen and (max-width: 480px) {
    #isi-detail-1 {
        font-size: 18px;
    }
    #isi-detail-2 {
        font-size: 15px;
    }
    #isi-detail-3 {
        font-size: 12px;
    }
    #isi-detail-4 {
        font-size: 25px;
        margin-top: 20px;
    }
    .main-nav-wrapper-a {
        font-size: 15px;
    }
}
</style>
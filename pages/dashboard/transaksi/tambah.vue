<template>
    <div>
        <Drawer>
            <div class="wrapper">
                <div class="card">
                    <div class="card__header">
                        <NuxtLink to="/dashboard/transaksi" class="card__header--back btn-ghost-circle">
                            <svg width="32" height="32" viewBox="0 0 24 24"><path fill="currentColor" d="m13.3 17.3l-4.6-4.6q-.15-.15-.212-.325q-.063-.175-.063-.375t.063-.375q.062-.175.212-.325l4.6-4.6q.275-.275.7-.275q.425 0 .7.275q.275.275.275.7q0 .425-.275.7L10.8 12l3.9 3.9q.275.275.275.7q0 .425-.275.7q-.275.275-.7.275q-.425 0-.7-.275Z" /></svg>
                        </NuxtLink>
                        <div class="card__header--title">
                            <svg width="32" height="32" viewBox="0 0 256 256">
                                <path fill="currentColor" d="M221.9 83.2a104 104 0 0 1-20.4 118.3a103.8 103.8 0 0 1-147 0a103.8 103.8 0 0 1 0-147A104 104 0 0 1 195.7 49l22.6-22.7a8.1 8.1 0 0 1 11.4 11.4l-62.1 62l-33.9 34a8.2 8.2 0 0 1-11.4 0a8.1 8.1 0 0 1 0-11.4l27.8-27.7a40.2 40.2 0 1 0 17.8 31.1a8 8 0 0 1 7.6-8.4a7.9 7.9 0 0 1 8.4 7.5a56 56 0 1 1-22.4-41.6l22.8-22.8a87.9 87.9 0 1 0 23.1 29.7a8 8 0 0 1 14.5-6.9Z" />
                            </svg>
                            <h2>Tambah Transaksi</h2>
                        </div>
                    </div>
                    <div class="card__body">
                        <form class="form">
                            <div class="form-control">
                                <label for="name" class="label">Nama</label>
                                <input id="name" type="text" class="input" />
                            </div>
                            <div class="form-control">
                                <label for="jenis-transaksi" class="label">Jenis Transaksi</label>
                                <select id="jenis-transaksi" class="select">
                                    <option>Pemasukan</option>
                                    <option>Pengeluaran</option>
                                </select>
                            </div>
                            <div class="form-control">
                                <label for="dompet" class="label">Dompet</label>
                                <select id="dompet" class="select">
                                    <option>Utama</option>
                                    <option>BRI</option>
                                    <option>BNI</option>
                                </select>
                            </div>
                            <div class="form-control">
                                <label for="jenis-transaksi" class="label">Kategori</label>
                                <select id="jenis-transaksi" class="select">
                                    <option>Makanan</option>
                                    <option>Liburan</option>
                                    <option>Transportasi</option>
                                    <option>Pajak</option>
                                    <option>Listrik</option>
                                    <option>Langganan</option>
                                </select>
                            </div>
                            <div class="form-control">
                                <label for="keterangan" class="label">Keterangan</label>
                                <input id="keterangan" type="text" class="input" />
                            </div>
                            <div class="form-control">
                                <label for="jumlah" class="label">Jumlah</label>
                                <input id="jumlah" type="text" class="input" />
                            </div>
                            <NuxtLink to="/dashboard/transaksi" class="btn">Tambah</NuxtLink>
                        </form>
                    </div>
                </div>
            </div>
        </Drawer>
    </div>
</template>

<style scoped>
.wrapper {
    padding: 1em;
    display: flex;
    justify-content: center;
}

.card {
    width: 600px;
    border: 1px solid rgb(223, 223, 223);
    border-radius: 10px;
}

.card__body {
    padding: 1em;
}

.card__header {
    display: flex;
    align-items: center;
    gap: 1em;
    padding: 1em;
    background-color: var(--super-light-grey);
}

.card__header--title {
    display: flex;
    align-items: center;
    gap: 1em;
}

.form {
    display: flex;
    flex-direction: column;
    gap: 1em;
}

.label {
    font-size: 18px;
    font-weight: 500;
}
</style>
<template>
    <div>
        <Drawer>
            <div class="wrapper">
                <div class="card">
                    <div class="card__header">
                        <NuxtLink to="/dashboard/dompet" class="card__header--back btn-ghost-circle">
                            <svg width="32" height="32" viewBox="0 0 24 24"><path fill="currentColor" d="m13.3 17.3l-4.6-4.6q-.15-.15-.212-.325q-.063-.175-.063-.375t.063-.375q.062-.175.212-.325l4.6-4.6q.275-.275.7-.275q.425 0 .7.275q.275.275.275.7q0 .425-.275.7L10.8 12l3.9 3.9q.275.275.275.7q0 .425-.275.7q-.275.275-.7.275q-.425 0-.7-.275Z"/></svg>
                        </NuxtLink>
                        <div class="card__header--title">
                            <svg class="menu__item--icon" width="32" height="32" viewBox="0 0 24 24"><path fill="currentColor" d="M21 18v1a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v1h-9a2 2 0 0 0-2 2v8a2 2 0 0 0 2 2m0-2h10V8H12m4 5.5a1.5 1.5 0 0 1-1.5-1.5a1.5 1.5 0 0 1 1.5-1.5a1.5 1.5 0 0 1 1.5 1.5a1.5 1.5 0 0 1-1.5 1.5Z"/></svg>
                            <h2>Tambah Dompet</h2>
                        </div>
                    </div>
                    <div class="card__body">
                        <form class="form">
                            <div class="form-control">
                                <label for="name" class="label">Nama</label>
                                <input id="name" type="text" class="input" />
                            </div>
                            <div class="form-control">
                                <label for="keterangan" class="label">Keterangan</label>
                                <input id="keterangan" type="text" class="input" />
                            </div>
                            <div class="form-control">
                                <label for="jumlah" class="label">Saldo Awal</label>
                                <input id="jumlah" type="text" class="input" />
                            </div>
                            <NuxtLink to="/dashboard/dompet"  class="btn">Tambah</NuxtLink>
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
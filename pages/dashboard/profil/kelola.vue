<script setup>
let edit = ref(false)

function toggleEdit() {
    edit.value = !edit.value
}

</script>

<template>
    <div>
        <Drawer>
            <div class="top-main-content">
                <img src="@/assets/img/profilePicture.jpg" class="profilepicture" />
                <div class="edit" @click="toggleEdit()" v-if="!edit">
                    <a style="font-size: 30px; margin-left: 30px">Ananda Pratama</a>
                    <img src="https://api.iconify.design/ic:round-mode-edit.svg" style="margin-left: 15px; width: 18px" />
                </div>
                <div class="form" v-if="edit">
                    <input class="input" type="text" placeholder="Nama Baru">
                    <div>
                        <button @click="toggleEdit()" class="btn">Batal</button>
                        <button @click="toggleEdit()" class="btn">Ubah</button>
                    </div>
                </div>
            </div>
        </Drawer>
    </div>
</template>

<style scoped>
.top-main-content, .form {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

.edit {
    cursor:pointer;
}

.form {
    display: flex;
    cursor:pointer;
}

.profilepicture {
    width: 300px;
    margin-bottom: 30px;
}
</style>
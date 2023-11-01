<script>
    export default {
        props: {
            contact: {type: Object, required: true},
        },
        name: 'ContactCard',
    };
</script>

<template>
    <div>
        <div class="p-l">
            <strong>Tên:</strong>
            {{ contact.name }}
        </div>

        <div class="p-l">
            <strong>E-mail:</strong>
            {{ contact.email }}
        </div>

        <div class="p-l">
            <strong>Địa chỉ:</strong>
            {{ contact.address }}
        </div>

        <div class="p-l">
            <strong>Điện thoại:</strong>
            {{ contact.phone }}
        </div>

        <div class="p-l">
            <strong>Liên hệ yêu thích:&nbsp;</strong>
            <i class="fas fa-check" v-if="contact.favorite"></i>
            <i class="fas fa-times" v-else></i>
        </div>
    </div>
</template>

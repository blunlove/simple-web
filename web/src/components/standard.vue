<template>
    <div class="standard">
        <child-title :headerData="title_data"></child-title>
        <div class="standard_image"></div>
    </div>
</template>

<script>
let title_data = {
    chinese: '国家标准试验',
    english: 'EN817 GB18145-2003',
}

import ChildTitle from './child/child_title.vue';
export default {
    name: 'standard',
    data() {
        return {
            title_data: title_data,
        }
    },
    components: {
        ChildTitle,
    }
}
</script>
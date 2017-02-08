<template>
    <img ref="image" :src="show" :alt="alt" />
</template>
<script type="text/javascript">
    export default {
        props: {
            small: {
                required: true,
                type: String
            },
            normal: {
                required: true,
                type: String
            },
            alt: {
                required: true,
                type: String
            }
        },
        data() {
            return {
                src: {
                    small: this.small,
                    normal: this.normal
                },
                show: this.small
            }
        },
        methods: {
            load(){
                let image = new Image();
                let self = this

                image.onload = () => {
                    setTimeout(() => {
                        self.show = self.src.normal
                    }, 500)
                }
                image.src = this.src.normal
            }
        },
        mounted(){
            this.load();
        }
    }
</script>
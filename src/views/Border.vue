<template>
    <my-page title="CSS 边框生成">
        <div class="common-container container">
            <div class="preview" :style="previewStyle"></div>
            <div class="form">
                <ui-slider class="slider" v-model="width" :min="1" :max="100" :step="1"/>
            </div>
            <pre><code>{{ code }}</code></pre>
        </div>
    </my-page>
</template>

<script>
    export default {
        data () {
            return {
                width: 1
            }
        },
        computed: {
            previewStyle() {
                return {
                    border: `${this.width}px solid #000`
                }
            },
            code() {
                return `.demo {
    border: ${this.width}px solid #000;
}`
            }
        },
        mounted() {
        },
        methods: {
        }
    }
</script>

<style scoped>
    .preview {
        width: 100px;
        height: 100px;
        margin-bottom: 24px;
        border: 1px solid #000;
    }
    .form {
        width: 240px;
        margin-bottom: 24px;
    }
</style>

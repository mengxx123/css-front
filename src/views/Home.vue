<template>
    <my-page title="CSS" :page="page">
        <div class="common-container">
            <app-list :data="groups" />
        </div>
    </my-page>
</template>

<script>
    /* eslint-disable */
    export default {
        data () {
            return {
                groups: [
                    {
                        apps: [
                            {
                                name: 'CSS 三角形',
                                desc: '',
                                icon: 'https://icons.yunser.com/icons/tool.svg',
                                to: 'xxx',
                                href: 'https://csstriangle.yunser.com/',
                                target: '_blank'
                            },
                            {
                                name: 'CSS 边框生成',
                                desc: '',
                                icon: 'https://icons.yunser.com/icons/tool.svg',
                                to: '/border'
                            }
                        ]
                    },
                ],
                page: {
                    menu: [
                        {
                            type: 'icon',
                            icon: 'search',
                            href: 'https://search.yunser.com?utm_source=edu',
                            target: '_blank',
                            title: '搜索'
                        },
                        {
                            type: 'icon',
                            icon: 'apps',
                            href: 'https://app.yunser.com?utm_source=edu',
                            target: '_blank',
                            title: '应用'
                        }
                    ]
                }
            }
        },
        computed: {
        },
        mounted() {
        },
        methods: {
            init() {
            },
            fileChange(e) {
            },
            sizeStr: function (size) {
            }
        }
    }
</script>

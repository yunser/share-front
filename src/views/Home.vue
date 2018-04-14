<template>
    <my-page title="分享">
        <div class="span five bdsharebuttonbox">
            <a href="#" class="bds_qzone" data-cmd="qzone" title="分享到QQ空间"></a>
            <a href="#" class="bds_tsina" data-cmd="tsina" title="分享到新浪微博"></a>
            <a href="#" class="bds_weixin" data-cmd="weixin" title="分享到微信"></a>
            <a href="#" class="bds_sqq" data-cmd="sqq" title="分享到QQ好友"></a>
            <a href="#" class="bds_douban" data-cmd="douban" title="分享到豆瓣网"></a>
            <a href="#" class="bds_bdhome" data-cmd="bdhome" title="分享到百度新首页"></a>
            <a href="#" class="bds_tieba" data-cmd="tieba" title="分享到百度贴吧"></a>
            <a href="#" class="bds_renren" data-cmd="renren" title="分享到人人网"></a>
            <a href="#" class="bds_more" data-cmd="more"></a>
            <!--<a class="bds_count" data-cmd="count"></a>-->
        </div>
    </my-page>
</template>

<script>
    /* eslint-disable */
    export default {
        data () {
            return {
                page: {
                    menu: [
                        {
                            type: 'icon',
                            icon: 'help',
                            to: '/help'
                        }
                    ]
                }
            }
        },
        mounted() {
            window._bd_share_config = {
                "common": {
                    "bdSnsKey": {
                        "tsina": "1250085586",
                        "tqq": "Vk8EikNNx5myYfSX"
                    },
                    "bdText": "123", // 分享文案
                    "bdMini": "2", // 分享图片
                    "bdMiniList": false,
                    "bdPic": "",
                    "bdStyle": "1",
                    "bdSize": "24"
                },
                "share": {},
                //"image": {"viewList": ["tsina", "tqq", "qzone", "renren"], "viewText": "分享云设工具到：", "viewSize": "16"}
            };
            let elem = document.getElementsByTagName('head')[0]
            elem.appendChild(document.createElement('script')).src = 'http://bdimg.share.baidu.com/static/api/js/share.js?v=86835285.js?cdnversion=' + (new Date().getTime() / 36e5)
        }
    }
</script>

<style scoped>
</style>

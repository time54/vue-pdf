<template>
  <div class="pdfDemo">
    <v-pdf :pdfUrl="pdfUrl"></v-pdf>
  </div>
</template>
<script>
    import pdf from './pdf'

    export default {
        data() {
            return{
                //  pdfUrl: '../../static/test.pdf'//本地调试
                pdfUrl: 'http://khtest.10jqka.com.cn/dev/taojinchao/vuepdf/dist/test.pdf',//pdf url地址 
            }
        },
        components: {
            'v-pdf': pdf
        }
    }
</script>
<style>
    .pdfDemo{
        border: 2px solid aqua;
    }
</style>



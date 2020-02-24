<template>
    <div>
        <table>
            <tr>
                <td>编号</td>
                <td>图书名称</td>
                <td>作者</td>
            </tr>
            <tr v-for="item in books">
                <td>{{item.id}}</td>
                <td>{{item.name}}</td>
                <td>{{item.author}}</td>
            </tr>

        </table>
    </div>
</template>

<script>
    export default {
        name: "Book",
        data(){
            return {
                msg:'hellovue',
                books:[
                    {
                        id: 1,
                        name: 'Java0',
                        author: 'lzp'
                    },
                    {
                        id:2,
                        name:'Java2',
                        author:'lzp2'
                    },
                    {
                        id:3,
                        name:'Java3',
                        author:'lzp3'
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>
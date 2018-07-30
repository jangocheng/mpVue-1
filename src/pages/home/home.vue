<template>
    <div>
        我是首页
    </div>
</template>

<script>
import {get} from './../../util.js'
import {formatTime} from './../../utils'
export default {
    async created () {
        const res = await get("/weapp/demo")
        console.log("demo=>",res)
        console.log("data=>",Date())
        console.log("data=>", formatTime(new Date(Date.now()) ))
    }
}
</script>
<style>

</style>

<template>
  <div >
    <img alt="emoji" :src="emoji" style="width:200px" id="imgid">
  </div>
</template>

<script>
export default {
  name: 'MyEmoji',
  data(){
    return{
      emoji:'',
      emojiList:[
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E4%BA%B2%E4%BA%B2.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/666.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E5%8F%AF%E7%88%B1.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E5%90%83%E7%93%9C.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E5%93%88%E6%AC%A0.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E5%A5%BD%E7%9A%84.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E5%AE%B3%E7%BE%9E.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E6%9C%BA%E6%99%BA.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E8%B0%83%E7%9A%AE.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E9%85%B7.svg',
        'https://emoji-e726.obs.cn-east-3.myhuaweicloud.com/kebiao/%E9%BE%87%E7%89%99.svg']
    }
  },
  mounted(){
    this.emoji = this.emojiList[Math.floor(Math.random() * this.emojiList.length)]
  },

}
</script>
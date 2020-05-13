<template>
  <div>
    <button @click="onClick()">Yeah!!!</button>
    <notifications group="page1" />
    <div>{{ $dateTimeToJaDate('2020-05-13T12:53:17+09:00') }}</div>
    <flag iso="us" />
  </div>
</template>

<script>


export default {
methods: {
    onClick: function(){
      this.$notify({ group: 'page1', text: 'Yeah !!!' })
    }
  }
}
</script>


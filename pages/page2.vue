<template>
  <div>
    <button @click="onClick()">Heyy !!!</button>
    <notifications group="page2" />
    <div>{{ $dateTimeToJaDate('2019-02-27T12:53:17+09:00') }}</div>
    <flag iso="jp" />
  </div>
</template>

<script>


export default {
methods: {
    onClick: function(){
      this.$notify({ group: 'page2', text: 'Heyy !!!' })
    }
  }
}
</script>
<template>
    <div>
        <div class="col-xs-12 col-sm-6">
            <p> {{ contentMessage }} </p>
        </div>
        
    </div>
</template>

<script>
  export default {
    data: function() {
      return {
        contentMessage: 'Server Details are currently not updated'
      }
    }
  }
</script>

<style>
</style
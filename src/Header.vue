<template>
    <div>
        <div class="row">
            <div class="col-xs-12">
                <header>
                    <h1>{{ headMessage }}</h1>
                </header>
            </div>
        </div>
    </div>
</template>

<script>
  export default {
    data: function() {
      return {
        headMessage: 'Server Status'
      }
    }
  }
</script>

<style>
</style
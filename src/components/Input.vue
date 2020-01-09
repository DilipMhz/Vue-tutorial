<template>
<div>
  <input :type="type" placeholder= "enter text"/>
</div>

</template>
<script>

  export default {
    props:{
      type: {
        type: String,
        default: "text"

      }
    }
  }
  </script>

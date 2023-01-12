<template>
  <input class="text-input" :type="type ? type : 'text'" :placeholder=placeholder :id="id" :required=required />
</template>

<script>
export default {
  name: "TextInput",
  props: {
    placeholder: String,
    id: String,
    required: Boolean,
    type: String
  }
}
</script>
<template>
  <div class="form__item" :class="[
              ($slots.captcha ? 'form__item_with-captcha' : false),
              (valign === 'bottom' && 'form__item_valign-bottom')
          ]">
    <slot>
      <label class="form__label" v-if=label :for=id>{{ label }}</label>
      <div class="form__input-block">
        <TextInput :id=id :placeholder=placeholder :required=required :type="type" />
        <div class="form__captcha" v-if="$slots.captcha">
          <slot name="captcha"></slot>
        </div>
      </div>
    </slot>
  </div>
</template>

<script>
import TextInput from "@/components/elements/TextInput";

export default {
  name: "FormItem",
  components: {TextInput},
  props: {
    placeholder: String,
    label: String,
    id: String,
    required: Boolean,
    type: String,
    valign: String
  }
}
</script>
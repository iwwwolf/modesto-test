<template>
  <FormComponent>
    <template v-if="currentStep == 1">
      <FormItem id="userName" label="Ваше имя" placeholder="Фролова Александра Васильевна" required />
      <FormItem id="companyName" label="Название Компании" placeholder="ООО Атлантика" required />
      <FormItem id="userEmail" label="E-mail" type="email" placeholder="flolovaalexa@com.rur" required />
      <FormItem id="userPhone" label="Номер телефона" placeholder="+7 (XXX) - XXX XX XX" required />
      <FormItem id="promoCode" label="Промокод" placeholder="HGF864" />
      <FormItem valign="bottom">
        <ButtonsBlock>
          <ButtonComponent variant="primary" @click.prevent="goToStep(2)">Далее</ButtonComponent>
        </ButtonsBlock>
      </FormItem>
    </template>
    <template v-if="currentStep == 2">
      <FormItem id="passwordInput" type="password" label="Пароль" placeholder="Создайте пароль" required />
      <FormItem id="confirmPasswordInput" type="password" label="Подтвердите пароль" placeholder="Повторите пароль" required />
      <FormItem id="captchaInput" label="Введите символы из картинки" placeholder="Код из картинки" required>
        <template v-slot:captcha>
          <img src="../assets/images/captcha.png" />
        </template>
      </FormItem>
      <FormItem valign="bottom">
        <ButtonsBlock>
          <ButtonComponent class="form__button-back" variant="secondary" @click.prevent="goToStep(1)">Назад</ButtonComponent>
          <ButtonComponent variant="primary">Отправить</ButtonComponent>
        </ButtonsBlock>
      </FormItem>
      <FormItem class="form__agreement">
        <CheckboxInput name="agreement" id="agreeInput">
          Я даю согласие на обработку моих персональных данных и правовых документов
        </CheckboxInput>
      </FormItem>
    </template>
  </FormComponent>
</template>

<script>
import FormItem from "@/components/elements/FormItem";
import FormComponent from "@/components/elements/FormComponent";
import ButtonComponent from "@/components/elements/ButtonComponent";
import ButtonsBlock from "@/components/elements/ButtonsBlock";
import CheckboxInput from "@/components/elements/CheckboxInput";

export default {
  name: "RegistrationForm",
  components: {
    CheckboxInput,
    ButtonsBlock,
    ButtonComponent,
    FormComponent,
    FormItem
  },
  data(){
    return {
      currentStep: 1,
    };
  },
  methods: {
    goToStep: function(step) {
      this.currentStep = step;
    }
  }
}
</script>

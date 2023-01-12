<template>
  <section class="form-section" id="registrationSection">
    <div class="main-container">
      <div class="form-section__content">
        <div class="form-section__text">
          <h2>Заполните форму и начните развивать свой бизнес прямо сейчас!</h2>
          <p>
            Регистрация на нашем сайте занимает несколько минут, просим ответить на все вопросы полностью и корректно!
            После подтверждения регистрации вы попадёте в систему, где большинство процессов автоматизированы,
            что сэкономит ваше время и деньги!
          </p>
        </div>
        <RegistrationForm />
      </div>
    </div>
  </section>
</template>

<script>
import RegistrationForm from '@/components/RegistrationForm.vue';

export default {
  name: "FormSection",
  components: {
    RegistrationForm
  }
}
</script>
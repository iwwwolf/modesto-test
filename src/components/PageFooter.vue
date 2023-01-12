<template>
  <footer class="footer">
    <div class="main-container">
      <div class="footer__content">
        <div class="footer__column">
          <h3>Наши офисы</h3>

          <ul class="footer__offices footer__list">
            <li>
              <address>
                Московский офис <br />
                <a href="tel:+74552678907">+7 455 267-89-07</a> <br />
                Берсеневский пер., д. 56, стр. 4, <br />
                6-й эт., Москва, 567754
              </address>
            </li>
            <li>
              <address>
                Ростовский офис <br />
                <a href="tel:+78788880167">+7 878 888-01-67</a> <br />
                Буденовский пр-т, д. 84, 6-й эт., <br />
                Ростов-на-Дону, 679965
              </address>
            </li>
          </ul>
        </div>

        <div class="footer__column">
          <h3>Мы в соц сетях</h3>

          <ul class="footer__list">
            <li><a href="#">Instagram</a></li>
            <li><a href="#">Facebook</a></li>
          </ul>
        </div>

        <div class="footer__column">
          <h3>Свяжитесь с нами</h3>

          <ul class="footer__list">
            <li>
              <a href="tel:+36787547894">+3 67 8754 7894</a>
            </li>
            <li>
              <a href="mailto:mflowers@flo.com">mflowers@flo.com</a>
            </li>

            <li>
              <ButtonComponent href="mailto:mflowers@flo.com" variant="primary">
                Написать
                <template v-slot:icon>
                  <svg width="20" height="16" viewBox="0 0 20 16" fill="none">
                    <path d="M5.28918 0.907613C8.42382 0.635125 11.5762 0.635125 14.7108 0.907613L16.2211 1.03889C17.2264 1.12629 18.0875 1.72596 18.5337 2.58374C18.5907 2.69347 18.5479 2.82633 18.4428 2.89144L12.1768 6.77037C10.833 7.60228 9.13844 7.61974 7.77772 6.81568L1.46989 3.08833C1.36798 3.02811 1.3212 2.90415 1.36713 2.79505C1.77529 1.82548 2.69292 1.1333 3.77895 1.0389L5.28918 0.907613Z" fill="black"/>
                    <path d="M1.362 4.76688C1.20603 4.67472 1.00703 4.7739 0.988851 4.95414C0.735115 7.46977 0.796526 10.0092 1.17308 12.5133C1.3716 13.8334 2.44901 14.8455 3.77895 14.9611L5.28918 15.0924C8.42382 15.3649 11.5762 15.3649 14.7108 15.0924L16.2211 14.9611C17.551 14.8455 18.6284 13.8334 18.8269 12.5133C19.2145 9.93625 19.2682 7.32174 18.9882 4.73428C18.9685 4.55276 18.7662 4.45541 18.6109 4.55151L12.9664 8.04576C11.1482 9.1713 8.8556 9.19492 7.01462 8.10707L1.362 4.76688Z" fill="black"/>
                  </svg>
                </template>
              </ButtonComponent>
            </li>
          </ul>
        </div>
      </div>
      <div class="footer__copyright">
        Авторские права 2008-2022 M-flowers.com
      </div>
    </div>
  </footer>
</template>

<script>
import ButtonComponent from "@/components/elements/ButtonComponent";
export default {
  name: "PageFooter",
  components: {ButtonComponent}
}
</script>
<template>
  <section id="contacts" ref="contacts">
    <div class="container">
      <p
        class="section-name"
        v-motion
        :initial="{ opacity: 0, x: -50 }"
        :visible="{ opacity: 1, x: 0, transition: {duration: 400, delay: 100}}"
      >/{{texts.headerContacts[store.state.lang]}}</p>
      <h2
        class="title"
        v-motion
        :initial="{ opacity: 0, y: -50 }"
        :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 200}}"
      >{{texts.contactsTitle[store.state.lang]}}</h2>
      <div class="contacts-inner">
        <div
          class="contacts-item"
          v-motion
          :initial="{ opacity: 0, scale: .5 }"
          :visible="{ opacity: 1, scale: 1, transition: {duration: 400, delay: 300}}">
          <div
            class="icon"
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="34" viewBox="0 0 30 34" fill="none">
              <path
                d="M20.7992 30.058V26.4213C20.8469 25.8171 20.765 25.2096 20.5591 24.6394C20.3531 24.0692 20.0279 23.5492 19.605 23.114C23.5943 22.6705 27.7869 21.1626 27.7869 14.244C27.7865 12.4749 27.1042 10.7736 25.8812 9.49223C26.4602 7.94443 26.4193 6.23358 25.7668 4.7151C25.7668 4.7151 24.2676 4.2716 20.7992 6.59047C17.8873 5.80335 14.8178 5.80335 11.9058 6.59047C8.43737 4.2716 6.9382 4.7151 6.9382 4.7151C6.28564 6.23358 6.24469 7.94443 6.82386 9.49223C5.59164 10.7831 4.90862 12.4998 4.91813 14.282C4.91813 21.15 9.11072 22.6579 13.1 23.152C12.6821 23.5829 12.3597 24.0966 12.1539 24.6598C11.9482 25.2231 11.8636 25.8233 11.9058 26.4213V30.058"
                stroke="black" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M12.0492 27.3876C8.25526 28.5994 5.09367 27.3876 3.19672 23.6521" stroke="black"
                    stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </div>
          <div
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <p>Github</p>
            <a target="_blank" href="https://github.com/mlutfullaev">@mlutfullaev</a>
          </div>
        </div>
        <div
          class="contacts-item"
          v-motion
          :initial="{ opacity: 0, scale: .5 }"
          :visible="{ opacity: 1, scale: 1, transition: {duration: 400, delay: 300}}">
          <div
            class="icon"
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <svg xmlns="http://www.w3.org/2000/svg" width="34" height="34" viewBox="0 0 34 34" fill="none">
              <path
                d="M27.6997 4.24596C27.3428 4.26256 27.0066 4.36632 26.7078 4.48254H26.7036C26.4006 4.6029 24.9605 5.20885 22.7732 6.12609C20.5859 7.04748 17.7471 8.24279 14.929 9.4298C9.30103 11.7997 3.76856 14.1322 3.76856 14.1322L3.83496 14.1073C3.83496 14.1073 3.45313 14.2318 3.05469 14.5057C2.85132 14.6385 2.6272 14.8212 2.43213 15.1075C2.23706 15.3939 2.07935 15.8339 2.13745 16.2862C2.23291 17.0541 2.73096 17.5148 3.08789 17.7679C3.44898 18.0253 3.79346 18.1456 3.79346 18.1456H3.80176L8.98975 19.8929C9.22217 20.64 10.571 25.0726 10.8948 26.0936C11.0857 26.7037 11.2725 27.0856 11.5049 27.3761C11.6169 27.5255 11.7498 27.65 11.9075 27.7496C11.9697 27.787 12.0361 27.816 12.1025 27.8409C12.1233 27.8534 12.144 27.8575 12.1689 27.8617L12.115 27.8492C12.1316 27.8534 12.144 27.8658 12.1565 27.87C12.198 27.8824 12.2271 27.8866 12.281 27.8949C13.1028 28.1439 13.7627 27.6334 13.7627 27.6334L13.8001 27.6044L16.863 24.8153L21.9971 28.754L22.1133 28.8038C23.1841 29.2728 24.2673 29.0113 24.8401 28.5506C25.417 28.0858 25.6411 27.4923 25.6411 27.4923L25.6785 27.3968L29.6462 7.07238C29.7583 6.57018 29.7874 6.10119 29.6628 5.64464C29.5383 5.1881 29.2188 4.76061 28.8328 4.53234C28.4426 4.29992 28.0566 4.22936 27.6997 4.24596ZM27.5918 6.42492C27.5876 6.49132 27.6001 6.48302 27.571 6.61168V6.62414L23.6406 26.7369C23.624 26.766 23.595 26.8282 23.5161 26.8905C23.4331 26.9569 23.3667 26.9984 23.0222 26.8614L16.7427 22.047L12.9492 25.5043L13.7461 20.4159C13.7461 20.4159 23.5825 11.2477 24.0059 10.8534C24.4292 10.4591 24.2881 10.3761 24.2881 10.3761C24.3171 9.89464 23.6489 10.235 23.6489 10.235L10.7122 18.2494L10.708 18.2286L4.50733 16.141V16.1368C4.50318 16.1368 4.49488 16.1327 4.49073 16.1327C4.49488 16.1327 4.52393 16.1202 4.52393 16.1202L4.55713 16.1036L4.59033 16.0912C4.59033 16.0912 10.127 13.7587 15.7549 11.3888C18.573 10.2018 21.4119 9.00646 23.595 8.08507C25.7781 7.16784 27.3926 6.49547 27.4839 6.45812C27.571 6.42492 27.5295 6.42492 27.5918 6.42492Z"
                fill="black"/>
            </svg>
          </div>

          <div
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <p>Telegram</p>
            <a target="_blank" href="https://t.me/mlutfullaev">@mlutfullaev</a>
          </div>
        </div>
        <div
          class="contacts-item"
          v-motion
          :initial="{ opacity: 0, scale: .5 }"
          :visible="{ opacity: 1, scale: 1, transition: {duration: 400, delay: 300}}">
          <div
            class="icon"
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32" fill="none">
              <path
                d="M26.7114 27.8326H5.25315C2.45333 27.8326 0.175827 25.5551 0.175827 22.7553V9.20867C0.175827 6.4092 2.45368 4.13135 5.25315 4.13135H26.7114C29.5108 4.13135 31.7883 6.4092 31.7883 9.20867V22.7553C31.7883 25.5551 29.5108 27.8326 26.7114 27.8326ZM5.25315 5.61608C3.2721 5.61608 1.66056 7.22762 1.66056 9.20867V22.7553C1.66056 24.7364 3.2721 26.3483 5.25315 26.3483H26.7114C28.6924 26.3483 30.3039 24.7364 30.3039 22.7553V9.20867C30.3039 7.22762 28.6924 5.61608 26.7114 5.61608H5.25315Z"
                fill="#1D1D1B"/>
              <path
                d="M4.05504 9.27923C7.84994 12.9772 11.6448 16.6748 15.4398 20.3728C16.1472 21.0619 17.2329 19.9787 16.5244 19.2881C12.7295 15.5905 8.9346 11.8925 5.1397 8.19492C4.43228 7.50542 3.34656 8.58903 4.05504 9.27923Z"
                fill="#1D1D1B"/>
              <path
                d="M16.5244 20.3727C20.3193 16.6751 24.1142 12.9771 27.9091 9.27954C28.6172 8.58933 27.5322 7.50537 26.8245 8.19488C23.0296 11.8925 19.2347 15.5904 15.4397 19.2881C14.7316 19.9783 15.8166 21.0622 16.5244 20.3727Z"
                fill="#1D1D1B"/>
              <path
                d="M27.8673 22.9904C25.3422 20.5955 22.8167 18.2011 20.2916 15.8062C19.5754 15.1273 18.4889 16.2098 19.2069 16.8909C21.732 19.2857 24.2575 21.6802 26.7827 24.075C27.4989 24.754 28.5853 23.6711 27.8673 22.9904Z"
                fill="#1D1D1B"/>
              <path
                d="M5.24999 24.0746C7.77513 21.6798 10.3006 19.2853 12.8258 16.8905C13.5434 16.2098 12.4576 15.1265 11.7411 15.8059C9.21595 18.2007 6.69047 20.5951 4.16533 22.99C3.44773 23.6707 4.53344 24.7543 5.24999 24.0746Z"
                fill="#1D1D1B"/>
            </svg>
          </div>
          <div
            v-motion
            :initial="{ opacity: 0, y: -20 }"
            :visible="{ opacity: 1, y: 0, transition: {duration: 400, delay: 600}}">
            <p>Mail</p>
            <a target="_blank" href="mailto:mhoja9494@gmail.com">mhoja9494@gmail.com</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
@import '@/assets/variables';

#contacts {
  background: #f1f1f1;

  .contacts-inner {
    display: flex;
    gap: 20px;
    justify-content: center;
    align-items: center;
    padding: 40px 0;

    @media (max-width: 900px) {
      flex-wrap: wrap;
    }

    .contacts-item {
      display: flex;
      gap: 10px;
      padding: 10px;
      border-radius: 50px;
      align-items: center;
      justify-content: center;
      background: #fff;

      .icon {
        border-radius: 50%;
        width: 50px;
        height: 50px;
        padding: 5px;
        display: flex;
        align-items: center;
        justify-content: center;
        background: #fff;
        box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.15);
      }

      > div {
        padding-right: 15px;

        > p {
          font-size: 20px;
          font-weight: 500;

          @media (max-width: 350px) {
            font-size: 18px;
          }
        }

        > a {
          transition: .2s;

          &:hover {
            color: $second-color;
          }

          @media (max-width: 350px) {
            font-size: 15px;
          }
        }
      }
    }
  }
}
</style>
<script lang="ts" setup>
import store from '@/store/index'
import texts from '@/texts.json'
</script>

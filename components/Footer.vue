<template>
  <footer class="footer">
    <div class="footer-contact">
      <div class="footer-contact-content container ">
        <div class="footer-contact-social">
        <img src="/img/logo.png" alt="logo" class="footer-contact-social-logo"/>
        <ul class="footer-contact-social-list">
          <li>
            <a>
              <img src="/img/icon_twiter.png" alt=""/>
            </a>
          </li>
          <li>
            <a>
              <img src="/img/icon_fb.png" alt=""/>
            </a>
          </li>
          <li>
            <a>
              <img src="/img/icon_inst.png" alt=""/>
            </a>
          </li>
        </ul>
      </div>
      <div class="footer-contact-info">
        <h5 class="footer-contact-info-title">Address</h5>
        <div class="footer-contact-info-wrap">
          <img src="/img/icon_address.png" class="first-icon">
          <p class="footer-contact-info-desc">Valletta Buildings, South Street, Valletta - VLT 1103 Malta, US <br> 20 Phan Dang Luu street, Hai Chau District, Danang city, Vietnam</p>
        </div>
        <div class="footer-contact-info-wrap">
          <img src="/img/icon_phone.png" class="second-icon">
          <p class="footer-contact-info-desc">(+1) 555-0108-000 or (+236) 555-0108</p>
        </div>
      </div>
      <div class="footer-contact-subcribe">
        <h5 class="footer-contact-info-title">Subscribe</h5>
        <p class="footer-contact-subcribe-desc">Subscribe to our newsletter and be the first to know about our updates</p>
        <input class="footer-contact-subcribe-input" placeholder="Enter your email" />
      </div>
      </div>
    </div>
    <div class="footer-author">
      <p class="footer-author-desc">2017 Copyright. Policy.</p>
    </div>
  </footer>
</template>

<style scoped lang="scss">
  .footer {
    padding: 0;

    &-contact {
      background-image: url('/img/bg_footer.jpg');
      background-size: cover;
      background-position: center;
      padding: 104px 0;

      &-content {
        display: flex;
        flex-direction: row;
        justify-content: space-between;

        ul {
          display: flex;
          flex-direction: row;

          li {
            margin-right: 32px;
          }
        }
      }

      &-social {
        &-logo {
          margin-bottom: 30px;
        }
      }

      &-info,
      &-subcribe {
        max-width: 410px;

        &-title {
          font-weight: bold;
          font-size: 24px;
          line-height: 30px;
          color: #fff;
          margin-bottom: 40px;
        }

        &-desc {
          font-size: 14px;
          line-height: 20px;
          color: #fff;

        }
      }

      &-info {
        &-desc {
          margin-bottom: 40px;
        }

        &-wrap {
          display: flex;
          flex-direction: row;
        }

        .first-icon {
          width: 30px;
          height: 34px;
          margin-right: 13px;
        }

        .second-icon {
          width: 26px;
          height: 34px;
          margin-right: 13px;
        }
      }

      &-subcribe {
        &-desc {
          margin-bottom: 12px;
        }

        &-input {
          width: 100%;
          height: 56px;
          border: 1px solid #fff;
          background: transparent;
          border-radius: 8px;
          outline: none;
          color: #fff;
          padding: 20px;
        }
      }

      &-input::placeholder {
        color: #fff;
      }
    }

    &-author {
      background-color: #000;
      padding: 30px 27px;

      &-desc {
        font-size: 18px;
        line-height: 126%;
        text-align: center;
        color: #fff;
      }
    }
  }

  @media (max-width: 768px) {
    .footer {
      &-contact {
        padding: 40px 16px;

        &-content {
          flex-direction: column;
        }

        &-social {
          text-align: center;

          &-list {
            justify-content: center;
          }
        }

        &-info {
          margin-top: 65px;

          &-title {
            margin-bottom: 22px;
          }
        }

        &-subcribe {
          margin-top: 65px;
        }
      }
    }
  }
</style>

<script>
export default {}
</script>

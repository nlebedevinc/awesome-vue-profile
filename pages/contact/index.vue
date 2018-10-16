<template>
  <section class="container">
    <header-logo />
    <div class="content">
      <div class="profile-card">
        <div class="profile-image">
          <img
            src="https://pp.userapi.com/c630420/v630420271/3c85e/2E0xR6-Z9Nc.jpg"
            alt=""/>
        </div>
      </div>
      <div class="form-container">
        <form>
          <div class="field">
            <label>Name</label>
            <input class="field-input" />
          </div>
          <div class="field">
            <label>Email</label>
            <input class="field-input" />
          </div>
          <div class="field">
            <label>Message</label>
            <textarea class="field-textarea"></textarea>
          </div>
          <div class="submit">
            <input type="submit" class="btn-submit"/>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
import HeaderLogo from '~/components/Header'

export default {
  components: {
    HeaderLogo
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  padding-top: 15px;
  padding-bottom: 15px;
  @media only screen and (min-device-width : 1200px) {
    max-width: 1035px;
    margin-top: 20px;
    margin-bottom: 20px;

    .profile-card {
      width: 300px;
    }

    .form-container {
      width: 700px;
    }
  }

  .profile-card {
    padding-left: 5px;
    height: 100px;
    float: left;
  }

  .form-container {
    height: 100px;
    padding-right: 5px;
    float: right;
  }

  .content {
    clear: both;
    padding: 50px 0;
  }

  .profile-image {
    max-height: 300px;
    overflow: hidden;
  }

  .field {
    margin-bottom: 24px;
    input, textarea {
      width: 100%;
      border-radius: 2px;
      background: #fafafa;
      font-size: 14px;
      margin-top: 6px;
      margin-bottom: 4px;
      padding: 10px;
    }

    .field-input {
      box-sizing: border-box;
      line-height: normal;
    }

    .field-textarea {
      min-height: 100px;
    }
  }

  .btn-submit {
    background-color: #272727;
    color: #fff;
    border: none;
    padding: 1em 2.5em;
    font-size: 14px;
    text-transform: uppercase;
    cursor: pointer;
  }
}
</style>

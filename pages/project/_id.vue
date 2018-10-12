<template>
  <section class="container">
    <header-logo />
    <div class="content">
      <div class ="image-container">
        <img
            src="https://i.ytimg.com/vi/sTGeC0IYeOU/maxresdefault.jpg"
            alt=""/>
      </div>
      <div class="description-container">
        <div class="description">
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
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
  }

  .content {
    clear: both;
    padding: 50px 0;
  }

  .image-container {
    margin: 0 auto;
    height: 400px;
    overflow: hidden;
  }

  .description-container {
    padding-top: 30px;
    .description {
      font-size: 20px;
      color: #43484c;
      margin: 0 auto;
      width: 770px;
      height: 400px;

      p {
        margin: 25px 0;
      }
    }
  }
}
</style>

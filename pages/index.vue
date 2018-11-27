<template>
  <div class="main-bg">
    <section class="container">
      <b-row>
        <b-col :md="3" class="mb-4" v-for="item in 16">
          <b-card
            img-src="https://picsum.photos/600/300/?image=25"
            img-alt="Image"
            img-top
            tag="article"
          >
            <p class="card-text">
              Some quick example text to build on the card
            </p>
            <div class="card-btn-group">
                <b-button href="#">View</b-button>
                <ul class="social-share">
                    <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                    <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
                    <li><a href="#"><i class="fa fa-dribbble"></i></a></li>
                    <li><a href="#"><i class="fa fa-skype"></i></a></li>
                </ul>
            </div>
          </b-card>
        </b-col>
      </b-row>
    </section>
  </div>
</template>

<script>
  export default {
    components: {}
  };
</script>

<style lang="scss">
  .main-bg {
    background: #454545;
    padding: 30px 0;
  }
  .card-btn-group{
    display: flex;
    justify-content: space-between;
    align-items: center;
    ul{
      list-style: none;
      margin-bottom: 0;
      >li{
        display: inline-block;
        vertical-align: middle;
        margin-right: 5px;
      }
      .fa{
        color: #6c757d;
      }
    }
  }
</style>

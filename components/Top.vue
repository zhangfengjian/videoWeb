<template>
  <div class="nav-wrap">
    <div class="nav">
      <div class="container">
          <a class="navbar-brand" href="index.html">
            <i class="fa fa-fa fa-cubes"></i>AppBox
          </a>
          <b-btn v-b-toggle.collapseMenu>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
          </b-btn>
          <b-nav>
            <b-nav-item active>Active</b-nav-item>
            <b-nav-item>Link</b-nav-item>
            <b-nav-item>Another Link</b-nav-item>
            <b-nav-item>Disabled</b-nav-item>
          </b-nav>
      </div>
    </div>
    <div class="nav-list">
      <b-collapse id="collapseMenu">
          <b-nav vertical>
            <b-nav-item active>Active</b-nav-item>
            <b-nav-item>Link</b-nav-item>
            <b-nav-item>Another Link</b-nav-item>
            <b-nav-item>Disabled</b-nav-item>
          </b-nav>
      </b-collapse>
    </div>
  </div>
</template>
<script>
  export default {};
</script>
<style lang="scss">
.nav-wrap{
  .nav{
    background: #151515;
    padding: 10px 0;
    .container{
      display: flex;
      justify-content: space-between;
      .nav-link{
        color: #fff;
        &.active{
          background: #555;
          border: 1px solid #333;
          border-radius: 4px;
        }
      }
      @media (max-width: 768px){
        .nav{
          display: none;
        }
      }
    }
    .navbar-brand{
      color: #fff;
      font-size: 1.25rem;
    }
    @media (min-width: 768px){
      .btn-secondary{
        display: none
      }
    }
    .btn-secondary{
      align-self:center;
      background-color: transparent;
      border: 1px solid #333;
      border-radius: 4px;
      padding: 9px 10px;
      .icon-bar{
        display: block;
        width: 22px;
        height: 2px;
        border-radius: 1px;
        background-color: #fff;
        &+.icon-bar{
          margin-top: 4px;
        }
      }
      &:focus{
        box-shadow: none;
      }
    }
    .btn-secondary:not(:disabled):not(.disabled):active{
      box-shadow: none;
      background-color: transparent;
    }
  }
  .nav-list{
    border-top: 1px solid #343434;
    .nav-link{
        color: #fff;
    }
  }
}
</style>

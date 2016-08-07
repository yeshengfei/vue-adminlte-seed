<template>
  <div class="wrapper">
    <main-header></main-header>
    <main-sidebar></main-sidebar>
    <div class="content-wrapper" >
      <router-view></router-view>
    </div>
    <main-footer></main-footer>
    <control-sidebar></control-sidebar>
    <!-- Add the sidebar's background. This div must be placed
       immediately after the control sidebar -->
    <div class="control-sidebar-bg"></div>
  </div>
</template>

<script>
import MainHeader from './components/common/MainHeader'
import MainSidebar from './components/common/MainSidebar'
import MainFooter from './components/common/MainFooter'
import ControlSidebar from './components/common/ControlSidebar'

export default {
  components: {
    MainHeader,
    MainSidebar,
    MainFooter,
    ControlSidebar
  }
}
</script>

<style lang="less">
  .wrapper {
    min-height: 600px;
  }

</style>

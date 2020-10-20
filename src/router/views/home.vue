<script>
import appConfig from '@src/app.config'
import Layout from '@layouts/main.vue'
import AuthModal from '@components/Modals/AuthModal.vue'

export default {
  page: {
    title: 'Home',
    meta: [{ name: 'description', content: appConfig.description }],
  },
  components: { AuthModal, Layout },
}
</script>

<template>
  <Layout>
    <AuthModal />
    <h1>Home Page</h1>
    <img src="@assets/images/logo.png" alt="Logo" />
  </Layout>
</template>

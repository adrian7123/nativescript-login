<template>
<Page>
    <ActionBar class="actionBar" text="Login"/>
    <FlexboxLayout flexDirection="column" alignItems="center" class="main">
        <Label class="title" text="Faça seu Login" textWrap="true" />
        <Image class="img" tintColor="#2DD881" :src="logo" />
        <Form />
    </FlexboxLayout>
</Page>
</template>

<script>
import Form from '../components/Form'

export default {
    data() {
        return {
            logo: '~/assets/img/logo.png'
        }
    },
    components: {
        Form
    }
}
</script>

<style scoped lang="scss">
    @import '../assets/sass/Home';
</style>

<template>
  <StackLayout>
    <TextField hint="Email" v-model="emailText" keyboardType="email" focus="true" />
    <TextField hint="Senha" v-model="senhaText" secure="true" keyboardType="password" />
    <Button text="Login" @tap="click()"/>
    <FlexboxLayout justifyContent="space-between">
        <Label text="esqueceu a senha?"/>
        <Label text="cadastre-se"/> 
        
    </FlexboxLayout>
  </StackLayout>
</template>

<script>
import Users from '@/views/Users'

export default {
    name: 'Form',
    data() {
        return {
            emailText: '',
            senhaText: '',
        }
    },
    methods: {
        click() {
            console.log('clicado')
        }
    }

}
</script>

<style scoped lang="scss">
    @import '../assets/sass/Form';

</style>
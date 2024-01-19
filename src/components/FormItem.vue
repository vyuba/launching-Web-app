<script>
    export default{
        data(){
            return{
                message: ''
            }
        },
        methods:{
            showAlert(){
                alert('email has been sent to ' + this.message)
            }
        },
        mounted(){
            // this.showAlert()
        }
    }
</script>

<template>
    <form id="form">

        <p>Get notified when we launched our website</p>

        <div class="form-group">
            <input v-model="message" type="text" class="form-control" placeholder="Your email address">
            <button @click ="showAlert" type="button" class="submit-button"><i class="icon icon-envelope"></i><span>NOTIFY ME</span></button>
        </div>

    </form>
</template>
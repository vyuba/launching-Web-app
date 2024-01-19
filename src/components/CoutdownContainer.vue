<script setup>
  import CountdownItem from './CountdownItem.vue';
</script>


<script>
export default{
    data(){
        return{
            preye: '',
            today: '',
            day:'',
            hours:'',
            minutes:'',
            seconds:'',
        }
    },
    methods:{
        timeFunction(){
            const today = new Date();
            this.today = today
            console.log(this.today)
            const day = today.getDate()
            this.day = day
            console.log(this.day);
            const hours = today.getHours()
            this.hours = hours
            const minutes = today.getMinutes()
            this.minutes = minutes
            const seconds = today.getSeconds()
            this.seconds = seconds

            if (this.seconds < 10) {
                this.seconds ='0' + this.seconds
            }
            if (this.minutes < 10) {
                this.minutes ='0' + this.minutes
            }
            if (this.hours < 10) {
                this.hours ='0' + this.hours
            }
        },
        
    },
    mounted(){
        this.timeFunction()
        setInterval(this.timeFunction, 1000)
    }
}
</script>
<template>
        <div id="countdown-clock">
            <CountdownItem>
                {{ hours }}
                <small>hours</small>
            </CountdownItem>
            <CountdownItem>
                {{ minutes }}
                <small>minutes</small>
            </CountdownItem>
            <CountdownItem>
                {{ seconds }}
                <small>seconds</small>
            </CountdownItem>
        </div>
   
</template>
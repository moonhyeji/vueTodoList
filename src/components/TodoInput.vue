<template>
<div>
    <input type="text" v-model="newTodoItem">
    <button @click="addTodo">할일 추가</button>
</div>    
</template>
<script>
export default {
    data(){
        return{
            newTodoItem: ''
        }
    },
    methods:{
        addTodo(){
            if(this.newTodoItem && this.newTodoItem !== ""){
                var value = this.newTodoItem && this.newTodoItem.trim()
                localStorage.setItem(value,value)
                this.clearInput();
        }   
           // localStorage.setItem(this.newTodoItem, this.newTodoItem)
        },
        clearInput(){
            this.newTodoItem = "";
        }
    }
}
</script>
<style>
</style>
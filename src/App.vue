<template> 
<div id="app">
    <TodoHeader></TodoHeader>
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>

</div>

</template>
<script>
import TodoFooter from './components/TodoFooter.vue'
import TodoHeader from './components/TodoHeader.vue'
import TodoInput from './components/TodoInput.vue'
import TodoList from './components/TodoList.vue'



export default {
    components:{
        'TodoHeader' : TodoHeader,
        'TodoFooter' : TodoFooter,
        'TodoInput' : TodoInput,
        'TodoList' : TodoList
    }

}
</script>
<style>
body{
  text-align: center;
  background-color: #F6F6F8;
}
input{
  border-style: groove;
  width: 200px;
}
button{
  border-style: groove; /*groove 테두리가 창(canvas)에서 조각(파진)된 것처럼 보임*/
  margin-left: 5px;
}
.shadow{
  box-shadow: 5px 10px 10px rgba(0, 0, 0, 0.03);
}
</style>
<template>
  <div class="container">
    <h1 class="text-center pb-2">{{ttl}}</h1>
    <form @submit.prevent="">
      <div class="form-group">
        <label for="name">名前</label>
        <input type="text" class="form-control" id="name" v-model="data.name" @change="createMessage()">
      </div>
      <div class="form-group">
        <label for="student_id">学生番号</label>
        <input type="text" class="form-control" v-model="data.student_id" id="student_id" @change="createMessage()">
      </div>
      <div class="form-group pt-2">
        <button class="btn btn-primary btn-lg btn-block" id="send" type="submit">送信</button>
      </div>
    </form>
  </div>

</template>

<script>
export default {
  name: 'InputForm',
  props: {
    ttl: String
  },
  data(){
    return {
      data: {
        name: '',
        student_id: '',
      }
    }
  }
};
</script>
<style>
</style>

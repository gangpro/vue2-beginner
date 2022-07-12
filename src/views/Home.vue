<template>
  <div>
    <h1>Welcome to {{ title }}!</h1>
    <h2>Welcome to {{ subTitle }}!</h2>
    <hr>
    <!-- 데이터 바인딩은 v-model -->
    <input type="text" v-model="inputVal" /> <!-- v-model = value -->
    <button type="button" @click="getData">GET</button> <!-- @click = onclick -->
    <button type="button" @click="setData">SET</button> <!-- @click = onclick -->
    <hr>
    <select class="form-control" v-model="region" @change="changeRegion">
      <!-- element attribute 값은 콜론(:)으로 -->
      <option v-for="(data, index) in arr" :key="index" :value="data.id">{{ data.name }}</option>
    </select>
    <hr>
    <!-- v-if 조건에 맞으면 랜더링 함. 안 맞으면 아예 안함 -->
    <!-- v-show 랜더링 무조건 일단 함. -->
    <table class="table table-border" v-if="tableShow">
      <tr v-for="(data, index) in arr" :key="index">
        <td>{{ data.id }}</td>
        <td>{{ data.name }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'gang',
      subTitle: 'pro',
      inputVal: '123',
      arr: [
        { id: 'S', name: 'Seoul'},
        { id: 'B', name: 'Busan'},
        { id: 'J', name: 'Jeju'}
      ],
      region: 'J', // <select class="form-control" v-model="region"> 바인딩 됨
      tableShow: false
    }
  },
  watch: {
    input1 () {
      console.log('[watch] START')
      console.log(this.inputVal)
      console.log('[watch] END')
    }
  },
  methods: {
    getData () {
      alert(this.inputVal)
    },
    setData () {
      this.inputVal  = 'abc'
    },
    changeRegion () {
      alert(this.region)
    }
  },
  beforeCreate () {
    console.log('1 beforeCreate')
  },
  created () {
    console.log('2 created')
  },
  beforeMount () {
    console.log('3 beforeMount')
  },
  mounted () {
    console.log('4 mounted')
  },
  beforeUpdate () {
    console.log('5 beforeUpdate')
  },
  updated () {
    console.log('6 updated')
  },
  beforeDestroy () {
    console.log('7 beforeDestroy')
  },
  destroyed () {
    console.log('8 destroyed')
  }
}
</script>
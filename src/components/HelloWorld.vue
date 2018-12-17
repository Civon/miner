<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <!-- <div @click="">start</div> -->

    <table id="roomList" >
      <thead>
        <tr>
          <th>ID</th>
          <th>bets</th>
          <th>comments</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for:="value in rooms">
          <td>{{ value.id }}</td>
          <td>{{ value.bets }}</td>
          <td>{{ value.comments }}</td>
          <td><button @click="joinRoom(value.id)">join</button></td>
        </tr>
      </tbody>
    </table>

    
    or <button>Create a Room</button>
  </div>  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    // bet: Number
    // rooms: Array,
    // bets: Array
  },
  data: () => {
    return{
      rooms: [],
      value: {
        id:'1',
        bets: '2',
        comments: 'sdsdsd'
      },
      // isVisiable: false,
    }
  },
  methods: {
    // TODO: load room information when page loading
    joinRoom: id => {
      // turn to the playing page where user wanna join 
    }
    // showRoom: bet => {
    //   // TODO: update data: room with same bet
    //   isVisiable = true;
    // }
  },
  // computed: {
    
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#roomList {
    margin: auto;
    border: 3px solid purple;
}

</style>

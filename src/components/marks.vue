<template>
  <div>
    <ul>
      <li v-for="(sub,index) in markscard" :key="index" @click="sub.show = !sub.show">
      <h3>{{ sub.subject }} </h3>
      <h4 v-show="sub.show">{{ sub.marks }} </h4>
      <h4 v-show="sub.show">{{ sub.practical }} </h4>
      <h4 v-show="sub.show">{{ sub.total }}  </h4>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      markscard: [
        {
          subject: "physics",
          marks: "marks: 65/70",
          practical: "practical: 30/30",
          total: "total: 95",
          show: false,
        },
        {
          subject: "chemistry",
          marks: "marks: 64/70",
          practical: "practical: 30/30",
          total: "total: 94",
          show: false,
        },
        {
          subject: "maths",
          marks: "marks: 89/100",
          practical: "practical: -",
          total: "total: 89",
          show: false,
        },
        {
          subject: "english",
          marks: "marks: 92/100",
          practical: "practical: -",
          total: "total: 92",
          show: false,
        },
        {
          subject: "economics",
          marks: "marks: 71/80",
          practical: "practical: 20/20",
          total: "total: 91",
          show: false,
        },
      ],
    };
  },
};
</script>

<style scoped>
div{
 border: 2px solid rgb(53, 49, 49);
  margin: 0.5em 0.5em 0.5em 0.5em;
  padding: auto;
}
ul{
  display: flex;
  flex-wrap: wrap;
 padding:0;
  list-style-type: none;
   background-color:rgba(161, 167, 161, 0.719);
}
li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 2px solid rgba(25, 26, 25, 0.753);
    margin: 10px;
     background-color:rgba(215, 240, 224, 0.856);
}
h3{
    font: bold 30px "Times New Roman";
   
}
</style>

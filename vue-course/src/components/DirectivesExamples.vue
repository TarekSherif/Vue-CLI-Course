<template>
 <div>
   <h1>BindingExamples</h1>
   <br>
   <p>
     {{emp.name}}
     <br/>
     {{emp.sal}}
   </p>
  <table>
    <tr>
      <td>
        <table>
          <tr>
            <td colspan="2">
              
            </td>
          </tr>
          <tr>
            <th>Name:</th>
            <td>
              <input type="text" :value="emp.name">
            </td>
          </tr>
          <tr>
            <th>Salary:</th>
            <td>
              <input type="text" :value="emp.sal">
            </td>
          </tr>
          <tr>
            <td colspan="2">
              <input type="submit" value="Add Data" @click="addData()" >
            </td>
          </tr>
        </table>
      </td>
       <td>
        <table>
          <tr>
            <td colspan="2">
              
            </td>
          </tr>
          <tr>
            <th>Name:</th>
            <td>
              <input type="text" v-model="emp.name">
            </td>
          </tr>
          <tr>
            <th>Salary:</th>
            <td>
              <input type="text" v-model="emp.sal">
            </td>
          </tr>
          <tr>
            <td colspan="2">
              <input type="submit" value="Add Data" @click="addData()" >
            </td>
          </tr>
        </table>
      </td>
    </tr>
  </table>
 </div>
</template>

<script>
export default {
  name: 'BindingExamples',
 data:()=>{
   return {
    emp:{
      name:"Tarek Sherif",
      sal:5000
    }
   }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
table{
  margin: 0 auto
}
</style>

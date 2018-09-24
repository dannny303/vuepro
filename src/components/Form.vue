<template>
   <div class="container">
      <div class="panel panel-primary">
         <div class="panel-heading">
            <h3 class="panel-title">Add User and Report</h3>
         </div>
         <div class="panel-body">
            <form>
                <div class="form-group">
                  <label for="name">Name:</label>
                  <input type="text" class="form-control" placeholder="Name" v-model="name">
                </div>
                <div class="form-group">
                  <label for="email">Email:</label>
                  <input type="text" class="form-control" placeholder="Email" v-model="email">
                </div>
                <div class="from-group">
                   <lable for="date">Date:</lable>
                   <input type="date" class="form-control" v-model="date">
                </div>
                <div class="form-group">
                    <lable for="location">Location:</lable>
                    <input type="text" Class="form-control" placeholder="Location" v-model="location">
                </div>
                <div class="form-group">
                    <lable for="companions">Companions:</lable>
                    <input type="text" Class="form-control" placeholder="Companions" v-model="companions">
                </div>
                <div class="from-group">
                    <label for="wcam">Weather Conditions AM:
                        <input type="radio" id="sunny" value="Sunny" v-model="wcam">
                        <lable for="sunny">Sunny</lable>
                        <input type="radio" id="ptcloudy" value="Partly Cloudy" v-model="wcam">
                        <lable for="ptcloudy">Partly Cloudy</lable>
                        <input type="radio" id="stormy" value="Stormy" v-model="wcam">
                        <lable for="Stormy">Stormy</lable>
                    </label>
                </div>
                <div class="from-group">
                    <label for="wcpm">Weather Conditions PM:
                        <input type="radio" id="sunny" value="Sunny" v-model="wcpm">
                        <lable for="sunny">Sunny</lable>
                        <input type="radio" id="ptcloudy" value="Partly Cloudy" v-model="wcpm">
                        <lable for="ptcloudy">Partly Cloudy</lable>
                        <input type="radio" id="stormy" value="Stormy" v-model="wcpm">
                        <lable for="Stormy">Stormy</lable>
                    </label>
                </div>
                <br>
               <button type="submit" class="btn btn-primary">Submit</button>
            </form>
         </div>
      </div>
      <br>
      <div class="panel panel-success">
         <div class="panel-body">
            My Name is : {{ name }}
            My Email is : {{ email }}
            The date is : {{ date }}
            I went Fishing @ : {{ location }}
            Fished with : {{ companions }}
            Weather Conditions AM : {{ wcam }}
            Weather Conditions PM : {{ wcpm }}
         </div>
      </div>
   </div>
</template>

<script>
   export default {
  
   data () {
      return {
           name: '',
           email: '',
           date: ''
      }
   }
}
</script>
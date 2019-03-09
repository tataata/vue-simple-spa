<template>
  <div id="app">
    <h1>{{ msg }}</h1>

    <ul class="nav nav-tabs" id="salaryPocker" role="tablist">
      <li class="nav-item">
        <a class="nav-link disabled" id="employee-tab" data-toggle="tab" href="#employee" role="tab" aria-controls="employee" aria-selected="true">Employee</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" id="employer-tab" data-toggle="tab" href="#employer" role="tab" aria-controls="employer" aria-selected="false">Employer</a>
      </li>
    </ul>
    <div class="tab-content" id="salaryPockerContent">
      <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="employee-tab">
        <form id="minExpectation">
          <label for="minExpectationValue">Tell us what is your minimum expected salary?</label>
          <input type="number" name="minExpectationValue" id="minExpectationValue">
          <button>Submit</button>
        </form>
      </div>
      <div class="tab-pane fade" id="employer" role="tabpanel" aria-labelledby="employer-tab">
          <form id="maxBuget">
            <label for="maxBugetValue">What is your maximum budget for this position?</label>
            <input type="number" for="maxBugetValue" id="maxBugetValue">
            <button>Submit</button>
          </form>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Hey, you both!'
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>

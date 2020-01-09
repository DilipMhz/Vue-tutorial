<template>
  <div id="app">
    <TrendingFetcher :options="['JAN', 'FEB','MAR','APR','JUN','JUL','AUG','SEP','NOV','DEC']"/>
    <TrendingFetcher :options="['2010', '2011','2012','2013','2014','2015','2016','2017','2018','2019']"/>
    <checkBox />
    <ra />
    <Input type="text" />Enter usename
    <Input type="password" /> enter password
    <br>
    <buttons text="Submit" />

  </div>
</template>
<script>
import TrendingFetcher from './components/trending-fetcher';
import checkBox from './components/checkBox'
import ra from './components/ra';
import Input from './components/Input';
import buttons from './components/buttons';
export default {
  name: 'app',
  components: {
    TrendingFetcher,
    checkBox,
    ra,
    Input,
    buttons
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

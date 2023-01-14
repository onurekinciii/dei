<tamplate>
  <h1>awdawdwa</h1>
  <apexchart class="graph" type="line" height="350" width="550" :options="chartOptions" :series="series"></apexchart>
</tamplate>
<script>
export default {
  data(){
    return {
      series:[{
        name : "Sales",
        data : [4,3,10,9,29,19,22,9,12,7,19,5,13,9,17,2,7,5]
      }],
      chartOptions:{
        chart : {
          height:350,
          type:'line'
        },
        forecastDataPoint : {
          count:7
        },
        stroke:{
          width:5,
          curve:'smooth'
        },
        xaxis : {
          categories : [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18]
        },
        title:{
          text:'',
          align:"left",
          style : {
            fontSize:"16px",
            color:"#666"
          }
        },
        fill : {
          type : "gradient",
          gradient : {
            shade : "dark",
            gradientToColors : ['#FDD835'],
            shadeIntensity : 1,
            type : 'horizontal',
            opacityFrom : 1,
            opacityTo : 1,
            stops : [0,100,100,100]
          }
        },
        yaxis : {
          min: -10,
          max: 40
        }
      }
    }
  }
}
</script>
<style></style>

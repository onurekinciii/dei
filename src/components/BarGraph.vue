<tamplate>
  <div id="charts">
<apexchart class="graph" type="bar" height="350" width="550" :options="chartOptions" :series="series"></apexchart>
</div>
</tamplate>
<script>
export default{
  data(){
    return {
      series: [{
        data : [400,430,448,470,540,580,690,1100,1200,1380]
      }],
      chartOptions:{
        chart: {
          type : "bar",
          height : 350
        },
        plotOptions : {
          bar : {
            borderRadius:4,
            horizontal:true
          }
        },
        dataLabels : {
          enabled: false
        },
        xaxis : {
          categories : ["South Korea","Canada","United Kingdom","Netherlands","Italy","Franch","Japon","United States","China","Germany"]
        }
      }
    }
  }
}
</script>
<style></style>

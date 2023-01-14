<tamplate>
<div id="charts">
  <apexchart class="area" type="bar" height="350" width="550" :options="chartOptions" :series="series"></apexchart>
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
          type : "area",
          height : 350
        },
        stroke : {
          curve : "straight"
        },

        dataLabels : {
          enabled: false
        },
        xaxis : {
          categories : ["South Korea","Canada","United Kingdom","Netherlands","Italy","Franch","Japon","United States","China","Germany"]
        },
        yaxis : {
          opposite:true
        },
        legend:{
          horizontalAlign:'left'
        }
      }
    }
  }
}
</script>
<style></style>

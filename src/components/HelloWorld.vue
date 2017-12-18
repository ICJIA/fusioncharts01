<template>
  <div class="hello">
    <h2>Fusioncharts demo</h2>
    <fusioncharts
    type="column2d"
    width="350"
    height="350"
    dataFormat="json"
    :dataSource="fc"
    ></fusioncharts>
    <hr/>
    <h4>Chart data:</h4>{{fc}}
  </div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        data() {
            return {
                fc: {
                    "chart": {
                        "caption": "Harry's SuperMart",
                        "subCaption": "Top 5 stores in last month by revenue",
                        "numberPrefix": "$",
                        "theme": "ocean"
                    },
                    "data": [{
                        "label": "Bakersfield Central",
                        "value": "880000"
                    }, {
                        "label": "Garden Groove harbour",
                        "value": "730000"
                    }, {
                        "label": "Los Angeles Topanga",
                        "value": "590000"
                    }, {
                        "label": "Compton-Rancho Dom",
                        "value": "520000"
                    }, {
                        "label": "Daly City Serramonte",
                        "value": "330000"
                    }]
                }
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h1,
    h2 {
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
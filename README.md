## Classes

<dl>
<dt><a href="#graph">graph</a></dt>
<dd></dd>
</dl>

## Members

<dl>
<dt><a href="#map">map</a></dt>
<dd><p><code>Json object format required for the chart functions
  1) Bubble Chart</p>
<p>this is the bubblechart function plots a static bubble chart with a constant radius bubble chart</p>
<p>Format :
[
    {
        &quot;Market&quot;: &quot;Used Goods Marketplace&quot;,
        &quot;Amount&quot;: &quot;423225136&quot;,
        &quot;Last_Transaction_Date&quot;: &quot;2016-07-23&quot;,
        &quot;Investment_Count&quot;: &quot;14&quot;
    },
    .
    .
    .
    .
]</p>
<p>2) Bubble Chart Zoom</p>
<p>this function plots a static bubble chart with a constant radius and zoomable parameter</p>
<p>Format : 
[
    {
        &quot;Market&quot;: &quot;Used Goods Marketplace&quot;,
        &quot;Amount&quot;: &quot;423225136&quot;,
        &quot;Last_Transaction_Date&quot;: &quot;2016-07-23&quot;,
        &quot;Investment_Count&quot;: &quot;14&quot;
    },
    .
    .
    .
    .
]</p>
<p>3) Time line chart</p>
<p>this function plots a static bubble chart with a constant radius and zoomable parameters,</p>
<p>Format : 
 {  &quot;Skill development&quot;:{<br>      &quot;amount&quot;:2095630,
      &quot;data&quot;:[<br>         {<br>            &quot;brand_logo&quot;:null,
            &quot;brand&quot;:&quot;TapChief&quot;,
            &quot;entity&quot;:&quot;Pilani Experts Technology Labs Private Limited&quot;,
            &quot;amount&quot;:997815,
            &quot;photo&quot;:&quot;&quot;,
            &quot;date&quot;:&quot;2016-10-01&quot;,
            &quot;investor_name&quot;:&quot;Radhakrishna Nalabothu&quot;
         },
         .
         .
         .
      ],
    &quot;name&quot;:&quot;Skill development&quot;
   },
      .
      .
      .
      .
 }</p>
<p>4)heatMap</p>
<p>this function plots a heat map using the above given parameters,</p>
<p>Format : 
{ &quot;Market&quot; : &quot;Sector&quot;,
  &quot;children&quot; : [
  {
    &quot;Market&quot;: &quot;Used Goods Marketplace&quot;,
    &quot;Amount&quot;: 423225136,
    &quot;Last_Transaction_Date&quot;: &quot;2016-07-23&quot;,
    &quot;Investment_Count&quot;: 14
  },
  .
  .
  .
  .]
}</p>
<p>5)networkGraph</p>
<p>this function plots a network of nodes of startups and their investors</p>
<p>Format : 
[
  {
    &quot;name&quot;: &quot;Eko India Financial Services Private Limited&quot;,
    &quot;investors&quot;: [
      {
        &quot;investments&quot;: 2,
        &quot;id&quot;: 5526,
        &quot;name&quot;: &quot;Share India Commodity Brokers&quot;
      },
      .
      .
      .
      .
    ],
    &quot;id&quot;: 4
  },
  .
  .
  .
  .
]
</code></p>
</dd>
</dl>

<a name="graph"></a>

## graph
**Kind**: global class  

* [graph](#graph)
    * [.set_margin(top, bottom, left, text)](#graph.set_margin)
    * [.set_canvas(width, height)](#graph.set_canvas)
    * [.bubbleChart(data, xAxis, yAxis, r, text)](#graph.bubbleChart)
    * [.bubbleChartZoom(data, xAxis, yAxis, r, text)](#graph.bubbleChartZoom)
    * [.timeChart(data, xAxis, yAxis, r, text)](#graph.timeChart)
    * [.heatMap(data, area, color, name)](#graph.heatMap)
    * [.networkGraph(data, startup_name_key, startup_investor_key, startup_id_key, investor_name_key, investor_investments_key, investor_id_key)](#graph.networkGraph)

<a name="graph.set_margin"></a>

### graph.set_margin(top, bottom, left, text)
this function sets the margin for the graph in the canvas.

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| top | <code>int</code> | : corresponds to the top margin |
| bottom | <code>int</code> | : corresponds to the bottom margin |
| left | <code>int</code> | : corresponds to the left margin |
| text | <code>int</code> | : corresponds to the right margin |

<a name="graph.set_canvas"></a>

### graph.set_canvas(width, height)
this function sets the width and heigth of the canvas.

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| width | <code>int</code> | : corresponds to the width of the canvas |
| height | <code>int</code> | : corresponds to the height of the canvas |

<a name="graph.bubbleChart"></a>

### graph.bubbleChart(data, xAxis, yAxis, r, text)
this is the bubblechart function plots a static bubble chart with a constant radius bubble chart

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>json</code> | : json data obtained from the ajax code in example function |
| xAxis | <code>string</code> | : the json key which corresponds to the value plotted in the xAxis |
| yAxis | <code>string</code> | : the json key which corresponds to the value plotted in the yAxis |
| r | <code>string</code> | :  the json key which corresponds to the radius of the bubbles plotted |
| text | <code>string</code> | :  the json key which corresponds to the text inside the bubbles plotted |

<a name="graph.bubbleChartZoom"></a>

### graph.bubbleChartZoom(data, xAxis, yAxis, r, text)
this function plots a static bubble chart with a constant radius and zoomable parameters,

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>json</code> | : json data obtained from the ajax code in example function |
| xAxis | <code>string</code> | : the json key which corresponds to the value plotted in the xAxis |
| yAxis | <code>string</code> | : the json key which corresponds to the value plotted in the yAxis |
| r | <code>string</code> | :  the json key which corresponds to the radius of the bubbles plotted |
| text | <code>string</code> | :  the json key which corresponds to the text inside the bubbles plotted |

<a name="graph.timeChart"></a>

### graph.timeChart(data, xAxis, yAxis, r, text)
this function plots a static bubble chart with a constant radius and zoomable parameters,

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>json</code> | : json data obtained from the ajax code in example function |
| xAxis | <code>string</code> | : the json key which corresponds to the value plotted in the xAxis |
| yAxis | <code>string</code> | : the json key which corresponds to the value plotted in the yAxis |
| r | <code>string</code> | :  the json key which corresponds to the radius of the bubbles plotted |
| text | <code>string</code> | :  the json key which corresponds to the text inside the bubbles plotted |

<a name="graph.heatMap"></a>

### graph.heatMap(data, area, color, name)
this function plots a heat map using the above given parameters,

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>json</code> | : the json object obtained after passing the json file to ajax code in the example |
| area | <code>string</code> | : the json key which corresponds to the area of the cell in the heatmap |
| color | <code>string</code> | : the json key which correspond to the color depth of the cell |
| name | <code>string</code> | : the json key which corresponds to the cell name(i.e. text inside the cell) |

<a name="graph.networkGraph"></a>

### graph.networkGraph(data, startup_name_key, startup_investor_key, startup_id_key, investor_name_key, investor_investments_key, investor_id_key)
this function plots a network of nodes of startups and their investors

**Kind**: static method of [<code>graph</code>](#graph)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>json</code> | : the json object obtained after passing the json file to ajax code in the example |
| startup_name_key | <code>string</code> | : the json key which corresponds to the name of the startup node |
| startup_investor_key | <code>string</code> | : the json key which corresponds to the investors of the startup node |
| startup_id_key | <code>string</code> | : the json key which corresponds to the unique id of the startup node |
| investor_name_key | <code>string</code> | : the json key which corresponds to the name of the investor node |
| investor_investments_key | <code>string</code> | : the json key which corresponds to the investments of the investor node |
| investor_id_key | <code>string</code> | : the json key which corresponds to the unique id of the investor node |

<a name="map"></a>

## map
<code>Json object format required for the chart functions
  1) Bubble Chart

this is the bubblechart function plots a static bubble chart with a constant radius bubble chart

Format :
[
	{
		"Market": "Used Goods Marketplace",
		"Amount": "423225136",
		"Last_Transaction_Date": "2016-07-23",
		"Investment_Count": "14"
	},
    .
    .
    .
    .
]

2) Bubble Chart Zoom

this function plots a static bubble chart with a constant radius and zoomable parameter

Format : 
[
	{
		"Market": "Used Goods Marketplace",
		"Amount": "423225136",
		"Last_Transaction_Date": "2016-07-23",
		"Investment_Count": "14"
	},
    .
    .
    .
    .
]

3) Time line chart

this function plots a static bubble chart with a constant radius and zoomable parameters,

Format : 
 {  "Skill development":{  
      "amount":2095630,
      "data":[  
         {  
            "brand_logo":null,
            "brand":"TapChief",
            "entity":"Pilani Experts Technology Labs Private Limited",
            "amount":997815,
            "photo":"",
            "date":"2016-10-01",
            "investor_name":"Radhakrishna Nalabothu"
         },
         .
         .
         .
      ],
    "name":"Skill development"
   },
      .
      .
      .
      .
 }

4)heatMap

this function plots a heat map using the above given parameters,

Format : 
{ "Market" : "Sector",
  "children" : [
  {
    "Market": "Used Goods Marketplace",
    "Amount": 423225136,
    "Last_Transaction_Date": "2016-07-23",
    "Investment_Count": 14
  },
  .
  .
  .
  .]
}


5)networkGraph

this function plots a network of nodes of startups and their investors

Format : 
[
  {
    "name": "Eko India Financial Services Private Limited",
    "investors": [
      {
        "investments": 2,
        "id": 5526,
        "name": "Share India Commodity Brokers"
      },
      .
      .
      .
      .
    ],
    "id": 4
  },
  .
  .
  .
  .
]
</code>

**Kind**: global variable  

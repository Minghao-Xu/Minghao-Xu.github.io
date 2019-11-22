# Energy Data in Smart Local Energy Systems
Decarbonisation and decentralisation are transforming the UK energy sector, driving it towards a Net Zero carbon future. With respect to the system structure, this is a fundamental shift from centralised command and control-based structures to more decentralised, interactive and collaborative structures. The management of the new energy system involves multiple actors at different layers and will heavily require collecting, exchanging and interoperating with the data.

Traditionally, energy data are mainly generated in the energy system, i.e., generation plant, transmission networks, distribution networks and all the associated energy assets. The data collection has been governed by central processes with limited numbers of channels and restricted access. Data has not been particularly granular, and retrieval and processing timescales have been long.

In contrast, as the energy system is shifting to a more decentralised structure, local energy systems will play an increasingly dominant role in the future system. Correspondingly, consumer data are generating at an unprecedented speed mainly from smart meters and smart appliances. The management of the new energy system and the new business models, such as aggregated demand response, and Peer-to-Peer (P2P) energy trading, will rely on timely access to relevant, up-to-date and comprehensive customer data sets from multiple sources.

While the UK have been digitalising the energy system and an influx of energy data have been generated, the energy landscape has not been fully digitalised yet to date. The modernization and digitalisation are being hindered by often poor quality, inaccurate, or missing data, and lack of proper management and analysis of the data. The Energy Data Taskforce [^1] identified that a staged approach needed to be taken to achieve a Modern, Digitalised Energy System in order to fill the data gaps and maximises data value.
1. Data Visibility
2. Infrastructure and Asset Visibility
3. Operational Optimisation
4. Open Markets
5. Agile Regulation

Visibility is a key component and enabler to achieve a modern and digitalised energy system. Since 2010, researchers at the Centre for Sustainable Power Distribution (CSPD) in Bath have undertaken fundamental research to develop algorithms and tools to enable visibility, predictability of local energy resources over differing scales and lead times. In addition to the prohibitive expense for widespread monitoring device at local energy systems, the main technical challenges in managing the generated data, and subsequently analysing them, are three-fold:
1. Consumer data are large in volume;
2. Consumer data are generating at a high speed;
3. Consumer data are extremely volatile and uncertain.

The figures below are a demonstration of how volatile and uncertain consumer energy data are compared to more aggregated data.


<div class="row">
  <div class="column">
    <img src="/assets/images/Energy_Data/Aggregation.png" alt="Agrregation" style="width:100%">
    <p>Figure 1: Load Aggregation</p>
  </div>
  <div class="column">
    <img src="/assets/images/Energy_Data/Season.png" alt="Season" style="width:100%">
    <p>Figure 2: Load in Winver VS Summer</p>
  </div>
  <div class="column">
    <img src="/assets/images/Energy_Data/One Customer.png" alt="One Customer" style="width:100%">
    <p>Figure 3: One Consumer</p>
  </div>
</div>

Three categories of research work in CSPD have been conducted to increase consumer and network visibility.
1. Consumer Characterization and Segmentation

  We have proposed a novel multi-resolution clustering (MRC) method that for the first time classifies end customers directly from massive, volatile and uncertain smart metering data [^2]. The results show significant improvements over traditional time-series analysis, providing more accurate load profiling at a more granular level.

  We have also developed a consumer segmentation framework using consumers’ social-economic/ sociodemographic information [^3]. Energy behavior patterns could be directly inferred from consumers’ sociodemographic status.

  <style>
  img {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .caption {
      width: 5;
      text-align: left;
  }

  </style>

  <div>
  <img src="./assets/images/Energy_Data/Social-Eco Gene.png" alt="Social-Eco Gene" class="center" style="width:100%"/>
  <div class="caption">Figure 4: Social-Eco Gene Map</div>
  </div>


2. Load Forecasting

  We have developed a bespoke deep learning application for household load forecasting which can learn the uncertainties of domestic load profiles directly, and avoid overfitting encountered by most deep learning models [^4]. Specifically, the method enables learning of spatial information shared between interconnected customers and hence allowing more learning layers before the occurrence of overfitting.

  <style>
  img {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .caption {
      width: 5;
      text-align: left;
  }

  </style>

  <div>
  <img src="/assets/images/Energy_Data/Forecasting.png" alt="Forecasting" class="center" style="width:100%"/>
  <div class="caption">Figure 5: Forecasting Comparison Between Different Methods</div>
  </div>


3. Low Voltage Network Template

  We have developed and tested a cost-effective statistical method which significantly improves the visibility of LV networks without extensive monitoring cost [^5]. Specifically, a novel hybrid clustering technique was first developed to extract the underlying patterns of the substation data which are reified in the form of typical templates. The extracted patterns were then leveraged to train various regression models which can accurately infer the conditions of un-monitored LV substations entirely based on routinely available fixed data.
  <style>
  * {
    box-sizing: border-box;
  }

  .column {
    float: left;
    width: 50%;
    padding: 5px;
  }

  /* Clearfix (clear floats) */
  .row::after {
    content: "";
    clear: both;
    display: table;
  }
  </style>

  <div class="row">
    <div class="column">
      <img src="/assets/images/Energy_Data/LV Templates.png" alt="LV Templates" style="width:100%">
      <p>Figure 6: LV Templates</p>
    </div>
    <div class="column">
      <img src="/assets/images/Energy_Data/Power Within a Day.png" alt="Power Within a Day" style="width:100%">
      <p>Figure 7: Power Within a Day</p>
    </div>
  </div>



Big data and Artificial Intelligence are likely to play an important role in the early stages of local energy systems to estimate load profiles of energy customers and energy networks when there are significant data gaps. Critically, when smart meter and substation data is widely available, they will support advanced understanding of energy resources at different levels to inform high-precision energy management and trading.

[^1]: https://es.catapult.org.uk/news/energy-data-taskforce-report/
[^2]: Li, R., Li, F., & Smith, N. D. (2016). Multi-resolution load profile clustering for smart metering data. IEEE Transactions on Power Systems, 31(6), 4473-4482.
[^3]: Tong, X., Li, R., Li, F., & Kang, C. (2016). Cross-domain feature selection and coding for household energy behavior. Energy, 107, 9-16.
[^4]: Shi, H., Xu, M., & Li, R. (2017). Deep learning for household load forecasting—A novel pooling deep RNN. IEEE Transactions on Smart Grid, 9(5), 5271-5280.
[^5]: Li, R., Gu, C., Li, F., Shaddick, G., & Dale, M. (2014). Development of low voltage network templates—Part I: Substation clustering and classification. IEEE Transactions on Power Systems, 30(6), 3036-3044.
[^6]: Li, R., Gu, C., Li, F., Shaddick, G., & Dale, M. (2014). Development of low voltage network templates—Part II: Peak load estimation by clusterwise regression. IEEE Transactions on Power Systems, 30(6), 3045-3052.

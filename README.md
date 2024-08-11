<h1>Forest Fire Hazard</h1>

 ### Summary of my independet study

<h2>Description</h2>
<p>Forest fires occur every year in Spain, causing extensive economic and
biodiversity damage. Thanks to advancements in technology, there is a multitude of
tools in geographic information systems to analyze specific factors connected to the
ignition and spread of forest fires. In this way, the government can take action to
prevent them.
The following project analyzes different variables related to hazard and vulnerability to
determine the risk of forest fires in the municipality of Hinojosa del Duque.
Understanding the characteristics of the forest mass and how human activities are
involved helps determine the risk this municipality could face. Therefore, using GIS and
various statistical processes, it is possible to identify the most problematic areas and
allocate resources to prevent the highest possible damage
</p>


<h2>Languages and software Used</h2>

- <p>ARCGIS</p> 
+ <p>QGIS</p>
* <p>Python</p>
- <p>Excel</p>

<h2>Methodology</h2>
<p>The goal of this methodology  is to create cartography related to the risk of forest fire in Hinojosa del Duque, Cordoba, Spain. To do so, I have created a model on ArcGIS Desktop using different variables based on <a href="https://www.juntadeandalucia.es/medioambiente/portal/landing-page-publicacion/-/asset_publisher/FytOUWH22K7t/content/plan-infoca.-un-plan-de-acci-c3-b3n-al-servicio-del-monte-mediterr-c3-a1neo-andaluz-2003-/20151">INFOCA PLAN</a></p>

<h3>Hazard of forest fires.</h3>

<p>INFOCA Plan describes the risk of forest fires using two different variables. The first one is related to long-term danger and the second one to short-term danger. In this case, I focused on the long-term variables, which talk about the combustibility of the vegetation and the slope, which promote convective currents. For the vulnerability, I created two variables based on two different points of view. The first one consists of the human value over monetary values of objects, such as houses, farms, historical sites, protected areas, etc. In the end, I used the data on the hazard and vulnerability to determine the risk of forest fires in Hinojosa del Duque.</p>  

<p>Area of study:</p>
<img src="https://i.imgur.com/JL7ndw0.jpeg"height="70%" width="70%>
    
<b>Calculating hazard.</b>

<p>To calculate the danger of forrest fire, INFOCA PLAN describe a metodology called structural hazard which describe the hazard in the long term. This structural hazard is based on the combination of two different variables</p>

<img src="https://i.imgur.com/FD4Ogvj.png" height="50%" width="50%" alt="INFOCA PLAN METODOLOGY"/>
<b>Enter the variables into ArcGIS: </b>

<b><img src="https://i.imgur.com/aQojJyF.png" height="60%" width="60%" alt="Metodology on ArcGIS"/></b>

<p> The process can be summarized in two stages. In the first stage, I reclassified the digital terrain model into 5 categories and reclassified the land use layer of Andalusia according to the fuel model. Then, I combined the results of both to determine the combustibility index.</p>
<b>Results:  <br/>
<img src="https://i.imgur.com/CyhC1lS.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b></b>Calculating the vulerability.</b>
 <p> To develop the vulnerability, I reclassified different significant elements of human activities listed in the table below. Subsequently, I calculated the distance that these activities have with respect to the main communication routes, which is where the fire extinguishing devices would come from. This distance was normalized on a scale of 1 to 5 to be comparable with the previously made reclassification. Finally, both were multiplied and normalized once more from 1 to 5 to obtain the vulnerability of the study area</p>

<img src="https://i.imgur.com/8GPp9su.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<b>Naismith formula:</b>

<img src="https://i.imgur.com/OEzwWe5.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>

<b>Enter the variables intor ArcGIS:</b>

<img src="https://i.imgur.com/piictM2.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>

<b>Results:</b>

<img src="https://i.imgur.com/90c8nEH.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>

<b>Calculating forestfire risk.</b>

<p>To generate the forest fires risk map, you simply need to multiply the vulnerability layer with the natural hazard layer. To do this, both layers are first normalized to a scale of 1 to 3, and then after the multiplication, they are normalized again to the same scale to obtain the final result.</p>

<b>Results.</b>
 
<img src="https://i.imgur.com/ilzfuHj.png"  height="60%" width="60%"/>


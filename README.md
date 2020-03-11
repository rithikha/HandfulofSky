# HandfulofSky

![Image description](link-to-image)
Caption: 

**Project Link:** https://rithikha.github.io/HandfulofSky/index.html

**Reflective Analysis ** 
My little sister, like most children, is absolutely awestruck by the sky at night. Our house is at the boundary of the city and the absence of bright city lights makes for some excellent star-gazing. The goal of this map is not to answer any questions but rather to create a place for quiet and consequently, a space for meaningful questions to emerge.
While in my last lab and previous assignments I focused on and specifically emphasized data visualization within the map, my aim for this project was more to create an emotional experience through a digital environment. The map is just one of many elements used to transport (and in some ways force) the ever-busy modern user (anyone and everyone) into another headspace. So while this project used Mapbox GL JS to create and introduce pop-up interactivity and map camera animation, it also heavily relied on HTML and CSS to style the page in a particular way. These other elements include appealing to the other senses through music, formatted quotes and text, to provide greater context to the map and further provoke a meditative headspace, as well as the map itself. A border-radius was used  to create a curved border on the map. This, along with the map rotation served to take the user one step closer to feeling like they are peering down at the earth and the stars. 

The colour choices were kept to a cool palette of black and various blue and yellow tones. I considered getting rid of the contrast by using a black webpage background however the result looked a little tacky. Instead, after feedback (from Vicky Jiang) I changed the background to a light cream colour to address the glare that the previous white-background had. While there was also star data information that could be integrated into a popup, I decided to simplify rather than complicate, keeping them as background visuals (circles whose fade value was classified by their Brightness Value attribute). The map rotation speed is set at a value that I thought provided enough visual simulation while also making clicking the constellation lines less annoying and maintaining a feeling of calm.

Future Considerations - I wanted to add another layer containing only the stars that make up each of the constellations. This way I could increase their brightness so they would stand out more and add some more relevant information about the constellation through a pop-up with the star name.

I couldn’t figure out how to make the music autoplay as soon as the webpage was loaded. The audio is set to repeat however.

To complement the Nightfall quote I also wanted to change the mapstyle from a night style to a day style every rotation. I couldn’t get this to work but here’s the code I previously tried within **map.on('load', function () { **:

    function switchMap() {
      currentStyle = String(map.getStyle());
      if (currentStyle == "mapbox://styles/rithikha/ck7bdfx9g00yy1ip69s6szri4") {
        map.setStyle("mapbox://styles/rithikha/ck7lfr6ym0bas1it4gepfzwwt");
      }
      else {
        map.setStyle("mapbox://styles/rithikha/ck7bdfx9g00yy1ip69s6szri4");
      }
    }
    
    setInterval(switchMap, 12000);


**Collaborations**
Contributed to a couple critiques and mostly suggested minor design considerations for Vicky, Jassen and Lucas. Got some help from Vicky for making pop-ups in Mapbox, but I ended up following along this tutorial instead: https://docs.mapbox.com/mapbox-gl-js/example/polygon-popup-on-click/
Feedback from Vicky and Jassen included adjusting the margins for the map (changes made) and using a different background colour so it’s not so glaringly white.
The project was inspired by a much cooler map, the Star Atlas (https://staratlas.com/). I also used this tutorial to animate the map: https://www.youtube.com/watch?v=a8aplYWsj70
 

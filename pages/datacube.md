## Space-Time Data Cube

---

<style>

#scaled-frame {
  width: 500px;
  height: 500px;
  border: 1px;
    display: block;
    margin-right: auto;
    margin-left: auto;

}

table.center {
    margin-left:auto; 
    margin-right:auto;
  }

</style>


In this example I wanted to experiment with whether a space-time cube visualization would add any additional visual analytical qualities above a 2 dimensional (or 2.5 :smirk: ).

For this illustration I selected one of my morning runs where I usually like to analyse my running pace (or rather lack of it). I always run with a GPS sports watch, my current being the [Garmin Vivosport](https://support.garmin.com/en-US/?identifier=563441244&tab=topics) which is connected to my Garmin Connect account (more on this later).

From Garmin Connect it's straightforward enough to download data for a specific run in a GPX file so this was my space-time source in the form of latitude, longitude and timestamp.

I also wanted to give any visualization some geographical context so I also acquired an Ordnance Survey basemap for the region covered by my route.

Then turning to Jupyter Lab, matlab and plotly I set about building the following interactive visualization  

<table class="center">
    <iframe id="scaled-frame" src="../html/adamgoesforarun.html"></iframe>
    <p align="center">3d Datacube showing space-time</p>
</table>

In this visualisation time is represented on the z axis which is normalised to the start of the run at 0 seconds. When this is overlaid with the spatial dimensions x and y represented as lat and long, any change in pace is visualised by the changing of the gradient of the red line which is the path of the run.

Rotating the interactive data cube to a plan view where the z axis is perpendicular to the x,y axes emphasizes any change in gradient.

<a href="../jupyter/datacube.html"> View Source in Html </a>

#### Conclusions

Although an interesting exercise and a pretty visualisation I honestly don't think the extra dimension add anything to the analysis. Compare the 3d to the 2d using a colour to present pace (this is a standard widget on the Garmin Connect App). Personally I much pefer the 2d view   

<table class="center">
    <a href="/pages/datacube.md"><img src="../images/datacube/2drunning.png"  /></a>
    <p align="center">Standard Pace Chart </p>
</table>

All opinions expressed are my own and based on my experiences with my own equipment.
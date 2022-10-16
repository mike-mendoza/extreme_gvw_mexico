# EECAN NPBN GUI
## A Non-parametric Bayesian Network (NPBN) for modelling axle loads

This work is based on the publications _A Non-parametric Bayesian Network for multivariate probabilistic modelling of Weigh-in-Motion System Data_ https://doi.org/10.1016/j.trip.2022.100552


$\mathrm{EECAN}_{\mathrm{NPBN}}$ was used in the research _Mapping extreme gross vehicle weights using a Non-parametric Bayesian Network_ 

---

The Graphical User Interface **EECAN NPBN** can be downloaded from  <span style="font-size:larger;">**[here](https://1drv.ms/u/s!Ao_8atl7piKAmZ82GcBUYvXnU3s3kA?e=iFxzTe)**</span>. It computes synthetic axle loads of five truck types similar to those reported in the Statistic Field Study of Domestic Road Transportation (EECAN, for its acronym in Spanish) origin-destination survey database. 

The surveys have been conducted for four consecutive days per year by the Mexican Ministry of Communications and Transports, in a varying number of stations surveyed every year from 1991 until 2017.

The Non-parametric Bayesian Network was computed using _PY_BANSHEE_ (paper in review prosses) the python version of BANSHEE MATLAB (https://doi.org/10.1016/j.softx.2020.100588).

The available vehicle types are: 

* `C2`: Single-unit vehicle with two axles
* `C3`: Single-unit vehicle with three axles 
* `T3S2`: Three-axle tractor plus two-axle semitrailer
* `T3S3`: Three-axle tractor plus three-axle semitrailer
* `T3S2R4`: Three-axle tractor plus two-axle semitrailer plus four-axle trailer

The codes of the Mexican vehicle types are given by the Ministry of Communications and Transport. 

In the main window of the GUI. The user can choose desired number samples and the desired units (kN, kg, ton, kip). The output is a database presented in a 11-column table with synthetic axle loads observations (different every time the model is run), of the vehicles with up to nine axles 

There are, three main check boxes: 1) vehicle type subset, 2) NPBN and rank correlation matrix plot.

1. If the `vehicle type subset` check box is selected, the user needs to select the desired vehicles types and provide their corresponding proportions (or the probability of observing each vehicle type). Otherwise, the 5 vehicle types will be used to generate synthetic observations. 
2. If the `NPBN and rank correlation matrix plot` check box is selected, he Non-Parametric Bayesian Network (NPBN) direct acyclic graph and the rank correlation matrix plot will be shown as a colour map. 

Once all the values are set by pressing the `compute` button the synthetic axle loads will be generated and the histogram of the gross vehicle weight distribution and a bar plot of the truck types will be shown. The computed data can be stored in a CSV file by pressing the `Save csv` button.  

More information can be found in the Quick User Guide file. 

## Installation
Download from <span style="font-size:larger;">**[here](https://1drv.ms/u/s!Ao_8atl7piKAmZ82GcBUYvXnU3s3kA?e=iFxzTe)**</span> and extract EECAN_NPBN.zip file. Double click on the file extracted file (in some cases it is needed to add an exception in your antivuris). 


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[GNU](https://choosealicense.com/licenses/gpl-3.0/)

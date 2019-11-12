# Resources
Consider this a public bookmark bar. These are resources I've found useful or think might be one day.

Disclaimers: still in progress, definitely not comprehensive, links may not work, and in no particular order.

I welcome any additions, suggestions, or corrections! Feel free to create a pull request or send me an [email](mailto:eltuck@umich.edu).

I've found a good portion of this from links other folks have shared on  [Twitter](https://twitter.com/emilyltucker). Thanks, y'all. Also a very big thank you to everyone who created the original content.

## Table of Contents
* [Python](#python)
* [R](#r)
* [GitHub](#github)
* [AMPL](#ampl)
* [Julia](#Julia)
* [Other languages](#other-programming-languages)
* [General coding](#general-coding--computation)
* [Math prog. software](#math-programming-software)
* [Math prog. resources](#math-programming-resources)
* [Operations research-adjacent material](#operations-research-adjacent-material)
* [Data viz](#data-visualization)
* [Datasets](#datasetsdatabases)
* [Communication](#communicationdissemination)
* [Healthcare](#healthcare)
* [Jobs and summer schools](#jobssummer-schools)
* [Funding](#funding)
* [Teaching](#teaching)
* [Blogs I like (and read occasionally)](#blogs-i-like-and-read-occasionally)
* [Various advice](#various-advice)
* [Eclectic](#eclectic)

### Python
* Overview
  * [Whirlwind tour](https://github.com/jakevdp/WhirlwindTourOfPython) from [@jakevdp](https://github.com/jakevdp)
  * [Overview](https://vknight.org/Introduction_to_OOP/OverviewOfPython/) from [@drvinceknight](https://github.com/drvinceknight)
  * [Scipy lecture notes](http://www.scipy-lectures.org/)
    * [Getting started](https://www.scipy-lectures.org/intro/index.html)
  * Targeted
    * [Python for Mathematicians](https://github.com/drvinceknight/Python-Mathematics-Handbook) (drvincekinght)
    * [Python for Epidemiologists](https://github.com/pzivich/Python-for-Epidemiologists) (pzivich)
* Free Textbooks
  * [_Think Python_](http://greenteapress.com/wp/think-python-2e/) by [@AllenDowney](https://github.com/AllenDowney), beginners guide, programming exp. not necessary
  * [_Python Data Science Handbook_](https://jakevdp.github.io/PythonDataScienceHandbook/) by [@jakevdp](https://github.com/jakevdp)
  * [_Intro to Machine Learning in Python_](https://github.com/amueller/introduction_to_ml_with_python) by [@amueller](https://github.com/amueller)
  * [_Bayesian Methods for Hackers_](https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers) (Pilon)
  * [_Modeling and Simulation in Python_](http://greenteapress.com/wp/modsimpy/) by [@AllenDowney](https://github.com/AllenDowney), targeted towards intro undergrads
* Community
  * [Slack channel](https://py4ds.slack.com) to learn data science in Python
* Overall tutorial
  * [Python Software Foundation](https://docs.python.org/3.6/tutorial/index.html)
* Topics/packages
  * Pandas (data processing)
    * [Beginner tutorial](http://gregreda.com/2013/10/26/intro-to-pandas-data-structures/) from [@gjreda](https://github.com/gjreda)
    * [Intermediate tutorial](http://tomaugspurger.github.io/modern-1-intro) from [@tomaugspurger](https://github.com/tomaugspurger)
  * Networks
    * Package: [NetworkX](https://github.com/networkx/networkx)
      * Tutorial: [network analysis](https://programminghistorian.org/lessons/exploring-and-analyzing-network-data-with-python) using humanities data
      * Tutorial: [Chinese postman problem](https://www.datacamp.com/community/tutorials/networkx-python-graph-tutorial)
      * [Network simplex](https://networkx.github.io/documentation/networkx-1.9.1/reference/generated/networkx.algorithms.flow.network_simplex.html)
    * Package: [SNAP](https://snap.stanford.edu/snappy/index.html)
      * Analysis of graphs and networks
      * Claims often faster and able to solve larger problems than NetworkX
  * Simulation
    * Discrete-event
      * Package: [SimPy](https://simpy.readthedocs.io/en/latest/)
        * [Google group](https://groups.google.com/forum/#!forum/python-simpy)
        * [Book chapter](http://users.iems.northwestern.edu/~nelsonb/IEMS435/PythonSim.pdf) by Barry Nelson
      * Package: [Ciw](http://ciw.readthedocs.io/en/latest/) (for open queueing networks)
    * Agent-based modeling
      * Package: [Mesa](https://github.com/projectmesa/mesa), general purpose
        * [Tutorial](https://github.com/projectmesa/mesa)
      * Package: [ABCE](https://abce.readthedocs.io/en/0.9.3b2/), economic modeling
  * [List](https://wiki.python.org/moin/PythonForOperationsResearch) of operations-research-related packages
  * Optimization
    * [Overview](https://coral.ie.lehigh.edu/~ted/files/modeling/lectures/ModelingWithPython.pdf) (Ted Ralphs)
    * Modeling languages
      * Package: [gurobipy](https://www.gurobi.com/documentation/8.0/quickstart_windows/py_python_interface)
        * [Walk-through](https://www.gurobi.com/documentation/8.0/quickstart_windows/py_simple_python_example.html) of building simple model
        * [Walk-through](https://www.gurobi.com/documentation/8.0/quickstart_windows/py_python_dictionary_examp.html) of semi-complex model
        * Example models
          * [List](https://www.gurobi.com/documentation/8.0/examples/python_examples.html)
          * [Guided tour](https://www.gurobi.com/documentation/8.0/examples/example_tour.html)
      * Package: [PuLP]( https://projects.coin-or.org/PuLP), linear programs
      * Package: [Pyomo](http://www.pyomo.org/), all-purpose
        * [How to](https://groups.google.com/forum/#!topic/pyomo-forum/NWU1LW6GWL8) run models
        * [Example models](http://nbviewer.jupyter.org/github/Pyomo/PyomoGallery/tree/master/)
      * Package: [Pysp](https://pypi.org/project/coopr.pysp/), extends Pyomo for stochastic programming
    * Solvers & algorithms
      * Package: [scipy.optimize](https://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html)
      * Package: [CVXPY](http://www.cvxpy.org/), convex opt
        * [Short-course](http://www.cvxpy.org/short_course/index.html)
      * Package: [Optimist](https://scholarsarchive.byu.edu/cgi/viewcontent.cgi?article=1330&context=iemssconference), SDDP in water systems
      * Package: [PyBnB](https://pypi.org/project/pybnb/), parallel branch-and-bound
      * Package: [StochOPy](https://github.com/keurfonluu/StochOPy), stochastic optimization
      * Package: [StOpt](https://gitlab.com/stochastic-control/StOpt), stochastic control (written in C++, Python bindings)
      * Package: [py-lapsolver](https://github.com/cheind/py-lapsolver), fast linear assignment problems
      * Package: [munkres](http://software.clapper.org/munkres/), Hungarian algorithm
      * Library: [PyMaxFlow](https://github.com/pmneila/PyMaxflow), Max flow/min cut
      * Package: [PyPSA](https://pypsa.org/), power systems analysis
      * Package: [PySCIPOpt](https://github.com/SCIP-Interfaces/PySCIPOpt)
        * [Book](https://scipbook.readthedocs.io/en/latest/index.html)
    * Plot [convex hull](https://docs.scipy.org/doc/scipy-0.19.0/reference/generated/scipy.spatial.ConvexHull.html)
    * Examples
      * [Optimization tutorial](https://github.com/ekhoda/optimization-tutorial) (ekhoda)
      * TSP
        * Implement TSP, [Video](https://www.coursera.org/lecture/delivery-problem/branch-and-bound-UyBJC)
        * A few algos [tutorial](https://nbviewer.jupyter.org/url/norvig.com/ipython/TSP.ipynb) (Norvig)
      * [Genetic algo](https://towardsdatascience.com/evolution-of-a-salesman-a-complete-genetic-algorithm-tutorial-for-python-6fe5d2b3ca35) (Stoltz)
      * [Facility location problems](https://scipbook.readthedocs.io/en/latest/flp.html) (SCIP)
  * Dimensionality reduction
    * Package: [umap](https://github.com/lmcinnes/umap), uniform manifold approx. and projection
  * Game theory [(source)](http://nashpy.readthedocs.io/en/stable/discussion/other-python-game-theory-libraries.html)
    * Software: [Gambit](http://www.gambit-project.org/)
    * Package: [Nashpy](http://nashpy.readthedocs.io/en/stable/), 2-player games/compute equilibria, [paper](http://joss.theoj.org/papers/10.21105/joss.00904)
    * Package: [Axelrod](http://axelrod.readthedocs.io/en/stable/), iterated prisoner's dilemma
    * Package: [PyNFG](https://pythonhosted.org/PyNFG/), network form games
    * Library: [lrslib](http://cgm.cs.mcgill.ca/~avis/C/lrs.html), _lrsnash_ can be used to compute Nash equilibria
    * Within [SageMath](http://doc.sagemath.org/html/en/reference/game_theory/index.html), games: cooperative with finite players; matching; normal form with N players
  * Math
    * SageMath textbook: [_Computational Mathematics with SageMath_](http://sagebook.gforge.inria.fr/english.html), Zimmermann et al.
  * Machine learning
      * [Flowchart](http://scikit-learn.org/stable/tutorial/machine_learning_map/), choosing the right estimator
      * Sklearn [tutorial](https://github.com/jakevdp/sklearn_tutorial) from [@jakevdp](https://github.com/jakevdp)
      * [Checklist](http://queirozf.com/entries/heads-up-for-deploying-scikit-learn-models-to-production-quick-checklist) before releasing (Almeida)
  * Statistics
    * Package: [lifelines](https://github.com/CamDavidsonPilon/lifelines), survival analysis
  * Supply chain
    * Package: [Supplychainpy](https://github.com/KevinFasusi/supplychainpy)
  * Webscraping
    * [Tutorial](https://towardsdatascience.com/byod-build-your-own-dataset-for-free-67133840dc85) (by Agarwal)
  * Convert PDF to html
    * Package: [PDFMiner](https://github.com/euske/pdfminer), then can be used to parse
  * Other fields
    * Package: [CobraPy](https://opencobra.github.io/cobrapy/), biological network modeling - constraints/optimization
    * ChemE [code](https://github.com/CAChemE/stochastic-optimization), optimize process simulators
  * Visualization / figures
    * [Python Graph Gallery](https://python-graph-gallery.com/) - lots of examples with code
    * [Overview](http://pythonplot.com/) of plotting for exploratory analysis (Hopper)
    * Seaborn [Examples](https://jakevdp.github.io/PythonDataScienceHandbook/04.14-visualization-with-seaborn.html)
    * Altair
      * Example code, [notebooks](https://github.com/altair-viz/altair_notebooks)
      * Video [tutorial](https://www.youtube.com/watch?v=ms29ZPUKxbU&t=2431s) from [@jakevdp](https://github.com/jakevdp)
    * R-style graphing
      * Package: [plotnine](https://plotnine.readthedocs.io/en/stable/)
      * Package: [ggplot](https://www.r-bloggers.com/ggplot2-style-plotting-in-python/)
    * Funny
      * [XKCD-style figures](https://matplotlib.org/xkcd/examples/showcase/xkcd.html)
* Notebooks
  * Package [nbdime](https://github.com/jupyter/nbdime) - version control with notebooks
  * Reproducible data analysis, ([videos](https://jakevdp.github.io/blog/2017/03/03/reproducible-data-analysis-in-jupyter/), VanderPlas)
  * "I don't like notebooks" ([slides](https://docs.google.com/presentation/d/1n2RlMdmv1p25Xy5thJUhkKGvjtV-dkAIsUXP-AL4ffI/edit#slide=id.g362da58057_0_1), Joel Grus)
  * "I like notebooks: Response to Joel Grus" ([slides](https://docs.google.com/presentation/d/1XmbeH_sdOKqhi05_FbH2EdRw948i8IvBz1PdfJGbhf4/edit#slide=id.p), Hopper)
* How to...
  * [Run code](https://marisacarlos.com/pages/how-to-run-python-file)
  * Set up
    * Add Python to PATH: [medium post](https://medium.com/@GalarnykMichael/install-python-on-windows-anaconda-c63c7c3d1444)
    * Install packages that aren't available via conda: [stackoverflow](https://stackoverflow.com/questions/41060382/using-pip-to-install-packages-to-anaconda-environment)
    * Install TensorFlow: [medium post](https://medium.com/@Oysiyl/install-tensorflow-1-8-0-with-gpu-from-source-on-ubuntu-18-04-bionic-beaver-35cfa9df3600)
    * Manage/use environments:
      * [conda docs](https://conda.io/docs/user-guide/tasks/manage-environments.html)
      * [tutorial](https://medium.freecodecamp.org/why-you-need-python-environments-and-how-to-manage-them-with-conda-85f155f4353c)
  * Export to file
    * [Strings](https://www.guru99.com/reading-and-writing-files-in-python.html)
    * Numpy array [to txt](https://docs.scipy.org/doc/numpy-1.15.0/reference/generated/numpy.savetxt.html)
    * Numpy array [to csv](https://stackoverflow.com/questions/6081008/dump-a-numpy-array-into-a-csv-file)
  * [Write unit tests](https://github.com/numpy/numpy/blob/master/doc/TESTS.rst.txt), SciPy
    * [FIRST principle](https://pragprog.com/magazines/2012-01/unit-tests-are-first)
* What's a...
  * Generator? [stackoverflow](https://stackoverflow.com/questions/1756096/understanding-generators-in-python)
  * _pycache_ file? [answer 1](https://www.python.org/dev/peps/pep-3147/), [answer 2](https://stackoverflow.com/questions/16869024/what-is-pycache)
* Humor
  * [xkcd 353](https://xkcd.com/353/)
  * [xkcd 1987](https://xkcd.com/1987/)

### R
* Reference
  * Free Textbooks
    * [An Introduction to R](https://cran.r-project.org/doc/manuals/r-release/R-intro.html)
    * [_Hands-On Programming with R_](https://rstudio-education.github.io/hopr/) (Grolemund)
    * [_R for Data Science_](https://r4ds.had.co.nz/) by [@hadley](https://github.com/hadley/) and [@garrettgman](https://github.com/garrettgman)
      * Some [solutions](https://jrnold.github.io/r4ds-exercise-solutions/) (Arnold)
    * [_R Programming for Data Science_](https://bookdown.org/rdpeng/rprogdatascience/) (Peng, 2019)
    * [_Advanced R_](https://adv-r.hadley.nz/) (Wickham)
      * Some [solutions](https://advanced-r-solutions.rbind.io/) (Grosser et al.)
    * [_R Packages_](http://r-pkgs.had.co.nz/) (Wickham)
    * [_Text Mining with R_](https://www.tidytextmining.com/) by [@juliasilge](https://github.com/juliasilge) and [@dgrtwo](https://github.com/dgrtwo/)
    * [_Exploratory Data Analysis with R_](https://bookdown.org/rdpeng/exdata/)(Peng, 2016)
    * [_Efficient R Programming_](https://bookdown.org/csgillespie/efficientR/) (Gillespie, Lovelace, 2016)
    * [_Functional programming and unit testing for data munging with R_](https://b-rodrigues.github.io/fput/) (Rodrigues, 2017)
    * [_R Markdown: The Definitive Guide_](https://bookdown.org/yihui/rmarkdown/) (Xie et al., 2019)
  * [Cheat sheets](https://www.rstudio.com/resources/cheatsheets/)
    * [Base R](https://www.povertyactionlab.org/sites/default/files/r-cheat-sheet.pdf)
    * ggplot2: [Two pages](https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf); [Longer](http://zevross.com/blog/2014/08/04/beautiful-plotting-in-r-a-ggplot2-cheatsheet-3/)
    * [Syntax comparison](http://www.science.smith.edu/~amcnamara/Syntax-cheatsheet.pdf): base R vs. formula vs. tidyverse
  * Styleguides
    * [From Google](https://google.github.io/styleguide/Rguide.xml)
    * [Tidyverse](http://style.tidyverse.org/)
  * [R Cookbook](http://www.cookbook-r.com/)
* [Search engine](https://rseek.org/) for R help
* Learn R
  * [Handbook](https://github.com/DARTH-git/R-Handbook/blob/master/Handbook_in_R_markdown.pdf) - Intro to R for Decision Modelers (Pechlivanoglou et al)
  * [Seminar code](https://stats.idre.ucla.edu/stat/data/intro_r/intro_r_flat.html) - Intro to R seminar code (IDRE)
  * Compilation of resources
    * [Arnholt](https://alanarnholt.github.io/resources.html)
  * Courses & collection of tutorials
    * [UC Business Analytics](http://uc-r.github.io/)
    * [Coding club](https://ourcodingclub.github.io/tutorials/), Univ. of Edinburgh
    * [Stat 545](http://stat545.com/topics.html), R course with many materials online
  * Websites
    * [R-bloggers](https://www.r-bloggers.com/)
    * [R FAQ](https://stackoverflow.com/questions/tagged/r-faq) on StackOverflow
    * [R Weekly](https://rweekly.org/), new R resources every week
* Communities/fora
  * [Tidy Tuesdays](https://github.com/rfordatascience/tidytuesday/blob/master/README.md), a weekly data viz project
    * Package: [TidyTuesdayR](https://github.com/thebioengineer/tidytuesdayR/) - to help download data
    * See results from each week: [TidyTuesdayRocks](https://nsgrantham.shinyapps.io/tidytuesdayrocks/) (Grantham)
  * [Community](https://medium.com/@kierisi/r4ds-the-next-iteration-d51e0a1b0b82) to walk through _R for Data Science_ book together
  * [R-Ladies](https://rladies-community-slack.herokuapp.com/) community on Slack
  * [RStudio Community](https://community.rstudio.com/)
* Packages/topics
  * Package: [EpiModel](http://www.epimodel.org/)
    * Short course [resources](http://www.epimodel.org/), [slides](http://statnet.github.io/sb/EpiModel-Slides.pdf)
    * [Gallery](https://github.com/statnet/EpiModel-Gallery) of extensions
  * dplyr
    * Joins
      * [Cheatsheet](http://stat545.com/bit001_dplyr-cheatsheet.html) (Stat 545)
      * [Gifs](https://github.com/gadenbuie/tidy-animated-verbs#tidy-animated-verbs) of join types (gadenbuie)
    * Tutorials
      * [Selecting columns](https://suzan.rbind.io/2018/01/dplyr-tutorial-1/)
      * [Filtering rows](https://suzan.rbind.io/2018/02/dplyr-tutorial-3/)
      * [Summarizing and slicing](https://suzan.rbind.io/2018/04/dplyr-tutorial-4/)
  * Bootstrapping
    * Package: [slipper](https://github.com/jtleek/slipper)
    * Package: [boot](https://cran.r-project.org/web/packages/boot/index.html)
      * [How to use](https://stats.idre.ucla.edu/r/faq/how-can-i-generate-bootstrap-statistics-in-r/)
  * Package: [reprex](https://github.com/tidyverse/reprex)
    * Prep short bits of code (e.g., to post on StackOverflow)
  * Webscraping
    * [Tutorial](http://www.interhacktives.com/2017/01/25/scrape-tweets-r-journalists/) by Watts, for journalists
    * [Tutorial](http://utstat.toronto.edu/~nathan/teaching/sta4002/Class1/scrapingtwitterinR-NT.html) by Taback
  * K-means
    * [Tutorial](https://uc-r.github.io/kmeans_clustering), UC Business
  * Package: [sociome](https://rdrr.io/github/NikKrieger/sociome/) - access to social determinants of health data
  * Stats
    * Package: [precisely](https://github.com/malcolmbarrett/precisely) - estimate power size based on precision
* Operations research
  * [Paper](http://josilber.scripts.mit.edu/IAPEducationPaperDistribute.pdf) on using R for OR
  * [Website](https://www.r-orms.org/) with resources
  * Package: [ompr](https://github.com/dirkschumacher/ompr) - mixed-integer LPs
  * Package: [optplot](https://github.com/dirkschumacher/optplot) - plot opt models
* Simulation
  * Microsimulation [tutorial](https://github.com/DARTH-git/Microsimulation-tutorial) (Krijkamp et al.)
* Statistics
  * Summary
    * Package: [summarytools](https://cran.r-project.org/web/packages/summarytools/vignettes/Introduction.html), e.g., `view(dfSummary(iris))`
  * Principal component analysis [tutorial](https://www.datacamp.com/community/tutorials/pca-analysis-r) (Hayden)
  * Survival analysis
    * Package: [survival](https://cran.r-project.org/web/packages/survival/index.html), base analysis
    * Package: [survminer](http://www.sthda.com/english/wiki/survminer-r-package-survival-data-analysis-and-visualization), improved visuals
      * [Cheatsheet](https://rpkgs.datanovia.com/survminer/survminer_cheatsheet.pdf)
    * [Tutorial](https://www.datacamp.com/community/tutorials/survival-analysis-R)
* Health economics
  * Package: [hesim](http://innovationvalueinitiative.github.io/hesim/), simulation
  * Package: [dampack](https://github.com/feralaes/dampack), decision-analytic models
* Math
  * ODEs: Package: [odin](https://github.com/mrc-ide/odin)
* Visualizations
  * Examples - [R Graph Gallery](https://www.r-graph-gallery.com/)
  * Create figures
    * Package: [ggplot2](https://ggplot2.tidyverse.org/)
    * Package: [ggpubr](http://www.sthda.com/english/rpkgs/ggpubr/) - wrapper around ggplot
      * Intended to be easier to create pub-ready figures
  * Package: [rvg](https://github.com/davidgohel/rvg) - export figures to be editable in Powerpoint
  * Package: magick, [vignette](https://cran.r-project.org/web/packages/magick/vignettes/intro.html) - image processing
  * Graphs and networks
    * [Tutorial](http://kateto.net/network-visualization) (Ognyanova)
    * Package: [DiagrammeR](https://github.com/rich-iannone/DiagrammeR)
      * [Example](http://yetanothermathprogrammingconsultant.blogspot.com/2018/07/graph-drawing-in-rstudio.html) (Kalvelagen)
    * Package: [Plotly](https://plot.ly/python/tree-plots/)
  * Gantt charts
    * Package: [GanttR](https://insileco.github.io/2017/09/20/gantt-charts-in-r/)
    * [Other options](https://stackoverflow.com/questions/3550341/gantt-charts-with-r)
  * Interactive timelines
    * Package: [timevis](https://github.com/daattali/timevis)
  * Spatial data
    * Package: [sf](https://github.com/r-spatial/sf), simple features
  * Maps
    * Package: [ggmap](https://github.com/dkahle/ggmap)
      * [Using Stamen maps](https://statisticaloddsandends.wordpress.com/2018/10/25/getting-started-stamen-maps-with-ggmap/) (Tay)
    * Package: [urbnmapr](https://github.com/UrbanInstitute/urbnmapr), state and county
  * Colors / themes
    * [Color/fill/transparency in ggplot2](https://ggplot2.tidyverse.org/reference/aes_colour_fill_alpha.html) (tidyverse)
    * RColorBrewer
      * [Explanation](https://moderndata.plot.ly/create-colorful-graphs-in-r-with-rcolorbrewer-and-plotly/) (by chelsea in R)
      * [GUI](http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3) to review options on a map
* Markdown/reports
  * Thesis [template](https://rosannavanhespenresearch.wordpress.com/category/writing-your-thesis-with-r-markdown/)
  * knitr html [template](http://biostat.mc.vanderbilt.edu/wiki/Main/KnitrHtmlTemplate)
  * Package: [Tufte](https://github.com/rstudio/tufte) - in style of Tufte
* How to...
  * Set up
    * [Update R](https://www.linkedin.com/pulse/3-methods-update-r-rstudio-windows-mac-woratana-ngarmtrakulchol), run in RGui, not RStudio
    * Have your code [text you](https://www.r-bloggers.com/let-r-python-send-messages-when-the-algorithms-are-done-training/) when done running
  * Data
    * List factor levels
      * [List all including those without observations - levels()](https://stackoverflow.com/questions/42856796/levels-of-factor-still-show-after-deleting-the-elements), could also use droplevels()
      * [Only list those with observations - unique()](https://chemicalstatistician.wordpress.com/2018/03/10/use-unique-instead-of-levels-to-find-the-possible-values-of-a-character-variable-in-r/) (Cai)
    * Add rows to dataframe
      * [Use list() rather than c() if types are mixed](https://stackoverflow.com/questions/28467068/add-row-to-dataframe)
  * Plot things
    * Axes
      * [Rearrange categories](https://trinkerrstuff.wordpress.com/2012/10/15/how-do-i-re-arrange-ordering-a-plot/)
      * [Convert axes to percents](https://stackoverflow.com/questions/27433798/how-to-change-y-axis-range-to-percent-from-number-in-barplot-with-r)
      * [Change size of title and labels](https://stackoverflow.com/questions/14942681/change-size-of-axes-title-and-labels-in-ggplot2)
      * [Rotate labels](http://tallman-world.tumblr.com/post/89964965867/rhow-to-rotate-axis-labels-in-ggplot2)
    * [Plot all data in background](https://drsimonj.svbtle.com/plotting-background-data-for-groups-with-ggplot2) on faceted ggplot2 figures
    * [Change colors](http://www.sthda.com/english/wiki/ggplot2-colors-how-to-change-colors-automatically-and-manually)
    * Iteratively make plots
      * [Using loops](https://ourcodingclub.github.io/2017/02/08/funandloops.html)
      * [Using purrr](https://dpananos.github.io/posts/2018/04/blog-post-8/) by [@dpananos](https://github.com/Dpananos)
    * Plot multiple figures
      * [Faceting](https://stackoverflow.com/questions/31798162/generating-multiple-plots-in-ggplot-by-factor), must be same plot type
      * Package: [cowplot](https://cran.r-project.org/web/packages/cowplot/vignettes/plot_grid.html) (Claus Wilke)
        * [Shared legends](https://cran.r-project.org/web/packages/cowplot/vignettes/shared_legends.html)
      * Package: [GridExtra](https://www.r-bloggers.com/extra-extra-get-your-gridextra/) - paneling ggplot figures
      * Function: [Multiplot](https://www.rdocumentation.org/packages/scater/versions/1.0.4/topics/multiplot)
      * If using [base R](https://www.statmethods.net/advgraphs/layout.html)
    * [Drill-down figures](https://plotly-r.com/linking-views-with-shiny.html#advanced-applications), with plotly
    * [Save high resolution figures](https://www.r-bloggers.com/high-resolution-graphics-with-r/)
  * [Fit distributions](http://www.di.fc.ul.pt/~jpn/r/distributions/fitting.html)
  * [Write an R package](https://github.com/jtleek/rpackages) by [@jtleek](https://github.com/jtleek)
* What is...
  * [::](https://stackoverflow.com/a/35241015)
  * Pipe operator %>%
    * [Short explanation](https://github.com/hadley/healthyr_preamble) from [@hadley](https://github.com/hadley/)
    * [Longer](https://www.datacamp.com/community/tutorials/pipe-r-tutorial) from DataCamp
  * [Environments, namespaces, etc.](http://blog.obeautifulcode.com/R/How-R-Searches-And-Finds-Stuff/) (Suraj Gupta)
* Humor or fun
  * Package: [Cowsay](https://cran.r-project.org/web/packages/cowsay/vignettes/cowsay_tutorial.html), tutorial - make animals say funny things
  * [Excel 2003 themed figures](https://cran.r-project.org/web/packages/ggthemes/vignettes/ggthemes.html)
  * Package: [GeomMLBStadiums](https://github.com/bdilday/GeomMLBStadiums) - draw baseball stadiums in ggplot2

### GitHub
  * Beginner [Tutorial](http://try.github.io/)
  * [Guide to Git with R](http://happygitwithr.com/)
  * Cheat sheets
    * [By Chris Albon](https://chrisalbon.com/git/github_cheatsheet/)
    * [By Joshua Hibbert](https://github.com/joshnh/Git-Commands)
    * [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
  * [Binder](https://mybinder.org/) - Convert Jupyter notebooks to executables
  * How to...
    * [Install git](https://www.develves.net/blogs/asd/articles/using-git-with-powershell-on-windows-10/#installing-git)
    * [Undo](https://www.atlassian.com/git/tutorials/undoing-changes)
    * [Save credentials](https://help.github.com/articles/caching-your-github-password-in-git/) (i.e., username/password)
    * [Exit git log](https://stackoverflow.com/questions/9483757/how-to-exit-git-log-or-git-diff) (soln: type 'q')
    * [Revert to older version](https://www.git-tower.com/learn/git/faq/restore-repo-to-previous-revision) (use new branch)
    * Repos
      * [Clone a repo](https://help.github.com/articles/cloning-a-repository/)
      * [Use cloned repo](https://stackoverflow.com/questions/14217406/why-i-cant-push-a-newly-cloned-repo)
    * Manage branches
      * [Merge](https://www.atlassian.com/git/tutorials/using-branches/git-merge)
      * [Delete](https://koukia.ca/delete-a-local-and-a-remote-git-branch-61df0b10d323)
    * Forking
      * [Tutorial](https://guides.github.com/activities/forking/)
    * Deal with errors:
      * [Local changes being overwritten](https://stackoverflow.com/questions/15745045/how-do-i-resolve-git-saying-commit-your-changes-or-stash-them-before-you-can-me)
      * [Unlink of file](https://stackoverflow.com/questions/4389833/unlink-of-file-failed-should-i-try-again) - essentially, had to close AMPL, then worked fine
  * What is...
    * [a bare repository?](http://www.saintsjd.com/2011/01/what-is-a-bare-git-repository/)
    * [Travis CI?](https://stackoverflow.com/questions/22587148/trying-to-understand-what-travis-ci-does-and-when-it-should-be-used)
  * Humor:
    * [xkcd 1597](https://xkcd.com/1597/)
    * [xkcd 1296](https://xkcd.com/1296/)


### AMPL
* Free textbook: [_AMPL_](https://ampl.com/resources/the-ampl-book/chapter-downloads/) (Fourer, Gay, and Kernighan)
* Intro to AMPL [Handout](http://www.math.wsu.edu/faculty/bkrishna/FilesMath567/S17/Handouts/Handout_AMPL_1.pdf) (Krishnamoorthy)
* Help forum: [Google group](https://groups.google.com/forum/#!forum/ampl)
* Specifics
  * [Dynamic set definitions](https://groups.google.com/forum/#!msg/ampl/Wr_KxvKWBpM/FGeILLXGZzAj), e.g., AVAIL vs. AVAIL_all
  * [argmin](https://ampl.com/faqs/i-have-declared-set-s-and-param-b-s-how-do-i-write-an-ampl-expression-for-the-arg-min-of-bi-that-is-the-s-in-s-such-that-bs-equals-the-minimum-of-bi-over-all-i-in-s/)
  * [Sampling discrete random variables from uniform distribution](https://groups.google.com/forum/#!msg/ampl/Wjl-PC-kkiY/FGgDMedidLkJ)

### Julia
  * How to use
    * [Manual](https://docs.julialang.org/en/v1/index.html)
    * [Style guide](https://docs.julialang.org/en/v1/manual/style-guide/)
    * [Cheat sheet](https://juliadocs.github.io/Julia-Cheat-Sheet/)
  * Free textbooks
    * [_Think Julia_](https://benlauwens.github.io/ThinkJulia.jl/latest/book.html) (Lauwens)
    * [_Julia Programming for Operations Research (ver1)_](https://www.softcover.io/read/7b8eb7d0/juliabook) (Kwon, [code](https://github.com/chkwon/jpor_codes))
  * Resource compilations
    * [Many resources](https://julialang.org/learning/) (Julia site)
    * [Lists of packages related to different areas](https://svaksha.github.io/Julia.jl/) (svaksha) - click on the .md links to see
  * Fora
    * [Discourse - optimization](https://discourse.julialang.org/c/domain/opt)
    * [Discourse - general Julia](https://discourse.julialang.org/)
    * [Slack channel](https://julialang.slack.com/), [link to invitation](https://slackinvite.julialang.org/)
    * [List of communities](https://julialang.org/community/)
  * Videos
    * [JuliaCon 2018 videos](https://discourse.julialang.org/t/juliacon2018-videos-on-youtube/13734)
    * [JuliaCon 2019 videos](https://www.youtube.com/playlist?list=PLP8iPy9hna6StY9tIJIUN3F_co9A0zh0H)
    * [Tutorials](https://www.youtube.com/playlist?list=PLP8iPy9hna6SCcFv3FvY_qjAmtTsNYHQE)
  * Operations research
    * [Optimization in Julia](http://www.juliaopt.org/) - nice summary of solvers at bottom of page
    * Modeling languages
      * [JuMP](http://www.juliaopt.org/JuMP.jl/0.18/) - general
      * [Convex.jl](https://convexjl.readthedocs.io/en/latest/) - disciplined convex
    * Solvers/algorithms
      * [JuliaStochOpt](https://github.com/JuliaStochOpt)
        * Including: [discrete-time stochastic control](https://github.com/JuliaStochOpt/StochDynamicProgramming.jl)
      * [SDDP](https://github.com/odow/SDDP.jl) (stochastic dual dynamic prog); [tutorials](https://odow.github.io/SDDP.jl/latest/index.html)
      * [SDDiP](https://github.com/lkapelevich/SDDiP.jl) (SDDP with integer variables)
      * [StructJuMP](https://github.com/StructJuMP/StructJuMP.jl) (2-stage stochastic programs)
      * [DSP](https://github.com/Argonne-National-Laboratory/DSPsolver.jl) (stochastic mixed-integer)
      * [Complementarity.jl](https://github.com/chkwon/Complementarity.jl) (mixed-complementarity and math programs with equilibrium problems)
      * [CLP](https://github.com/JuliaOpt/Clp.jl) - COIN-OR LP solver
      * [L-shaped solver](https://github.com/martinbiel/LShapedSolvers.jl)
    * Specifics
      * [Rolling horizon](https://discourse.julialang.org/t/rolling-horizon-implementation/23048)
  * Other math/CS
    * [Evaluate derivatives](http://www.juliadiff.org/)
    * [Differential equations](http://juliadiffeq.org/)
    * [Calculus](https://github.com/JuliaMath/Calculus.jl)
    * [Machine learning](https://github.com/JuliaML)
      * [Tutorial](https://www.cs.purdue.edu/homes/hnassar/JPUG/ML-Tutorial.html) (JPUG)
    * Game Theory
      * [Tutorial](https://nbviewer.jupyter.org/github/QuantEcon/QuantEcon.notebooks/blob/master/game_theory_jl.ipynb)
  * [Plots](http://docs.juliaplots.org/latest/)
    * [Tutorial](https://www.cs.purdue.edu/homes/hnassar/JPUG/plotting.html) (JPUG)
    * [Tutorial](http://docs.juliaplots.org/latest/tutorial/#tutorial-1) (documentation)
    * [Formatting and style by backend](http://docs.juliaplots.org/latest/supported/#supported-1)
  * Performance
    * Tips ([from manual](https://docs.julialang.org/en/v1/manual/performance-tips); [from JPUG](https://www.cs.purdue.edu/homes/hnassar/JPUG/performance.html))
    * Package: [TimerOutputs.jl](https://github.com/KristofferC/TimerOutputs.jl)
    * Package: [BenchmarkTools.jl](https://github.com/JuliaCI/BenchmarkTools.jl)
  * Other
    * [OhMyREPL.jl](https://github.com/KristofferC/OhMyREPL.jl) (syntax highlighting in REPL)
    * Parallel computing
      * [Overview](https://docs.julialang.org/en/v1/manual/parallel-computing/index.html)
      * [Tutorial](https://codingclubuc3m.github.io/2018-06-06-Parallel-computing-Julia.html) (García-Heredia)
      * [parallel_computing.jl](https://www.cs.purdue.edu/homes/hnassar/JPUG/parallel_computing.jl) (Nassar)
      * [Caching pool](https://github.com/JuliaOpt/Gurobi.jl/issues/119#issuecomment-375445961) (odow)
      * Examples
        * [Gurobi](https://discourse.julialang.org/t/parallel-solves-in-gurobi-jl/9908/2) (odow)
        * [JuMP and Ipopt] (https://discourse.julialang.org/t/running-jump-using-ipopt-in-parallel/9167)
  * Package dev and workflow
    * [Create and register a package](https://attractivechaos.wordpress.com/2018/09/26/creating-a-new-package-in-julia/) (attractivechaos)
    * [Create local package](https://stackoverflow.com/questions/29211641/julia-create-and-use-a-local-package-without-internet)
    * [Workflow v1.0](https://medium.com/@Jernfrost/my-new-workflow-with-julia-1-0-99711103d97c) (Engheim)
    * Patching packages
      * [Discourse answer 1](https://discourse.julialang.org/t/recommended-way-to-develop-fix-with-packages/14436/12) (sdewaele)
      * [Discourse answer 2](https://discourse.julialang.org/t/develop-a-local-version-of-a-registered-package-and-submit-changes-as-a-pull-request/24868) (CameronBieganek)
    * [Unit testing](https://docs.julialang.org/en/v1/stdlib/Test/)
  * How to:
    * [Install a package the first time](https://stackoverflow.com/questions/51793629/how-to-install-a-package-in-julia-1-0-undefvarerror-pkg-not-defined)
    * [Install a specific version of a package](https://julialang.github.io/Pkg.jl/v1/managing-packages/) (answered within the first section)
    * [Install a package from github](https://github.com/JuliaPolyhedra/QHull.jl/issues/21#issuecomment-429418324) (example)
    * Suppress multiple Gurobi license messages - send environment to solver: [v1](https://discourse.julialang.org/t/suppress-license-output-from-solver-in-jump-model/20828/4)
  * What is:
    * The ! after a function name? (answer)[https://stackoverflow.com/questions/45396685/what-does-exclamation-mark-means-after-the-name-of-functions]

### Other programming languages
* SQL
  * [Sequel Pro]( https://www.sequelpro.com/) - for Mac
* MATLAB
  * [FAST](https://web.stanford.edu/~lcambier/fast/index.php) - Stochastic dual dynamic programming (open-source)
  * [Optimization](https://www.mathworks.com/products/optimization.html) (paid)
  * [Global optimization](https://www.mathworks.com/products/global-optimization.html) (paid)

### General coding / computation
  * Overview/best practices
    * Overview ([slides](http://reckoningrisk.com/research-practice/coding/2018/better-coding-practices) from [@tommlogan](https://github.com/tommlogan))
    * [Best practices](https://rawgit.com/marcio-mourao/Programming-Best-Practices/master/Workshop.html) from [@marcio-mourao](https://github.com/marcio-mourao)
    * [Good enough practices](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510) (Wilson et al.)
    * [Best practices](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745) (Wilson et al.)
    * [Coding standards](https://eecs280staff.github.io/eecs280.org/assets/EECS_280_Coding_Standards.pdf) (EECS 280, UM)
  * Textbooks
    * [Compilation of free textbooks](https://github.com/EbookFoundation/free-programming-books/blob/master/free-programming-books.md)
  * Courses
    * System and Software Tools ([slides](https://courses.cs.washington.edu/courses/cse391/16sp/index.shtml))
    * Intro to computing for computer scientists ([lectures](https://c4cs.github.io/))
      * E.g., Linux, command line, version control, shells, scripting
    * Computing for Social Sciences ([slides, resources, etc.](https://cfss.uchicago.edu/syllabus.html))
    * Data Skills for Reproducible Science ([notes, code](https://gupsych.github.io/data_skills/))
    * Software Carpentry [many resources](https://github.com/swcarpentry/swcarpentry)
    * Intro to Biomedical Data Science ([materials](https://bims8382.github.io/2018/))
  * Command line
    * Bash
      * [Shell commands](https://courses.cs.washington.edu/courses/cse391/16sp/bash.html)
      * [Reference manual](https://www.gnu.org/software/bash/manual/bashref.html)
    * [Overview](http://linuxcommand.org/index.php) (William Shotts)
    * Free textbook: [_The Linux Command Line_](http://linuxcommand.org/tlcl.php) (William Shotts)
    * Intro ([slides](https://cscar.research.umich.edu/wp-content/uploads/sites/5/2016/09/Intro-to-Command-Line.pdf), UM CSCAR)
  * Linux
    * [Intro course](https://training.linuxfoundation.org/training/introduction-to-linux/) (free online)
  * Remote computing
    * SSH - aka Secure Shell (allows secure remote login even if network insecure)
      * [PuTTy](https://www.putty.org/)
    * File transfer
      * [WinSCP](https://winscp.net/eng/download.php) - Windows
      * [Cyberduck](https://cyberduck.io/) - Mac/Windows
      * Large files: [Globus](https://www.globus.org/)
        * Basic version for research/education is free
    * Cluster computing
      * [PBS overview](https://www.youtube.com/watch?v=SW8Lu1-JaSM) (batch scripting, 40min video)
      * Unixm
        * Book: [_The Unix Workbench_](https://seankross.com/the-unix-workbench/) (Kross)
        * [Tutorial for beginners](http://info.ee.surrey.ac.uk/Teaching/Unix/index.html)
        * [vi commands](https://www.cs.colostate.edu/helpdocs/vi.html)
  * Text editors
    * [Atom](https://atom.io/)
      * [Keyboard shortcuts](https://github.com/nwinkler/atom-keyboard-shortcuts/blob/master/README.md) (nwinkler)
    * [Vim](https://www.vim.org/)
      * Game to learn Vim: [Vim Adventures](https://vim-adventures.com/)
    * [Emacs](https://www.gnu.org/software/emacs/)
    * [Visual Studio Code](https://code.visualstudio.com/)
    * [Sublime](https://www.sublimetext.com/)
    * [Nano](https://www.nano-editor.org/)
  * Share code
    * [Carbon](https://carbon.now.sh) - nice formatting for screenshotting code
  * Parallel computing
    * [Intro](https://computing.llnl.gov/tutorials/parallel_comp/)(Barney)
  * Servers
    * [The introduction to servers I wish I'd had](https://dev.to/harri_etty/the-introduction-to-servers-i-wish-i-d-had-44jl) (Harriet)
  * What are/is...
    * [src vs. bin folders?](https://www.quora.com/Eclipse-software-Whats-the-difference-between-the-bin-and-src-folders)
    * the difference between statically and dynamically typed lanugages? [stackoverflow](https://stackoverflow.com/questions/1517582/what-is-the-difference-between-statically-typed-and-dynamically-typed-languages); [blogpost](https://pythonconquerstheuniverse.wordpress.com/2009/10/03/static-vs-dynamic-typing-of-programming-languages/) (From Python Conquers)
  * How to...
      * [Add environment variables/PATH](https://helpdeskgeek.com/windows-10/add-windows-path-environment-variable/)

### Math programming software
* Overviews
  * [From Math Opt Society](http://www.mathopt.org/Optima-Issues/optima103.pdf) (Sept 2017)
  * [Convex MINLP solver comparison](http://www.optimization-online.org/DB_FILE/2018/06/6650.pdf) (Jun 2018)
  * Benchmarks
    * [Linear programs](http://plato.asu.edu/ftp/lpsimp.html) - simplex (Mittelmann)
* Solvers
  * Commercial
    * [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio) (free for academics)
    * [Gurobi](http://www.gurobi.com/) (free for academics)
    * [Xpress](https://community.fico.com/community/fico-optimization-community)
    * [MOSEK](https://www.mosek.com/), especially SOCP, SDP
  * Non-commercial
    * [GLPK](https://www.gnu.org/software/glpk/) (LP, MIP)
    * [SCIP](http://scip.zib.de/) (MIP, MINLP, constraint IP)
    * [Bonmin](https://projects.coin-or.org/Bonmin) (MINLP)
    * [Couenne](https://projects.coin-or.org/Couenne) (Non-convex MINLP)
    * [MAiNGO](https://www.avt.rwth-aachen.de/cms/AVT/Forschung/Software/~rggn/Globale-Optimierung/lidx/1/) (MINLP)
    * NEOS:
      * [Server](https://neos-server.org/neos/)
      * [Guide](https://neos-guide.org/)
    * [Concorde](http://www.math.uwaterloo.ca/tsp/concorde/index.html) (TSP - traveling salesman)
    * [OpenSolver](https://opensolver.org/) - Excel add-in, extends standard Excel solver
    * [Ipopt](https://projects.coin-or.org/Ipopt) (nonlinear, local)
    * [BiqBin](http://biqbin.fis.unm.si/) (Binary quadratic)
    * [DSP](https://github.com/Argonne-National-Laboratory/DSP) (Stochastic mixed-integer programs)
    * [ECOS](https://github.com/embotech/ecos) (Second-order conic programs), [website](https://www.embotech.com/ECOS)
    * [OSQP](https://osqp.org/) (Operator Splitting Quadratic Program)
    * [Mini-CP](https://minicp.bitbucket.io/) (Constraint programming)
    * [Dakota](https://dakota.sandia.gov/)
  * [OR-Tools](https://developers.google.com/optimization/) from Google
* Modeling lanugages
  * [SolverStudio](http://solverstudio.org/) (free) - Excel add-on, useful when OpenSolver not big enough
  * [AMPL](https://ampl.com/)
  * [OPL](https://www.ibm.com/analytics/data-science/prescriptive-analytics/optimization-modeling)
  * [LP add-on for Google sheets](https://developers.google.com/optimization/lp/add-on)
* Application specific
  * Facility location
    * [SITATION](https://daskin.engin.umich.edu/software/)
  * Agent-based
    * [NetLogo](https://ccl.northwestern.edu/netlogo/)


### Math programming resources
* Textbooks available for free
  * [_A First Course in Linear Optimization v3.0_](https://github.com/jon77lee/JLee_LinearOptimizationBook/blob/master/JLee.3.0.pdf) by [@jon77lee](https://github.com/jon77lee/)
  * [_Decision Modeling_](https://linney.mun.ca/pages/view.php?ref=36808) (David M. Tulett, author-provided source) - optimization for undergrads
  * [_Convex Optimization_](http://www.seas.ucla.edu/~vandenbe/cvxbook.html) (Stephen Boyd and Lieven Vandenberghe)
  * [_MOSEK Modeling Cookbook_](https://themosekblog.blogspot.dk/2018/05/new-modeling-cookbook.html)
    * Conic optimization, not specific to MOSEK solver
  * [_Foundations and Methods of Stochastic Simulation_](http://users.iems.northwestern.edu/~nelsonb/IEMS435/) (Barry Nelson)
  * [_Intro to Applied Linear Algebra_](https://web.stanford.edu/~boyd/vmls/) (Stephen Boyd and Lieven Vandenberghe)
  * [Myths and Counterexamples](https://glossary.informs.org/myths/CurrentVersion/myths.pdf) (Harvey Greenberg)
  * [_Iterative Methods in Combinatorial Optimization_](https://www2.isye.gatech.edu/~msingh94/book.html) (Lau et al., 2011)
* Communities / forums
  * [Operations Research Stack Exchange](https://or.stackexchange.com)
  * No longer in use: [OR Exchange](https://www.or-exchange.org/)
  * Google groups
    * [AMPL](https://groups.google.com/forum/#!forum/ampl)
    * [Gurobi](https://groups.google.com/forum/#!forum/gurobi)
    * [AIMMS](https://groups.google.com/forum/#!forum/aimms)
    * [Pyomo](https://groups.google.com/forum/#!forum/pyomo-forum)
  * [Stack Overflow](https://stackoverflow.com/)
  * [Optimization Online](http://www.optimization-online.org/) (preprint site)
  * [IE faculty listserv](https://lists.clemson.edu/mailman/listinfo/iefac.list), e.g., job postings, etc.
* Overviews
  * [Glossary](https://glossary.informs.org/ver2/mpgwiki/index.php?title=Main_Page)
  * [OR Notes](http://people.brunel.ac.uk/~mastjjb/jeb/or/orweb.html) (JE Beasley)
* Models
  * [GAMS model library](https://www.gams.com/latest/gamslib_ml/libhtml/)
* Algorithms
  * [List/explanation](https://neos-guide.org/algorithms) from the folks at NEOS
* Test sets/libraries
  * Compilation: [on OR.SE](https://or.stackexchange.com/questions/244/optimization-problem-libraries/246), [on GitHub](https://github.com/ekhoda/optimization_problem_libraries)
  * [MIPLIB](http://miplib.zib.de/)
  * [OR Library](http://people.brunel.ac.uk/~mastjjb/jeb/info.html)
  * [TSPLIB](https://www.iwr.uni-heidelberg.de/groups/comopt/software/TSPLIB95/)
  * [Networks](http://networkrepository.com/dimacs.php) (DIMACS)
  * [MINLP](https://wiki.mcs.anl.gov/leyffer/index.php/MacMINLP) in AMPL
  * [VRP-REP](http://www.vrp-rep.org/) - vehicle routing
    * Commonly used (per Laporte 2007): [CMT, 1979](http://www.vrp-rep.org/references/item/christofides-et-al-1979.html), [GWKC, 1998](http://www.vrp-rep.org/datasets/item/2014-0004.html)
  * Facility location
    * [Bilde-Krarup](http://resources.mpi-inf.mpg.de/departments/d1/projects/benchmarks/UflLib/BildeKrarup.html) (Quite old - 1977)
* Course resources
  * Math Programming (generally)
    * [Notes](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-251j-introduction-to-mathematical-programming-fall-2009/lecture-notes/) (Bertsimas, Fall 2009)
    * Large-scale opt: [Slides](http://www.seas.ucla.edu/~vandenbe/ee236c.html) (Vandenberghe, 2016)
    * [Several courses](http://homepages.rpi.edu/~mitchj/courses.html) (Mitchell)
    * [Video tutorials](https://homepages.rpi.edu/~sharkt/ORMVideos.html) (Sharkey, Nurre)
  * Linear programming
    * [Slides](http://www.seas.ucla.edu/~vandenbe/ee236a/ee236a.html) (Vanedenberghe, 2013)
  * Combinatorial optimization
    * [Lecture notes](https://homepages.cwi.nl/~lex/files/dict.pdf) (Schrijver, 2017)
    * [Lecture notes](https://ocw.mit.edu/courses/mathematics/18-997-topics-in-combinatorial-optimization-spring-2004/index.htm) (Goemans, Spring 2004)
    * [Notes](https://courses.engr.illinois.edu/cs598csc/sp2010/) (Chekuri, Spring 2010)
  * Computational methods
    * [Notes](https://people.orie.cornell.edu/bdg79/ORIE6125/index.html) (Grimmer, Ding 2018)
  * Convex Optimization
    * [Slides](http://www.seas.ucla.edu/~vandenbe/cvxbook/bv_cvxslides.pdf) (Vandenberghe)
    * [Slides](http://www.seas.ucla.edu/~vandenbe/ee236b/ee236b.html) (Vandenberghe, 2019)
    * [Slides](http://www.ifp.illinois.edu/~angelia/convex_optimization_lectures.htm) (Nedich)
    * Convex Opt II
      * [Notes](https://web.stanford.edu/class/ee392o/) (Boyd and Luo, Fall 2003)
      * [Slides, notes](https://web.stanford.edu/class/ee364b/lectures.html) (Duchi)
      * [Notes](http://statweb.stanford.edu/~candes/math301/hand.html) (Candes)
  * Applied numerical computing
    * [Slides, notes](http://www.seas.ucla.edu/~vandenbe/ee133a.html) (Vandenberghe, 2018)
  * Stochastic programming
    * [Videos, slides](http://uclengiechair.be/operations-research-linma-2491/) (Papavasiliou)
    * [Lecture notes](https://www2.isye.gatech.edu/people/faculty/Alex_Shapiro/SPbook.pdf) (Shapiro, Dentcheva, Ruszczynski)
    * [Readings](https://castlelab.princeton.edu/orf-544/) (Powell, Fall 2017)
  * Optimal Learning
    * [Various materials](http://optimallearning.princeton.edu/) (Powell)
  * Opt for machine learning
    * [Slides](https://github.com/udellgroup/orie7191) (Udell)
  * SDP
    * [Slides](http://www.mit.edu/~parrilo/cdc03_workshop/index.html) (Parrilo, Lall)
  * Scheduling theory and applications
    * [Slides and handouts](https://sites.google.com/site/karmelshehadeh/Teaching/SCHEDULING-THEORY-AND-ALGORITHMS-COURSEWINTER-2018-UMICH) (Shehadeh, Winter 2018)
* OR in practice
  * [Wagner Prize Videos](https://www.informs.org/Resource-Center/Video-Library/Wagner-Competition-Videos) (INFORMS)
* Other
  * [IFORS Developing Countries page](http://ifors.org/developing_countries/index.php?title=Main_Page) - a variety of open-source resources
  * [OR societies around the world](http://people.brunel.ac.uk/~mastjjb/jeb/or/orweb.html)
  * [COIN-OR Foundation](https://www.coin-or.org/)
    * [Resources](https://www.coin-or.org/resources/)
  * INFORMS tutorials ([videos](https://www.informs.org/Resource-Center/Video-Library/INFORMS-TutORials))
* Topics
  * Benders Decomposition
    * [Using callbacks](https://orinanobworld.blogspot.com/2011/10/benders-decomposition-then-and-now.html) to avoid rebuilding the scenario tree by [@parubin](https://twitter.com/parubin)
    * Examples:
      * [In AMPL](https://ampl.com/NEW/LOOP2/)
      * [With callbacks](http://www.zverovich.net/2013/09/01/modern-benders-decomposition-in-ampl.html) by [@vitaut](https://github.com/vitaut)
  * Decision diagrams for integer programming
    * [Slides](http://www.andrew.cmu.edu/user/vanhoeve/mdd/presentations/DD%20IP%20EURO%202019.pdf) (van Hoeve)
  * Disjunctive programming
    * [Overview from GAMS](https://www.gams.com/latest/docs/UG_EMP_DisjunctiveProgramming.html)
    * [Video](https://www.youtube.com/watch?v=dfgzaVd8gLg) (Ruiz)
  * Gradient descent
    * [Intro](https://hbfs.wordpress.com/2012/04/24/introduction-to-gradient-descent/) Blogpost (Pigeon)
  * MINLP (Mixed-integer nonlinear programming)
    * [Overview](http://egon.cheme.cmu.edu/ewocp/docs/EWOMINLPGrossmann.pdf) (Grossmann)
    * [Slides](http://coral.ie.lehigh.edu/wp-content/uploads/presentations/siopt-05-minlp-presentation.pdf) (Leyffer and Linderoth, in 2005)
  * Nonlinear optimization
    * [Slides](http://cepac.cheme.cmu.edu/pasilectures/biegler/BieglerLecture.pdf) (Biegler)
    * [Short course slides](https://www.minlp.org/pdf/Bologna07.pdf) (Wachter)
  * Numerical issues
    * [Gurobi guidelines](http://www.gurobi.com/documentation/8.1/refman/numerics_gurobi_guidelines.html)
  * SDP (Semidefinite programming)
    * [Rendl 1](http://www.ipco2008.deis.unibo.it/summerschool/Rendl_bertinoro1.pdf), [Rendl 2](http://www.ipco2008.deis.unibo.it/summerschool/Rendl_bertinoro2.pdf)
  * Subgradient methods
    * [Notes](https://web.stanford.edu/class/ee364b/lectures/subgrad_method_notes.pdf) (Boyd) - minimize convex function, non-differentable
  * Supply chain
    * [XSG game](https://istm.zu.ac.ae/xsg), [overview](https://sinansalman.github.io/xsg/) - supply chain simulation game (Salman)
  * Variables
    * Semicontinuous ([post by Rubin](https://orinanobworld.blogspot.com/2011/03/semicontinuous-variables.html), [post by Kalvelagen](http://yetanothermathprogrammingconsultant.blogspot.com/2016/08/semi-continuous-variables.html))
    * Semi-integer ([post by Kalvelagen](http://yetanothermathprogrammingconsultant.blogspot.com/2015/12/a-model-with-semi-integer-variables.html))
* How to...
  * [Linearize product of variables](https://www.leandro-coelho.com/linearization-product-variables/)
  * [Linearize max/max/absolute value](https://www.leandro-coelho.com/how-to-linearize-max-min-and-abs-functions/)
  * [Linearize max(0,y)](https://orinanobworld.blogspot.com/2010/12/lps-and-positive-part.html) by [@prubin73](https://github.com/prubin73)
  * Remember primal / dual conversion
    * [Sensible-odd-bizarre (SOB) method](https://math.stackexchange.com/questions/83844/simplex-method-duality-by-bazaraa?answertab=oldest#tab-top), citing [this paper](https://www.math.hmc.edu/~benjamin/papers/sob.pdf)

### Operations research-adjacent material
* Linear Algebra
  * Videos
    * [Intuitive overview](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) (~2hrs, 3Blue1Brown)
    * [Intro course lectures](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/) (Strang)
  * Review and reference ([handout](http://cs229.stanford.edu/section/cs229-linalg.pdf), Kolter and Do)
  * Intro to matrix algebra ([handout](http://ibgwww.colorado.edu/%7Ecarey/p7291dir/handouts/matrix.algebra.pdf), Carey)
  * [Course notes, exercises, book](http://vmls-book.stanford.edu/) (Boyd and Vandenberghe)
* Economics and game theory
  * Game theory
    * [Intro course lectures](https://oyc.yale.edu/economics/econ-159) (Ben Polak)
    * [Course slides](http://www.ifp.illinois.edu/~angelia/game_lectures.htm) (Nedich)
  * [Slides from several courses](https://www.sas.upenn.edu/~jesusfv/teaching.html) (Fernández-Villaverde)
    * Including: computational methods; tools; macro dynamics; graduate macro; macro uncertainty shocks; equil macro; global econ history; political econ of early America
* Networks
  * Free textbook: [_Networks, Crowds, and Markets_](http://www.cs.cornell.edu/home/kleinber/networks-book/) (Easley, Kleinberg), intro undergrad
  * [List of resources](https://github.com/briatte/awesome-network-analysis) (briatte)
  * Bayes nets
    * [Tutorial](https://www.norsys.com/tutorials/netica/secA/tut_A1.htm) (Netica)
    * [Intro slides](https://www.cs.cmu.edu/afs/cs/academic/class/15381-s07/www/slides/032707bayesNets1.pdf) (CMU)
* Data Science
  * How to get started
    * [Blog post](https://www.jessemaegan.com/post/data-science-with-r-how-do-i-start/) by [@kierisi](https://github.com/kierisi)
    * [Plan](http://seankross.com/notes/data-science-from-scratch/) (Kross)
  * [Directory](http://www.datasciguide.com/content/) of materials (DataSciGuide)
  * [DataFramed podcast](https://www.datacamp.com/community/podcast) (DataCamp)
  * Courses
    * Foundations of Data Science ([video, slides, assignments](http://data8.org/), Berkeley)
      * [Textbook](https://www.inferentialthinking.com/chapters/intro) (Adhikari, DeNero)
    * Applied data science ([course readings](https://github.com/hadley/stats337#readings) from [@hadley](https://github.com/hadley/))
    * Intro to data ethics ([course module](https://www.scu.edu/ethics/focus-areas/technology-ethics/resources/an-introduction-to-data-ethics/), Shannon Vallor)
  * Examples
    * [Work habits and bicycles](https://jakevdp.github.io/blog/2015/07/23/learning-seattles-work-habits-from-bicycle-counts/) (VanderPlas)
* Machine Learning
  * Communities
    * [Google group](https://groups.google.com/forum/#!forum/ml-news/categories)
    * [CrossValidated](https://stats.stackexchange.com/), stackexchange
  * Textbooks
    * [_Intro to Statistical Learning_](https://www-bcf.usc.edu/~gareth/ISL/) (James et al.)
    * [_Elements of Statistical Learning_](https://web.stanford.edu/~hastie/ElemStatLearn/) (Hastie, Tibshirani, Friedman) - more technical than James et al. book
    * [_Statistical Learning with Sparsity_](https://web.stanford.edu/~hastie/StatLearnSparsity/index.html) (Hastie, Tibshirani, Wainwright)
    * [_A Brief Intro to ML for Engineers_](https://arxiv.org/abs/1709.02840) (Simeone)
    * [_Fairness in ML_](http://fairmlbook.org/) (Barocas, Hardt, Narayanan) - book in progress
  * [Technical Notes - ML and AI](https://chrisalbon.com/#machine_learning) from [@chrisalbon](https://github.com/chrisalbon)
  * [ML flashcards](https://machinelearningflashcards.com/) from [@chrisalbon](https://github.com/chrisalbon)
    * [Scrape off Twitter](https://github.com/Dpananos/GetCards) for free ([@Dpananos](https://github.com/Dpananos))
  * Courses
    * [Recordings, slides](http://www.cs.columbia.edu/~amueller/comsw4995s18/schedule/) ([@amueller](https://github.com/amueller))
    * [Recordings, slides](https://www.r-bloggers.com/in-depth-introduction-to-machine-learning-in-15-hours-of-expert-videos/) (Hastie, Tibshirani)
    * [Course notes](http://web.eecs.umich.edu/~cscott/past_courses/eecs545f15/index.html) (Clayton Scott)
    * [Notes, slides](https://github.com/thejakeyboy/umich-eecs545-lectures) (Abernathy)
    * [Learning with big messy data - Slides](https://people.orie.cornell.edu/mru8/orie4741/lectures.html) (Udell)
  * Topics
    * [How decision trees work](https://brohrer.github.io/how_decision_trees_work.html) (Rohrer)
    * [Taxonomy of reproducibility](http://www.rctatman.com/files/2018-7-14-MLReproducability.pdf)
    * [Monte Carlo tree search](https://int8.io/monte-carlo-tree-search-beginners-guide/)
    * [Data leakage](https://machinelearningmastery.com/data-leakage-machine-learning/) (Brownlee)
* Deep learning
  * [Slides](https://github.com/Kinghsy/EECS-498-598-Deep-Learning) (EECS 498-598)
* Compilations
  * [From Vodrahalli](https://kiranvodrahalli.github.io/links/)
  * [From Finlayson](https://sgfin.github.io/learning-resources/)
* Statistics
  * Communities/forums
    * [datamethods](https://discourse.datamethods.org/) - health-related stats forum
    * [Talk Stats](http://talkstats.com/)
    * [CrossValidated](https://stats.stackexchange.com/)
  * Books
    * [_Causal Inference_](https://www.hsph.harvard.edu/miguel-hernan/causal-inference-book/) (Hernan and Robins)
      * [Notes about book](https://sgfin.github.io/2019/06/19/Causal-Inference-Book-Glossary-and-Notes/) (Finlayson)
      * [DAGs from book](https://sgfin.github.io/2019/06/19/Causal-Inference-Book-All-DAGs/) (Finlayson)
  * [Glossary of Statistical Terms](http://hbiostat.org/doc/glossary.pdf) (Harrell)
  * [10 rules to use stats](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004961) (comp biology)
  * [Essential statistics with R](https://bims8382.github.io/2018/r-stats.html) ()
  * [Document and avoid these problems](http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist) (biostat)
  * [StatPrimer](http://www.sjsu.edu/faculty/gerstman/StatPrimer/) (Gerstman)
  * Courses
    * [Clinical trials - design/analysis](https://newonlinecourses.science.psu.edu/stat509/node/164/) (Penn State, notes)
  * Tests
    * [What test should I use?](https://stats.idre.ucla.edu/other/mult-pkg/whatstat/) (Examples in R, Stata, SAS, SPSS)
    * [t-tests](https://pharmafactz.com/pharmaceutical-calculations-comparing-two-means-using-t-test/)
  * Specific topics
    * Odds ratios ([Best practices](https://jamanetwork.com/journals/jama/fullarticle/2686777); Norton, Dowd, Maciejewski, paywall)
    * Dirichlet processes ([notes](http://dp.tdhopper.com/) by [@tdhopper](https://github.com/tdhopper))
    * Experimental design ([warning signs](http://norvig.com/experiment-design.html), Norvig)
    * Survival analysis ([overview](https://www.theanalysisfactor.com/the-six-types-of-survival-analysis-and-challenges-in-learning-them/), Grace-Martin)
  * [Same stats for different data](https://www.autodeskresearch.com/publications/samestats)
* Probability
  * [Review](https://www.cs.mcgill.ca/~dprecup/courses/ML/Materials/prob-review.pdf) (Maleki and Do)
* Mathematics
  * [Primers](https://jeremykun.com/primers/) (Kun)
  * [Notes](http://www.math.uconn.edu/~kconrad/blurbs/) (Conrad)
  * [Compilation of courses](https://hackernoon.com/be-a-better-programmer-with-these-40-mathematics-courses-d8ca48a2f8a2) (Dhar)
  * Boolean functions
    * [Lecture videos](http://www.cs.cmu.edu/~odonnell/aobf12/) (O'Donnell)
    * Free textbook: [_Analysis of Boolean Functions_] (http://www.contrib.andrew.cmu.edu/~ryanod/?page_id=2334) (O'Donnell)
* Computer science
  * [FAQ about C](http://c-faq.com/index.html)
* Ethics and social good
  * Mechanism design for social good ([Reading list](http://md4sg.com/researchgroup/index.html))
  * Ethics and policy in data science ([syllabus](https://docs.google.com/document/d/1GV97qqvjQNvyM2I01vuRaAwHe9pQAZ9pbP7KkKveg1o/edit))
* Other
  * [Compilation of lots of resources for students](https://github.com/dipakkr/A-to-Z-Resources-for-Students#a-to-z-resources-for-students-boy-) (FrontBench)
  * [Blockchain overview](https://www.youtube.com/watch?v=qOVAbKKSH10) (2 hr video)
  * [Gentle intro to graph theory](https://medium.com/basecs/a-gentle-introduction-to-graph-theory-77969829ead8) (Joshi)
  * [Habits of highly mathematical people](https://medium.com/@jeremyjkun/habits-of-highly-mathematical-people-b719df12d15e) (Kun)

### Data visualization
* Free Textbooks
  * [_Fundamentals of Data Visualization_](http://serialmentor.com/dataviz/) by [@clauswilke](https://github.com/clauswilke)
  * [_Data Visualization: A Practical Introduction_](http://socviz.co/) by [@kjhealy](https://github.com/kjhealy)
* Course
  * Data viz [Videos](https://www.youtube.com/playlist?list=PLehuLRPyt1HzQoXEhtNuYTmd0aNQvtyAK), Ghodsi, U. Waterloo
* Color
  * [Guide to using color](https://blog.datawrapper.de/colorguide/) (Rost)
  * [Color oracle](http://colororacle.org/) - convert screen to what a color blind person would see
* Networks
  * [Overview of software, etc.](https://www.lib.ncsu.edu/measuring-research-impact/visualizing-impact), NC State
  * [Gephi](https://gephi.org/)
    * [Tutorial](https://www.lib.ncsu.edu/sites/default/files/ResearchImpactNetworkGuide.pdf) - create citation network, NC State
  * [Example - citation network](http://nealcaren.web.unc.edu/a-sociology-citation-network/) (Caren, using Python & d3.js)
  * [Graphviz](http://graphviz.readthedocs.io/en/stable/index.html) (python)
    * [Examples](http://graphviz.readthedocs.io/en/stable/examples.html)
    * [Force-directed graph](https://bl.ocks.org/mbostock/4062045) (json/html)
* Community
  * [Data viz book club](https://blog.datawrapper.de/bookclub-tufte/)
    * [On Twitter](https://twitter.com/datavisclub)
* Various
  * [Multiple views on how to choose a visualization](https://medium.com/multiple-views-visualization-research-explained/multiple-views-on-how-to-choose-a-visualization-b3ffc99fcddc) (Franconeri, 2019)
  * [Ten simple rules for better figures](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003833) (Rougier et al., 2014)

### Datasets/databases
* Note: health-related data is in this [section](#healthcare)
* [Search engine](https://toolbox.google.com/datasetsearch)
* Compilations
  * [Data.gov](https://www.data.gov/)
  * [From Vanderbilt Biostats](http://biostat.mc.vanderbilt.edu/wiki/Main/DataSets)
  * [Kaggle](https://www.kaggle.com/datasets)
  * [Public datasets](https://github.com/awesomedata/awesome-public-datasets)
  * [Google Public Data Explorer](https://www.google.com/publicdata/directory)
  * [Datasets available via R packages](https://vincentarelbundock.github.io/Rdatasets/datasets.html)
  * Open/public datasets for machine learning
    * [List 1](https://medium.com/datadriveninvestor/the-50-best-public-datasets-for-machine-learning-d80e9f030279) (Stanford)
    * [List 2](https://blog.bigml.com/list-of-public-data-sources-fit-for-machine-learning/) (BigML)
  * Network datasets
    * [From DIMACS](http://networkrepository.com/dimacs.php)
    * [From @kateto](http://kateto.net/2016/05/network-datasets/)
    * [From @profjure](https://snap.stanford.edu/data/)
  * Time series
    * [From DataMarket](https://datamarket.com/data/list/?q=provider:tsdl)
    * [Economic](https://fred.stlouisfed.org/) (Fed Reserve)
  * [Good, small datasets](http://veekaybee.github.io/2018/07/23/small-datasets/) (Vicki Boykis)
* Specific sources
  * [Bureau of Labor Statistics](https://www.bls.gov/data/), e.g., [Consumer Price Index](https://www.bls.gov/cpi/data.htm) (inflation)
  * [US Census Bureau](https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml)
  * Pew Research Center: [data](http://www.pewresearch.org/download-datasets/) and [how to analyze](https://medium.com/pew-research-center-decoded/how-to-analyze-pew-research-center-survey-data-in-r-f326df360713)
  * [Neighborhood atlas](https://www.neighborhoodatlas.medicine.wisc.edu/) - disparities / deprivation work, [perspective about](https://www.nejm.org/doi/full/10.1056/NEJMp1802313) (paywall?)
  * [FEMA Hazus](https://www.fema.gov/hazus)
  * FiveThirtyEight
    * [List of available data](https://data.fivethirtyeight.com/), [data](https://github.com/fivethirtyeight/data), [R package](https://github.com/rudeboybert/fivethirtyeight)
  * [European statistics](http://ec.europa.eu/eurostat/data/database)
  * [IMF](http://www.imf.org/en/Data)
  * [WHO](http://www.who.int/gho/en/)
  * [Quandl](https://docs.quandl.com/docs/python) - financial / economic data - some are free
* Literature
  * [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/)
  * [Scopus](https://www.scopus.com/search/form.uri?display=basic)
  * [Web of Science](https://clarivate.com/products/web-of-science/web-science-form/web-science-core-collection/)
  * [Embase](https://www.elsevier.com/solutions/embase-biomedical-research)
  * [CENTRAL (Cochrane reviews)](http://www.cochranelibrary.com/about/central-landing-page.html)
  * [Google Scholar](https://scholar.google.com/)

### Communication/dissemination
* Sharing data ([guide](https://github.com/jtleek/datasharing) by [@jtleek](https://github.com/jtleek))
* Open-source: [How to choose license](https://choosealicense.com/)
* Manuscripts
  * How to write
    * [Your first paper](https://github.com/jtleek/firstpaper) ([@jtleek](https://github.com/jtleek), biostat)
    * [12 steps to writing](https://thehealthresearchjourney.wordpress.com/2014/12/05/the-12-steps-to-writing-a-paper-and-staying-sane/)
    * [Writing a paper](https://intra.ece.ucr.edu/~rlake/Whitesides_writing_res_paper.pdf) (Whitesides)
    * Healthcare-focused
      * [Prep for a medical journal](https://medicine.umich.edu/sites/default/files/content/downloads/Welch%20Manuscripts.pdf) (Welch, 1999 paper)
      * [Writing for Impact](https://medicine.umich.edu/sites/default/files/content/downloads/WritingResearchPaper_Ibrahim_0.pdf) (Ibrahim and Dimick)
      * [Policy papers in clinical journals](https://sph.umich.edu/cehr/pdf/Manuscript_Guide.pdf) (UM CHEAR)
      * [Picking a journal](http://jane.biosemantics.org/)
      * [Reporting guidelines](https://www.equator-network.org/reporting-guidelines/)
  * [Run a "paper sprint"](https://sph.umich.edu/cehr/pdf/Paper_Sprint_Manual.pdf)
  * Staying organized
    * [Publication planner](http://www.raulpacheco.org/2016/06/designing-and-implementing-a-publications-planner/) (Pacheco-Vega)
  * [Types of reviews](http://guides.temple.edu/c.php?g=78618&p=4156607) (Temple U) - Systematic, scoping, etc.
* [Visual abstracts](https://static1.squarespace.com/static/5854aaa044024321a353bb0d/t/5a527aa89140b76bbfb2028a/1515354827682/VisualAbstract_Primer_v4_1.pdf)
* Policy
  * [How to use research to affect policy](https://www.nature.com/articles/s41599-018-0176-7) (Oxfam)
  * [Connect research to policy](https://www.healthaffairs.org/do/10.1377/hblog20180403.254308/full/) (Quinn)
  * [More than a press release](https://theincidentaleconomist.com/wordpress/a-press-release-is-not-enough-videos/) (Frakt, Videos)
* [Working with the media](http://senseaboutscienceusa.org/media-guide-for-scientists/)
* Writing for lay outlets
  * [For "The Conversation"](https://www.slideshare.net/cczuhajewski/writing-for-the-conversation-106342981) (slides, Chang and Czuhajewski)
* Writing help
  * [Lots of resources](https://owl.purdue.edu/owl/purdue_owl.html) (Purdue)
* Reference software
  * [Zotero](https://www.zotero.org/)
  * [Mendeley](https://www.mendeley.com/)
  * [EndNote](http://endnote.com/)
* LaTeX
  * [Getting started](https://nilesjohnson.net/latex.html) (Johnson, [Code](https://gitlab.com/nilesjohnson/latex_starter))
  * [Overview](https://www.maths.tcd.ie/~dwilkins/LaTeXPrimer/) (Wilkins)
  * Collaboration
    * [ShareLaTeX](https://www.sharelatex.com/)
  * Templates
    * [Example for journals](https://www.leandro-coelho.com/default-latex-article-style-modifications/) (Coelho)
    * Thesis templates:
      * [From U Wolverhamptom](https://github.com/snim2/phdtemplate)
      * [From Michigan](http://clasp.engin.umich.edu/pages/current/dissertation-template)
  * Beamer tips and tricks ([slides](https://github.com/paulgp/beamer-tips/blob/master/slides.pdf), [source code](https://github.com/paulgp/beamer-tips), from [@paulgp](https://github.com/paulgp))
  * Graphics
    * [Tikz and PGF](http://www.texample.net/tikz/)
  * Indicating math mode
    * [Using /( /) vs $](https://tex.stackexchange.com/questions/510/are-and-preferable-to-dollar-signs-for-math-mode)
* Writing a book
  * [Self-publishing](https://medium.com/@jeremyjkun/on-self-publishing-a-programmers-introduction-to-mathematics-1472b7511c99?curator=MediaREDEF) (Kun)

### Healthcare
* Guides
  * [Healthcare Industry](https://kresgeguides.bus.umich.edu/healthcarebiotechhome) (largely UM students only)
  * [Health management and policy](http://guides.lib.umich.edu/hmp)
  * Finding health statistics
    * [From UM](http://guides.lib.umich.edu/healthstats)
    * [From Wisconsin-Madison](http://researchguides.ebling.library.wisc.edu/c.php?g=293234)
* Datasets / databases
  * Medicare Part B
    * [National summary files](https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Part-B-National-Summary-Data-File/Overview.html)
    * [Carrier summary files](https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Part-B-Carrier-Summary-Data-File/Overview.html)
    * Not free: [CCW](https://www.ccwdata.org/web/guest/home)
  * CDC: [data/stats](https://www.cdc.gov/DataStatistics/)
    * [Chronic disease datasets](https://chronicdata.cdc.gov/)
      * E.g., [Maternal and child health](https://chronicdata.cdc.gov/browse?category=Maternal+%26+Child+Health)
  * Critical care database: [MIMIC](https://mimic.physionet.org/)
  * Other
    * [Clinicaltrials.gov](https://clinicaltrials.gov/)
    * [Tufts Cost-Effectiveness Analysis Registry](http://healtheconomics.tuftsmedicalcenter.org/cear4/Home.aspx)
    * [Book recommendations from SHS](https://www.iise.org/SHS/details.aspx?id=18334)
  * Major surveys
    * [NHANES](https://www.cdc.gov/nchs/nhanes/index.htm) (in person)
    * [BRFSS](https://www.cdc.gov/brfss/annual_data/annual_data.htm) (phone, pronounced "Burfiss")
* Methods
  * Forums
    * [datamethods](https://discourse.datamethods.org/) - health-related stats forum
    * [MedStats](https://groups.google.com/forum/#!forum/medstats) - google group
  * [Pharmacy concentration calcs](https://pharmafactz.com/pharmaceutical-calculations-concentrations/)
* Newsletters
  * CDC's [Morbidity and Mortality Weekly Report](https://www.cdc.gov/mmwr/index.html)

### Jobs/Summer schools
* Jobs
  * Compilations
    * [Companies that hire operations researchers](https://github.com/dirkschumacher/or-companies/); from [@dirkschumacher](https://github.com/dirkschumacher)
    * [United Nations (UN) jobs](https://unjobhunt.com/) from from [@dirkschumacher](https://github.com/dirkschumacher)
    * [Humanitarian logistics orgs](https://chhs.gatech.edu/resources/links?qt-quicktab_logistics_links=4#qt-quicktab_logistics_links) (GT CHHS)
    * [Math-related](https://orfe.princeton.edu/graduate/jobs) (ORFE Princeton)
  * Listservs
    * [Inside Higher Ed](https://careers.insidehighered.com/)
    * [Infectious disease dynamics listserv](http://iddjobs.org/jobs/)
    * Twitter feeds with job postings
      * [R job listings](https://twitter.com/rjoblistings)
      * [Data science](https://twitter.com/NewDataSciJobs)
  * National labs
    * Sandia: [fellowships/postdocs](http://www.sandia.gov/careers/students_postdocs)
    * National Renewable Energy Lab [NREL](https://www.nrel.gov/careers/)
      * [Director's Postdoc Fellowship](https://www.nrel.gov/careers/directors-fellowship.html?mc_cid=6e3282f94d&mc_eid=079dfe7593)
    * Oak Ridge
      * [Postdocs](https://www.ornl.gov/content/ornl-s-postdoctoral-program)
      * [Weinberg Fellowship](https://www.ornl.gov/careers/alvin-m-weinberg-fellowship)
      * [Householder Fellowship](https://www.ornl.gov/careers/alston-s-householder-fellowship)
  * [Pathways to Science](https://pathwaystoscience.org/index.aspx) - internships, jobs, etc.
  * [How to build your portfolio](https://mpi4py.readthedocs.io/en/stable/index.html) (Harris)
  * What can you do with a math degree? [Videos](https://www.maa.org/programs/faculty-and-departments/pic-math/solving-real-world-problems) - PICMATH
  * Schools
    * [Summer schools 2019](https://thiagoserra.com/2019/01/15/summer-2019-schools-on-data-analytics-discrete-math-machine-learning-networks-optimization-and-other-relevant-topics-in-operations-research/) (Thiago Serra)
  * Undergrads
    * [MSRI-UP](http://www.msri.org/web/msri/education/for-undergraduates/msri-up) - summer math program for undergrads
    * [Job search resources](https://bigmathnetwork.org/resources-for-students/) - BIG Math
* Career prep
  * [Questions to think through career goals](https://github.com/BenLangmead/langmead-lab/blob/master/postdoc_questionnaire.md) from [@benlangmead](https://github.com/benlangmead)
    * [Slightly expanded](https://github.com/jtleek/careerplanning) from [@jtleek](https://github.com/jtleek)
* Academic job search
  * [OperationsAcademia.org](http://www.operationsacademia.org/) - OR/MS job postings and advice
  * University compilations
    * [Univ. of Michigan](http://crlt.umich.edu/PFF_Resources); [Berkeley](https://career.berkeley.edu/PhDs/PhDAcademic); [UPenn](https://www.vpul.upenn.edu/careerservices/writtenmaterials/); [Duke](https://studentaffairs.duke.edu/career/guides/academic-career-preparation)
  * [Materials checklist](https://career.ucsf.edu/sites/career.ucsf.edu/files/UCSF%20OCPD%20Checklist%20Faculty%20Materials.pdf) (UCSF)
  * Research statement
    * How to write
      * [Jim Austin](https://www.sciencemag.org/careers/2014/04/writing-research-plan); [Karen Kelsky](http://theprofessorisin.com/2016/09/16/dr-karens-rules-of-the-research-statement/); [UPenn](https://www.vpul.upenn.edu/careerservices/writtenmaterials/researchstatements.php); [U. Wash](https://uw.uconnectlabs.com/wp-content/uploads/sites/25/2016/06/Research-Statements.pdf); [GSA](https://serc.carleton.edu/NAGTWorkshops/careerprep/jobsearch/research_statement.html) (Geology); [Duke](https://studentaffairs.duke.edu/career/graduate-students/academic-career-preparation/research-statement); [Med College of Wisc](https://www.mcw.edu/-/media/MCW/Education/Graduate-School/Documents/ucla_researchstatementtemplate_46-47.pdf); [Cornell](https://gradschool.cornell.edu/academic-progress/pathways-to-success/prepare-for-your-career/take-action/research-statement/)
    * Samples
      * [UCSF](https://career.ucsf.edu/grad-students-postdocs/career-planning/academic-jobs/applying/academic-samples); [UPenn](https://www.vpul.upenn.edu/careerservices/writtenmaterials/teachingresearchsamples.php)
  * Teaching statement
    * [Univ. of Michigan](http://crlt.umich.edu/category/tstrategies/tstpts), [UPenn](https://www.vpul.upenn.edu/careerservices/writtenmaterials/teachingresearchsamples.php)
      * [Guidelines for teaching at MIT](https://tll.mit.edu/guidelines/guidelines-teaching-mit-and-beyond)
  * Diversity statement
    * [Univ. of Michigan](http://www.crlt.umich.edu/sites/default/files/resource_files/DiversityStatementHandout.pdf); [UCSD](http://facultydiversity.ucsd.edu/recruitment/contributions-to-diversity.html); [UNL](https://www.unl.edu/gradstudies/connections/writing-diversity-statement); [Vanderbilt](https://cft.vanderbilt.edu/guides-sub-pages/developing-and-writing-a-diversity-statement/); [Cincinnati](https://www.uc.edu/content/dam/uc/aess/docs/AWC/graduatehandouts/Diversity%20Statement%20(Accessible)%20%20.pdf)
  * Job talk
    * [Article - giving an excellent talk](https://chroniclevitae.com/news/2242-how-to-give-an-excellent-stem-job-talk?cid=VTEVPMSED1) (Carpenter, Waters)
    * [Article - Tips for a Successful Job Talk](https://www.insidehighered.com/advice/2018/01/10/advice-giving-effective-job-presentation-opinion) (Aguilar)
    * [Slides - How to Give a Seminar](https://www.eeassoc.org/doc/upload/Ten_Commandments_JM_Presentation_KS20190116211403.pdf) (Storesletten, econ)
    * [Slides - How to present your job market paper](https://www.eeassoc.org/doc/upload/HowToPresent_LaFerrara20190116211520.pdf) (La Ferrara, econ)
  * Interviews
    * [Commonly asked questions](https://www.vitae.ac.uk/researcher-careers/pursuing-an-academic-career/applying-for-academic-jobs/commonly-asked-questions-in-academic-interviews) (Vitae)
  * Videos
    * [Duke postdoc services](https://www.youtube.com/user/DukePostdocServices)
  * Articles
    * [The hiring process from the other side](https://career.berkeley.edu/PhDs/PhDhiring) (Berkeley)
  * Example materials
    * [From Philip Guo](http://www.pgbovine.net/faculty-job-application-materials.htm)
  * Advice
    * [Navigating the OR/MS academic job process](https://pubsonline.informs.org/do/10.1287/orms.2019.01.09/full/) (Dutta, Çağlayan)


### Twitter
* Communities I appreciate
  * [#orms](https://twitter.com/hashtag/orms?src=hash)
  * [#rstats](https://twitter.com/hashtag/rstats?src=hash)
  * [#phdchat](https://twitter.com/hashtag/phdchat?src=hash)
  * [#AcWri](https://twitter.com/hashtag/acwri?src=hash)
  * [#scicomm](https://twitter.com/hashtag/scicomm?src=hash)
* Hashtags that have included interesting discussions at some point
  * [#hiddencurriculum](https://twitter.com/hashtag/hiddencurriculum?src=hash)
  * [#phdtips](https://twitter.com/hashtag/phdtips?src=hash)
  * [#scrawledgrantadvice](https://twitter.com/hashtag/scrawledgrantadvice?src=hash)
* Other
  * [CV without Twitter](http://aurielfournier.github.io/cv-without-twitter/) (Auriel Fournier)

### Funding
* Compilations
  * [For early career researchers](https://research.jhu.edu/rdt/funding-opportunities/early-career/) (JHU)
  * [From _Science_](http://www.sciencemag.org/careers/where-search-funding)
  * [From USC](https://research.usc.edu/for-investigators/funding/federal/)
* [Federal grants](https://www.grants.gov/)
  * [Forecasted and posted](https://www.grants.gov/search-grants.html?agencyCode%3DHHS)
* CAREER Grants
  * [Materials](http://cisecareerworkshop.web.unc.edu/materials/) from CISE workshop, Mar 2019
* Specific
  * FDA - [Generic drug-related](https://www.fda.gov/drugs/generic-drugs/generic-drugs-collaboration-opportunities)
  * CDC - [HIV](https://www.cdc.gov/hiv/funding/index.html)
  * [Public Health Emergency](http://www.phe.gov/Preparedness/planning/hpp/Pages/funding.aspx)
* Grant proposals
  * [Open grants](https://www.ogrants.org/) - sample grant proposals

### Teaching
* [Guidebook](http://www.crlt.umich.edu/gsis/gsi_guide) (UM CRLT)
* Free textbook: [_Teaching Engineering_](https://engineering.purdue.edu/ChE/aboutus/publications/teaching_eng) (Wankat and Oreovicz)
* Blogposts
  * [Diversity and inclusion in the classroom](https://punkrockor.com/2016/04/21/what-i-do-for-diversity-and-inclusion-in-the-classroom/) (Laura Albert)
  * [Teaching math](https://momentssnippetsspirals.wordpress.com/2015/04/07/where-direct-instruction-fails-willingham-memorization-and-conceptual-understanding-2/) (K-12, Milos)
* Specifics
  * First day
    * [UNL](https://www.unl.edu/gtahandbook/first-day-class); [Lang](https://www.chronicle.com/interactives/advice-firstday)
  * [First 3 weeks](https://www.unl.edu/gradstudies/current/teaching/first-3-weeks) (UNL)
  * [Lesson planning](http://crlt.umich.edu/strategies-effective-lesson-planning) (UMich)
  * [Logistics of large classes - 10 articles](http://pgbovine.net/teaching-large-courses.htm) (Guo)
  * [Improving inclusion](https://www.chronicle.com/interactives/20190719_inclusive_teaching?cid=cp234) (Sathy and Hogan)
  * [Be more engaging](https://www.chronicle.com/interactives/advice-teaching?cid=cp234) (Cavanagh)

### Blogs I like (and read occasionally)
* Operations research-ish
    * [Punk Rock OR](https://punkrockor.com/) by [@lauraalbertphd](https://twitter.com/lauraalbertphd)
    * [OR in an OB World](https://orinanobworld.blogspot.com/) by [@prubin73](https://github.com/prubin73)
    * [Yet Another Math Programming Consultant](http://yetanothermathprogrammingconsultant.blogspot.com/) (Kalvelagen)
    * [Geraint Palmer's blog](http://www.geraintianpalmer.org.uk/blog/)
    * [Thiago Serra's blog](https://thiagoserra.com/blog/)
    * [Reckoning Risk](http://reckoningrisk.com/) by [@TomMLogan](https://github.com/tommlogan) and [@t-g-williams](https://github.com/t-g-williams)
* Other
    * [Math3Ma](http://www.math3ma.com/) by [@math3ma](https://twitter.com/math3ma) (math)
    * [Math Intersect Programming](https://jeremykun.com/) (Kun)
    * [Philip J. Guo's site](http://pgbovine.net/writings.htm)
    * [Azimuth](https://johncarlosbaez.wordpress.com/) (various STEM fields trying to save the planet, [index of entries](http://www.azimuthproject.org/azimuth/show/Azimuth+Blog))
    * [Armchair Ecology](https://armchairecology.blog/) (Poisot, computational biology)
* Humor
    * [Math with Bad Drawings](https://mathwithbaddrawings.com/)
    * [Lego Grad Student](https://brickademics.com/)
    * [PhD Comics](http://phdcomics.com/comics/most_popular.php)

### Various advice
* Grad students
  * [Picking a PhD advisor](https://www.sciencemag.org/careers/2019/04/what-matters-phd-adviser-here-s-what-research-says) (Langin, Science)
  * [For new grad students](https://medium.com/@dorsaamir/modest-advice-for-new-graduate-students-b0be6b8dbc22) (Dorsa Amir)
  * [Guide to grad school](http://marcua.net/writing/gradschool-guide/) (Adam Marcus, CS)
  * [Guidebook for succeeding in the PhD](https://static1.squarespace.com/static/55c143d9e4b0cb07521c6d17/t/5b4f409f575d1ff83c2f12d8/1531920545061/PhDGuidebook.pdf) (Alex Eble, econ, [another link](http://www.alexeble.com/advice/))
  * [Succeeding in the PhD](http://www.cs.jhu.edu/~mdredze/publications/HowtoBeaSuccessfulPhDStudent.pdf) (Dredze, Wallach; computer science)
  * [One year to dissertation](https://livefreeordichotomize.com/2018/09/14/one-year-to-dissertate/) (McGowan, [files](https://github.com/LucyMcGowan/dissertation-toolkit))
  * [Advisor/PhD student dynamics](https://chroniclevitae.com/news/1793-handling-your-imperfect-adviser) (Nelson)
  * [For female grad students](https://docs.google.com/document/d/1DMoSXf7pGRLMN1VP5-36nu2mkNBFEsJtERCi-AERwKk/edit) (political science, compiled by [@dianazobrien](https://twitter.com/dianazobrien))
  * [Attending big conferences](https://kieranhealy.org/blog/archives/2003/08/27/conference-advice/) (Kieran Healy, sociology)
  * [10 tips to win at grad school](https://chroniclevitae.com/news/2158-10-tips-to-help-you-win-at-graduate-school?cid=VTEVPMSED1) (Toor)
  * Compilations
    * [The Professor Is In](http://theprofessorisin.com/) (Karen Kelsky) - blog with various academic advice
    * [Many resources](http://www.raulpacheco.org/resources/) (Pacheco-Vega, polisci/georgraphy)
    * [Doing research](https://webpages.uncc.edu/sakella/advice.html) (Arinivas Akella, CS)
    * [Grad school, technical writing, etc.](http://cseweb.ucsd.edu/~mihir/education.html) (Mihir Bellare, CS)
* Undergrads
  * [Undergrad in the Lab Blog](http://undergradinthelab.com/)
  * [Lots of advice](https://pathwaystoscience.org/Library.aspx) (Pathways to Science)
  * [Applying to grad school](https://kcklett.wixsite.com/phduo) (Klett & Lee)
* New faculty
  * [Compliation](https://tomprof.stanford.edu/) (Stanford)
  * [Compilation](https://github.com/crazyhottommy/The-world-of-faculty) (Tang)
  * [The 7 Year Postdoc](https://blogs.scientificamerican.com/guest-blog/the-awesomest-7-year-postdoc-or-how-i-learned-to-stop-worrying-and-love-the-tenure-track-faculty-life/) (Nagpal)
    * [Counter thoughts](http://mathbionerd.blogspot.com/2017/07/not-awesomest-7-year-postdoc.html)
  * [Getting started](https://chroniclevitae.com/news/2225-how-to-start-off-right-in-your-new-job?cid=VTEVPMSED1) (Whitaker)
  * [If the 3rd year review goes poorly](https://www.chronicle.com/article/Operation-Keep-My-Job-/235535) (Albertson)
  * [Staying sane on the tenure track](https://people.orie.cornell.edu/shane/pubs/StayingSane.pdf) (Henderson)
  * [Faculty Mentoring Handbook](http://live-uarizona-diversity.pantheon.arizona.edu/sites/default/files/mentoring_handbook.pdf) (Arizona)
  * Running a lab
    * [Ten simple rules towards healthier research labs](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006914) (Maestre, 2019)
    * [_Making the Right Moves: A Practical Guide to Scientific Management_](https://www.hhmi.org/science-education/programs/making-right-moves) (HHMI) - free book about managing a lab
  * Working with research assistants
    * [Guidelines](https://www.tgs.northwestern.edu/academics/academic-student-services/assistantship-best-practices/research-assistants.html) (Northwestern)
    * [Hire and manage](https://duckofminerva.com/2015/03/how-to-hire-and-work-effectively-with-a-research-assistant.html) (MacKenzie)
  * Mentoring
    * [Compliation](https://www.aeaweb.org/about-aea/committees/cswep/newsletters/topics#mentoring) (AEA, econ)
* Job search
  * [Academic search](http://publish.illinois.edu/engr-mavis/files/2014/09/Academic-Job-Search-2016.pdf) (Nagi)
  * [Data science jobs](http://hookedondata.org/Advice-for-Applying-to-Data-Science-Jobs/) by [@robinsones](https://github.com/robinsones)
  * [Vitae](https://chroniclevitae.com/) - database, advice, etc.
  * [Job market mistakes](https://www.chronicle.com/article/5-Big-Picture-Mistakes-New/243475) (humanities)
* Various
  * [8 tips for saying no](http://www.antonpottegaard.dk/download/HowToSayNo.pdf) by [@APottegard](https://twitter.com/APottegard)
  * [The Pac-Man rule](http://ericholscher.com/blog/2017/aug/2/pacman-rule-conferences/) (Holscher) - always leave room for someone to join the group
  * [Econ prof's work style](http://people.ischool.berkeley.edu/~hal/Papers/how.pdf) (Hal Varian)
  * [Chris Blattman's blog](https://chrisblattman.com/) (econ prof, links on right-hand side)
  * [When your data science project doesn't work](https://medium.com/@skyetetra/so-your-data-science-project-isnt-working-7bf57e3f12f1)
  * [Blogs for female consultants/bus. travelers](https://corporette.com/resources-and-blogs-for-female-consultants/)
  * [Business clothes for women](https://twitter.com/arieldora/status/1072138548269195264) (Stern)
  * [Imposter syndrome resources](http://aurielfournier.github.io/imposter-syndrome/) (Fournier)
  * [The importance of stupidity in scientific research](https://jcs.biologists.org/content/121/11/1771) (Schwartz, 2008)
* Skills
  * Reading papers
    * [Reading papers](https://github.com/jtleek/readingpapers) by [@jtleek](https://github.com/jtleek)
    * [Technical papers](https://destenienock5.wixsite.com/destenienock/blog-posts/how-to-read-and-summarize-a-technical-paper) (Nock)
  * [Writing lit reviews](http://www.raulpacheco.org/resources/literature-reviews/) (Raul Pacheco-Vega)
  * [Organizing data in a spreadsheet](https://www.tandfonline.com/doi/full/10.1080/00031305.2017.1375989) (Broman and Woo, open access); not always the best idea, but some tips
    * Reviewing papers
      * [How to review a paper](https://github.com/jtleek/reviews) (Leek - biostat)
      * [Being a good reviewer](https://academic.oup.com/ajhp/article/74/24/2080/5102692) (DiDomenico et al., pharmacy)
  * [Writing production-level code](https://www.datascience.com/blog/production-level-code-for-data-science) (Pappakrishnan)
  * [How to report bugs effectively](https://www.chiark.greenend.org.uk/~sgtatham/bugs.html) (Simon Tatham) - perhaps send to your users
  * Debugging
    * [Infeasible models](http://yetanothermathprogrammingconsultant.blogspot.com/2018/08/the-best-way-to-debug-infeasible-models.html) (Kalvelagen)
    * [Rubber ducky method](https://rubberduckdebugging.com/) - explain in detail to an inanimate object
    * [Wolf-fence algorithm](http://coreygoldberg.blogspot.com/2008/12/wolf-fence-debugging.html) - basically binary search with fun description ([original paper](https://dl.acm.org/citation.cfm?id=358695), paywall)

### Eclectic
* CV of failures
  * [Johannes Haushofer](https://www.princeton.edu/~joha/Johannes_Haushofer_CV_of_Failures.pdf)
  * [WaPo article](https://www.washingtonpost.com/news/wonk/wp/2016/04/28/it-feels-really-good-to-read-about-this-princeton-professors-failures/)
* Grad school's ["hidden curriculum"](https://scatter.wordpress.com/2018/07/24/guest-post-grad-schools-hidden-curriculum/) (Calarco)
* Diversity
  * [Compilation of articles](https://www.astrobetter.com/wiki/Diversity) (AstroBetter - Equal Opportunity Astronomy)
* Pay your undergrad researchers
  * [Paper about field techs](https://github.com/aurielfournier/aurielfournier.github.io/blob/master/_pdfs/Fournier%2C%20Bond%20-%202015%20-%20Wildlife%20Society%20Bulletin.pdf) (Fournier, Bond)
  * [Other blog posts cited within](https://labandfield.wordpress.com/2016/03/09/volunteer-field-techs-are-bad-for-wildlife-ecology-the-response/)
* Meta - [list of "awesome" lists](https://github.com/sindresorhus/awesome)
* [Azimuth Project](http://www.azimuthproject.org/azimuth/show/HomePage)
  * Collaboration of scientists and engineers who want to save the planet
* Guide to Bad Data
  * [Github](https://github.com/Quartz/bad-data-guide)
  * [Article on Quartz](https://qz.com/572338/the-quartz-guide-to-bad-data/#user-content-there-are-inexplicable-outliers)
* [Technical / scientific debt](http://varianceexplained.org/r/scientific-debt/) from [@dgrtwo](https://github.com/dgrtwo)
* [Types of validity](http://www.amybucherphd.com/statistical-validity-types/) (Amy Bucher)
* [Testing](https://towardsdatascience.com/testing-to-learn-part-1-16a7968d2ba3) (Kehrer)
* Various software
  * [Digitize it](https://www.digitizeit.de/) - Convert figure to (x,y) data
  * [draftable](https://draftable.com/compare) - Compare pdf files
  * [color oracle](http://colororacle.org/) - convert screen to what a color blind person would see:
  * Poll meeting availability
    * [When2Meet](https://www.when2meet.com/)
    * [When is good](http://whenisgood.net/)
* Word
  * [How to change the Normal template](https://support.office.com/en-us/article/change-the-normal-template-normal-dotm-06de294b-d216-47f6-ab77-ccb5166f98ea)
* Fun OR (or related) applications
  * [2048 using MDPs](http://jdlm.info/articles/2018/03/18/markov-decision-process-2048.html) from [@jdleesmiller](https://github.com/jdleesmiller)
  * [Chutes & Ladders as a Markov chain](https://jakevdp.github.io/blog/2017/12/18/simulating-chutes-and-ladders/) [@jakevdp](https://github.com/jakevdp)
  * [Mario Kart drivers - Pareto efficiency](http://hinnefe2.github.io/python/tools/2015/09/21/mario-kart.html) from [@hinnefe2](https://github.com/hinnefe2)
  * [Text mining on country music lyrics](https://www.johnwmillr.com/trucks-and-beer/) (Miller)
* OR/Programming/etc. in Industry
  * [Netflix](https://medium.com/netflix-techblog/notebook-innovation-591ee3221233)
* Examples
  * [Queueing](https://kottke.org/19/01/its-time-for-some-queueing-theory) (Kottke)
* Algorithms
  * [15 important algorithms](https://interestingengineering.com/15-of-the-most-important-algorithms-that-helped-define-mathematics-computing-and-physics) (McFadden)
  * [100 days of algorithms](https://medium.com/100-days-of-algorithms) (Bouda), [code](https://github.com/coells/100days)
* [Beer game using AI](https://beergame.opexanalytics.com/#/)
* Websites
  * (Free) [Hosted by github](https://pages.github.com/)
    * [Tutorial](https://marisacarlos.com/pages/create-simple-academic-website) (Carlos)
    * [Themes](https://github.com/topics/jekyll-theme)
      * [Simple one for academics](https://github.com/academicpages/academicpages.github.io)
      * [Template for labs](http://www.allanlab.org/aboutwebsite.html)
  * (Free/Paid) [Wix](https://www.wix.com)
  * (Free) [Google Sites](https://sites.google.com/)
* [Icons](https://www.iconsdb.com/) - e.g., the Google Scholar logo
* [Download GoogleMaps to use offline](https://support.google.com/maps/answer/6291838)
* [Math genealogy project](https://genealogy.math.ndsu.nodak.edu/index.php)
* User interfaces
  * [Explaining UX to kindergartners](https://www.linkedin.com/pulse/explaining-ux-kindergartners-plus-few-lessons-those-who-teena-singh) (Singh)
  * [Terrible elevator control panels](https://www2.isye.gatech.edu/people/faculty/John_Bartholdi/misc/elevators/elevators.html) (Bartholdi)
* Source code for Apollo 11: [code](https://github.com/chrislgarry/Apollo-11)
* Humor
  * [Top 10 Illegitimate Proof Techniques](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/lecture-3-strong-induction/MIT6_042JF10_proof.pdf) (I think the original version of this list came from Dana Angluin)
  * ["The best way to write secure and reliable applications"](https://github.com/kelseyhightower/nocode)
  * [Add coffee stains to your LaTeX files](http://hanno-rein.de/archives/349) (Rein)
  * [Guide to interpreting faculty feedback](https://kieranhealy.org/blog/archives/2013/08/16/academic-feedback/)
  * [Spurious correlations](http://www.tylervigen.com/spurious-correlations) (Vigen)
    * [Make your own](http://tylervigen.com/discover)
  * [Create parody O'Reilly book covers](https://dev.to/rly)
  * [Improbable research](https://www.improbable.com/)
  * [Computer science research topic generator](https://www.cs.purdue.edu/homes/dec/essay.topic.generator.html)
  * [Gettysburg address via powerpoint](http://norvig.com/Gettysburg/index.htm) (Norvig)

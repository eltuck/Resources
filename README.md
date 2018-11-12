# Resources
Consider this a public bookmark bar. These are resources I've found useful or think might be one day. I've listed the full urls to external sites so you can see what you're clicking on (e.g., is it a pdf?).

Disclaimers: still in progress, definitely not comprehensive, links may not work, and in no particular order.

I welcome any additions, suggestions, or corrections! Feel free to create a pull request or send me an [email](mailto:eltuck@umich.edu).

I've found a good portion of this from links other folks have shared on  [Twitter](https://twitter.com/emilyltucker). Thanks, y'all. Also a very big thank you to everyone who created the original content.

## Table of Contents
* [Python](#python)
* [R](#r)
* [GitHub](#github)
* [General coding and computation](#general-coding--computation)
* [AMPL](#ampl)
* [Other programming languages](#other-programming-languages)
* [Math programming software](#math-programming-software)
* [Math programming resources](#math-programming-resources)
* [Operations research-adjacent material](#operations-research-adjacent-material)
* [Data visualization](#data-visualization)
* [Datasets and databases](#datasetsdatabases)
* [Communication and dissemination](#communicationdissemination)
* [Healthcare](#healthcare)
* [Jobs and summer schools](#jobssummer-schools)
* [Funding](#funding)
* [Teaching](#teaching)
* [Blogs I like (and read occasionally)](#blogs-i-like-and-read-occasionally)
* [Various advice](#various-advice)
* [Eclectic](#eclectic)

### Python
* Overview
  * Whirlwind tour from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/WhirlwindTourOfPython
  * Overview from [@drvinceknight](https://github.com/drvinceknight): https://vknight.org/Introduction_to_OOP/OverviewOfPython/
    * Python for Mathematicians: https://github.com/drvinceknight/Python-Mathematics-Handbook
  * Scipy lecture notes: http://www.scipy-lectures.org/
    * Getting started: https://www.scipy-lectures.org/intro/index.html
* Free Textbooks
  * _Think Python_ by [@AllenDowney](https://github.com/AllenDowney) http://greenteapress.com/wp/think-python-2e/
    * Beginners guide, programming exp. not necessary
  * _Python Data Science Handbook_ by [@jakevdp](https://github.com/jakevdp) https://jakevdp.github.io/PythonDataScienceHandbook/
  * _Intro to Machine Learning in Python_ by [@amueller](https://github.com/amueller) https://github.com/amueller/introduction_to_ml_with_python
  * _Modeling and Simulation in Python_ by [@AllenDowney](https://github.com/AllenDowney): http://greenteapress.com/wp/modsimpy/
   * Targeted towards intro undergrads
* Community
  * Slack channel to learn data science in Python: https://py4ds.slack.com
* Overall tutorial
  * Python Software Foundation: https://docs.python.org/3.6/tutorial/index.html
* Topics/packages
  * Pandas (data processing)
    * Beginner tutorial from [@gjreda](https://github.com/gjreda) http://gregreda.com/2013/10/26/intro-to-pandas-data-structures/
    * Intermediate tutorial from [@tomaugspurger](https://github.com/tomaugspurger) http://tomaugspurger.github.io/modern-1-intro
  * Networks
    * NetworkX
      * https://github.com/networkx/networkx
      * Tutorial: network analysis (humanities data) https://programminghistorian.org/lessons/exploring-and-analyzing-network-data-with-python
      * Tutorial: Chinese postman problem https://www.datacamp.com/community/tutorials/networkx-python-graph-tutorial
      * Network simplex https://networkx.github.io/documentation/networkx-1.9.1/reference/generated/networkx.algorithms.flow.network_simplex.html
    * SNAP: https://snap.stanford.edu/snappy/index.html
      * Analysis of graphs and networks
      * Claims often faster and able to solve larger problems than NetworkX
  * Simulation
    * Discrete-event
      * SimPy https://simpy.readthedocs.io/en/latest/
        * Google group: https://groups.google.com/forum/#!forum/python-simpy
        * Book chapter by Barry Nelson: http://users.iems.northwestern.edu/~nelsonb/IEMS435/PythonSim.pdf
      * Ciw: http://ciw.readthedocs.io/en/latest/
        * For open queueing networks
    * Agent-based modeling
      * Mesa: https://github.com/projectmesa/mesa
        * General purpose
        * Tutorial: https://github.com/projectmesa/mesa
      * ABCE: https://abce.readthedocs.io/en/0.9.3b2/
        * Tailored towards economic modeling
  * List of OR/MS-related packages: https://wiki.python.org/moin/PythonForOperationsResearch
  * Optimization
    * Overview (Ted Ralphs): https://coral.ie.lehigh.edu/~ted/files/modeling/lectures/ModelingWithPython.pdf
    * Modeling languages
      * gurobipy: https://www.gurobi.com/documentation/8.0/quickstart_windows/py_python_interface
        * Walk-through of building simple model: https://www.gurobi.com/documentation/8.0/quickstart_windows/py_simple_python_example.html
        * Walk-through of semi-complex model: https://www.gurobi.com/documentation/8.0/quickstart_windows/py_python_dictionary_examp.html
        * Examples
          * Walkthrough: https://www.gurobi.com/documentation/8.0/examples/example_tour.html
          * List: https://www.gurobi.com/documentation/8.0/examples/python_examples.html
      * PuLP (linear programs): https://projects.coin-or.org/PuLP
      * Pyomo: http://www.pyomo.org/
        * How to run models: https://groups.google.com/forum/#!topic/pyomo-forum/NWU1LW6GWL8
        * Example models: http://nbviewer.jupyter.org/github/Pyomo/PyomoGallery/tree/master/
      * Pysp: https://pypi.org/project/coopr.pysp/
        * Extends Pyomo for stochastic programming
    * Solvers / algos
      * scipy.optimize: https://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html
      * CVXPY (convex opt): http://www.cvxpy.org/
        * Short-course: http://www.cvxpy.org/short_course/index.html
      * Optimist (SDDP in water systems): https://scholarsarchive.byu.edu/cgi/viewcontent.cgi?article=1330&context=iemssconference
      * StochOPy (stochastic opt): https://github.com/keurfonluu/StochOPy
      * StOpt: https://gitlab.com/stochastic-control/StOpt
        * Written in C++, python bindings
      * py-lapsolver: https://github.com/cheind/py-lapsolver
        * Solver for fast linear assignment problems
      * munkres (aka Hungarian algo): http://software.clapper.org/munkres/
    * Plot convex hull: https://docs.scipy.org/doc/scipy-0.19.0/reference/generated/scipy.spatial.ConvexHull.html
  * Dimensionality reduction
    * umap: https://github.com/lmcinnes/umap
  * Game theory [(source)](http://nashpy.readthedocs.io/en/stable/discussion/other-python-game-theory-libraries.html)
    * Gambit: http://www.gambit-project.org/
    * Nashpy (compute equilibria for 2-player games): http://nashpy.readthedocs.io/en/stable/
      * Paper: http://joss.theoj.org/papers/10.21105/joss.00904
    * Axelrod (Iterated prisoner's dilemma): http://axelrod.readthedocs.io/en/stable/
    * PyNFG (Network form games): https://pythonhosted.org/PyNFG/
    * lrslib: http://cgm.cs.mcgill.ca/~avis/C/lrs.html
      * Library: lrsnash can be used to compute Nash equilibria
    * SageMath: http://doc.sagemath.org/html/en/reference/game_theory/index.html
      * Games: cooperative with finite players; matching; normal form with N players
  * Machine learning
      * Flowchart: choosing the right estimator: http://scikit-learn.org/stable/tutorial/machine_learning_map/
      * Sklearn tutorial from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/sklearn_tutorial
  * Supply chain
    * Supplychainpy: https://github.com/KevinFasusi/supplychainpy
  * Webscraping
    * (Rishav Agarwal) https://towardsdatascience.com/byod-build-your-own-dataset-for-free-67133840dc85
  * Convert PDF to html
    * PDFMiner: https://github.com/euske/pdfminer
    * Then can be used to parse
  * Other fields (that seem related)
    * CobraPy: https://opencobra.github.io/cobrapy/
      * Biological network modeling - constraints/optimization
    * Optimize process simulators: https://github.com/CAChemE/stochastic-optimization
      * Set of examples, chemical engineering
  * Visualization / figures
    * Python Graph Gallery: https://python-graph-gallery.com/
      * Lots of examples with code
    * Overview of plotting for exploratory analysis (Hopper): http://pythonplot.com/
    * Seaborn
      * Examples: https://jakevdp.github.io/PythonDataScienceHandbook/04.14-visualization-with-seaborn.html
    * Altair
      * Notebooks with example code: https://github.com/altair-viz/altair_notebooks
      * Video tutorial from [@jakevdp](https://github.com/jakevdp) https://www.youtube.com/watch?v=ms29ZPUKxbU&t=2431s
        * First ~40 min are a nice walkthrough; didn't watch the rest
    * R-style graphing
      * plotnine package: https://plotnine.readthedocs.io/en/stable/
      * ggplot package: https://www.r-bloggers.com/ggplot2-style-plotting-in-python/
    * Funny
      * XKCD-style figures: https://matplotlib.org/xkcd/examples/showcase/xkcd.html
* Notebooks
  * nbdime: https://github.com/jupyter/nbdime
    * Helpful for version control with notebooks
  * Videos on reproducible data analysis in notebooks (Jake VanderPlas): https://jakevdp.github.io/blog/2017/03/03/reproducible-data-analysis-in-jupyter/
  * Slides: "I don't like notebooks" (Joel Grus) https://docs.google.com/presentation/d/1n2RlMdmv1p25Xy5thJUhkKGvjtV-dkAIsUXP-AL4ffI/edit#slide=id.g362da58057_0_1
* How to...
  * Add Python to PATH: https://medium.com/@GalarnykMichael/install-python-on-windows-anaconda-c63c7c3d1444
  * Write unit tests (SciPy): https://github.com/numpy/numpy/blob/master/doc/TESTS.rst.txt
    * FIRST principle: https://pragprog.com/magazines/2012-01/unit-tests-are-first
  * Manage/use environments:
    * https://conda.io/docs/user-guide/tasks/manage-environments.html
    * https://medium.freecodecamp.org/why-you-need-python-environments-and-how-to-manage-them-with-conda-85f155f4353c
  * Install packages that aren't available via conda: https://stackoverflow.com/questions/41060382/using-pip-to-install-packages-to-anaconda-environment
  * Install TensorFlow: https://medium.com/@Oysiyl/install-tensorflow-1-8-0-with-gpu-from-source-on-ubuntu-18-04-bionic-beaver-35cfa9df3600
* What's a...
  * Generator: https://stackoverflow.com/questions/1756096/understanding-generators-in-python
  * _pycache_ file:
    * https://www.python.org/dev/peps/pep-3147/
    * https://stackoverflow.com/questions/16869024/what-is-pycache
* Humor
  * https://xkcd.com/353/
  * https://xkcd.com/1987/

### R
* Reference
  * Free Textbooks
    * _Hands-On Programming with R_ (Grolemund): https://rstudio-education.github.io/hopr/
    * _R for Data Science_ by [@hadley](https://github.com/hadley/) and [@garrettgman](https://github.com/garrettgman): https://r4ds.had.co.nz/
      * Some solutions (Arnold): https://jrnold.github.io/r4ds-exercise-solutions/
    * _Text Mining with R_ by [@juliasilge](https://github.com/juliasilge) and [@dgrtwo](https://github.com/dgrtwo/) https://www.tidytextmining.com/
  * Cheat sheets: https://www.rstudio.com/resources/cheatsheets/
    * ggplot2:
      * Two pages: https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf
      * Longer: http://zevross.com/blog/2014/08/04/beautiful-plotting-in-r-a-ggplot2-cheatsheet-3/
    * Syntax comparison: base R vs. formula vs. tidyverse: http://www.science.smith.edu/~amcnamara/Syntax-cheatsheet.pdf
  * Styleguides
    * From Google: https://google.github.io/styleguide/Rguide.xml
    * Tidyverse: http://style.tidyverse.org/
  * R Cookbook: http://www.cookbook-r.com/
* Search engine for R help: https://rseek.org/
* Learn R
  * Intro to R for Decision Modelers (Pechlivanoglou et al): https://github.com/DARTH-git/Handbook-R/blob/master/Handbook_in_R_markdown.pdf
  * Intro to R seminar code (IDRE): https://stats.idre.ucla.edu/stat/data/intro_r/intro_r_flat.html
  * Collection of tutorials
    * UC Business Analytics: http://uc-r.github.io/
    * Coding club (Univ. of Edinburgh): https://ourcodingclub.github.io/tutorials/
  * Websites:
    * R-bloggers: https://www.r-bloggers.com/
    * FAQ on StackOverflow: https://stackoverflow.com/questions/tagged/r-faq
* Communities
  * Tidy Tuesdays - a weekly data viz project https://github.com/rfordatascience/tidytuesday/blob/master/README.md
  * Community to walk through _R for Data Science_ book together: https://medium.com/@kierisi/r4ds-the-next-iteration-d51e0a1b0b82
* Packages/topics
  * Epidemic network modeling: http://statnet.github.io/nme/index.html
  * dplyr
    * Selecting columns https://suzan.rbind.io/2018/01/dplyr-tutorial-1/
    * Filtering rows
      https://suzan.rbind.io/2018/02/dplyr-tutorial-3/
    * Summarizing and slicing https://suzan.rbind.io/2018/04/dplyr-tutorial-4/
    * Gifs of join types (gadenbuie): https://github.com/gadenbuie/tidy-animated-verbs#tidy-animated-verbs
  * Bootstrapping
    * slipper - https://github.com/jtleek/slipper
    * boot - https://cran.r-project.org/web/packages/boot/index.html
      * How to: https://stats.idre.ucla.edu/r/faq/how-can-i-generate-bootstrap-statistics-in-r/
  * reprex: https://github.com/tidyverse/reprex
    * Prep short bits of code (e.g., to post on StackOverflow)
  * Webscraping
    * http://www.interhacktives.com/2017/01/25/scrape-tweets-r-journalists/
    * http://utstat.toronto.edu/~nathan/teaching/sta4002/Class1/scrapingtwitterinR-NT.html
  * K-means
    * https://uc-r.github.io/kmeans_clustering
  * sociome (social determinants of health) https://rdrr.io/github/NikKrieger/sociome/
* Operations research
  * Overviews
    * Paper on using R for OR: http://josilber.scripts.mit.edu/IAPEducationPaperDistribute.pdf
  * R for operations research (website): https://www.r-orms.org/
  * ompr (mixed-integer LPs): https://github.com/dirkschumacher/ompr
  * optplot (plot opt models): https://github.com/dirkschumacher/optplot
* Simulation
  * Tutorial on microsimulation (Krijkamp et al.): https://github.com/DARTH-git/Microsimulation-tutorial
* Health economics
  * hesim (simulation): http://innovationvalueinitiative.github.io/hesim/
  * dampack (decision-analytic models): https://github.com/feralaes/dampack
* Visualizations
  * Examples
    * R Graph Gallery: https://www.r-graph-gallery.com/
  * Create figures
    * ggplot2: https://ggplot2.tidyverse.org/
    * ggpubr: http://www.sthda.com/english/rpkgs/ggpubr/
      * Wrapper around ggplot - intended to be easier to create pub-ready figures
  * rvg: https://github.com/davidgohel/rvg
    * Export figures so they can be editable in powerpoint
  * Graphs and networks
    * DiagrammeR https://github.com/rich-iannone/DiagrammeR
      * Example (Kalvelagen) http://yetanothermathprogrammingconsultant.blogspot.com/2018/07/graph-drawing-in-rstudio.html
    * Plotly: https://plot.ly/python/tree-plots/
  * Gantt charts
    * GanttR function: https://insileco.github.io/2017/09/20/gantt-charts-in-r/
    * Other options: https://stackoverflow.com/questions/3550341/gantt-charts-with-r
  * Interactive timelines
    * timevis: https://github.com/daattali/timevis
  * Spatial data
    * sf package (simple features): https://github.com/r-spatial/sf
  * Maps
    * urbnmapr: https://github.com/UrbanInstitute/urbnmapr
       * State and county maps
  * Colors / themes
    * RColorBrewer
      * Explanation (by chelsea in R): https://moderndata.plot.ly/create-colorful-graphs-in-r-with-rcolorbrewer-and-plotly/
      * GUI to review options on a map: http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3
* Markdown/reports
  * Tufte style for markdown: https://github.com/rstudio/tufte
  * knitr html template: http://biostat.mc.vanderbilt.edu/wiki/Main/KnitrHtmlTemplate
* How to...
  * Rearrange categories in a plot https://trinkerrstuff.wordpress.com/2012/10/15/how-do-i-re-arrange-ordering-a-plot/
  * Save high resolution figures: https://www.r-bloggers.com/high-resolution-graphics-with-r/
  * Plot all data in background on faceted ggplot2 figures: https://drsimonj.svbtle.com/plotting-background-data-for-groups-with-ggplot2
  * Iteratively make plots
    * Using loops: https://ourcodingclub.github.io/2017/02/08/funandloops.html
    * Using purrr by [@dpananos](https://github.com/Dpananos) https://dpananos.github.io/posts/2018/04/blog-post-8/
  * Plot multiple figures
    * Faceting (must be same plot type): https://stackoverflow.com/questions/31798162/generating-multiple-plots-in-ggplot-by-factor
    * cowplot (Claus Wilke): https://cran.r-project.org/web/packages/cowplot/vignettes/plot_grid.html
      * Shared legends: https://cran.r-project.org/web/packages/cowplot/vignettes/shared_legends.html
    * GridExtra (paneling ggplot figures): https://www.r-bloggers.com/extra-extra-get-your-gridextra/
    * Multiplot function: http://www.cookbook-r.com/Graphs/Multiple_graphs_on_one_page_(ggplot2)/
    * If using base R: https://www.statmethods.net/advgraphs/layout.html
  * Convert axes to percents: https://stackoverflow.com/questions/27433798/how-to-change-y-axis-range-to-percent-from-number-in-barplot-with-r
  * Fit distributions: http://www.di.fc.ul.pt/~jpn/r/distributions/fitting.html
  * Write an R package by [@jtleek](https://github.com/jtleek): https://github.com/jtleek/rpackages
  * Update R: https://www.linkedin.com/pulse/3-methods-update-r-rstudio-windows-mac-woratana-ngarmtrakulchol
    * Run in RGui rather than RStudio
  * Add code to text you when your model is done running:
    * https://www.r-bloggers.com/let-r-python-send-messages-when-the-algorithms-are-done-training/
      * Uses Telegram's Bot API: https://core.telegram.org/api
* What is...
  * :: https://stackoverflow.com/a/35241015
  * Pipe operator %>%
    * Short explanation from [@hadley](https://github.com/hadley/) https://github.com/hadley/healthyr_preamble
    * Longer from DataCamp: https://www.datacamp.com/community/tutorials/pipe-r-tutorial
  * Environments, namespaces, etc. (Suraj Gupta): http://blog.obeautifulcode.com/R/How-R-Searches-And-Finds-Stuff/
* Funny or fun
  * Cowsay: https://cran.r-project.org/web/packages/cowsay/vignettes/cowsay_tutorial.html
    * Make animals say funny things (Yoda is my favorite)
  * Excel 2003 themed figures: https://cran.r-project.org/web/packages/ggthemes/vignettes/ggthemes.html
  * GeomMLBStadiums: https://github.com/bdilday/GeomMLBStadiums
    * Draw baseball stadiums in ggplot2

### GitHub
  * Beginner Tutorial: http://try.github.io/
  * Guide to Git with R: http://happygitwithr.com/
  * Cheat sheets
    * By Chris Albon: https://chrisalbon.com/software_engineering/cloud_computing/github_cheatsheet/
    * By Joshua Hibbert: https://github.com/joshnh/Git-Commands
    * Markdown: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
  * Convert Jupyter notebooks in repo to executables: https://mybinder.org/
  * How to...
    * Install git: https://www.develves.net/blogs/asd/articles/using-git-with-powershell-on-windows-10/#installing-git
    * Undo: https://www.atlassian.com/git/tutorials/undoing-changes
    * Save credentials (i.e., username/password):
    https://help.github.com/articles/caching-your-github-password-in-git/
    * Exit git log: https://stackoverflow.com/questions/9483757/how-to-exit-git-log-or-git-diff (soln: type 'q')
    * Repos
      * Clone a repo: https://help.github.com/articles/cloning-a-repository/
      * Use cloned repo: https://stackoverflow.com/questions/14217406/why-i-cant-push-a-newly-cloned-repo
    * Manage branches
      * Merge: https://www.atlassian.com/git/tutorials/using-branches/git-merge
      * Delete: https://koukia.ca/delete-a-local-and-a-remote-git-branch-61df0b10d323
    * Deal with errors:
      * Local changes being overwritten: https://stackoverflow.com/questions/15745045/how-do-i-resolve-git-saying-commit-your-changes-or-stash-them-before-you-can-me
      * Unlink of file: https://stackoverflow.com/questions/4389833/unlink-of-file-failed-should-i-try-again
        * Essentially: had to close AMPL, then worked fine
  * Specifics (background)
    * What is a bare repository? http://www.saintsjd.com/2011/01/what-is-a-bare-git-repository/
  * Humor:
    * https://xkcd.com/1597/
    * https://xkcd.com/1296/

### General coding / computation
* Overview/best practices
  * Overview and slides from [@tommlogan](https://github.com/tommlogan): http://reckoningrisk.com/research-practice/coding/2018/better-coding-practices
  * Best practices from [@marcio-mourao](https://github.com/marcio-mourao): https://rawgit.com/marcio-mourao/Programming-Best-Practices/master/Workshop.html
  * Good enough practices (Wilson et al.): https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510
* Courses
  * System and Software Tools (slides): https://courses.cs.washington.edu/courses/cse391/16sp/index.shtml
  * Intro to computing for computer scientists (lectures): https://c4cs.github.io/
    * E.g., Linux, command line, version control, shells, scripting
  * Computing for Social Sciences (slides, resources, etc.): https://cfss.uchicago.edu/syllabus.html
* Command line
  * Bash
    * Shell commands: https://courses.cs.washington.edu/courses/cse391/16sp/bash.html
    * Reference manual: https://www.gnu.org/software/bash/manual/bashref.html
  * Overview (William Shotts): http://linuxcommand.org/index.php
  * Free textbook: _The Linux Command Line_ (William Shotts) http://linuxcommand.org/tlcl.php
  * Intro (slides, UM CSCAR): https://cscar.research.umich.edu/wp-content/uploads/sites/5/2016/09/Intro-to-Command-Line.pdf
* Linux
  * Intro course (free online): https://training.linuxfoundation.org/training/introduction-to-linux/
* Remote computing
  * SSH - aka Secure Shell (allows secure remote login even if network insecure)
    * PuTTy: https://www.putty.org/
  * File transfer
    * (Windows) WinSCP: https://winscp.net/eng/download.php
    * (Mac/Windows) Cyberduck: https://cyberduck.io/
    * Large files: Globus: https://www.globus.org/
      * Basic version for research/education is free
  * Cluster computing
    * PBS overview (batch scripting, 40min video): https://www.youtube.com/watch?v=SW8Lu1-JaSM
    * Unix
      * Book: _The Unix Workbench_ (Kross) https://seankross.com/the-unix-workbench/
      * vi commands: https://www.cs.colostate.edu/helpdocs/vi.html
* Other
  * src vs. bin folders: https://www.quora.com/Eclipse-software-Whats-the-difference-between-the-bin-and-src-folders
  * How to add environment variables/PATH: https://helpdeskgeek.com/windows-10/add-windows-path-environment-variable/
* Text editors
  * Atom: https://atom.io/
  * Vim: https://www.vim.org/
    * Vim Adventures (game to learn Vim): https://vim-adventures.com/
  * Emacs: https://www.gnu.org/software/emacs/
  * Visual Studio Code: https://code.visualstudio.com/
  * Sublime: https://www.sublimetext.com/
  * Nano: https://www.nano-editor.org/

### AMPL
* (Free) Book: https://ampl.com/resources/the-ampl-book/chapter-downloads/
* Google group (help forum): https://groups.google.com/forum/#!forum/ampl
* Specifics
  * Dynamic set definitions
    https://groups.google.com/forum/#!msg/ampl/Wr_KxvKWBpM/FGeILLXGZzAj
    * E.g., AVAIL vs. AVAIL_all
  * argmin: https://ampl.com/faqs/i-have-declared-set-s-and-param-b-s-how-do-i-write-an-ampl-expression-for-the-arg-min-of-bi-that-is-the-s-in-s-such-that-bs-equals-the-minimum-of-bi-over-all-i-in-s/
  * Sampling discrete random variables from uniform distribution: https://groups.google.com/forum/#!msg/ampl/Wjl-PC-kkiY/FGgDMedidLkJ

### Other programming languages
* Julia
  * Optimization in Julia: http://www.juliaopt.org/
    * Nice summary of solvers at bottom of page
  * Modeling languages
    * JuMP (general): http://www.juliaopt.org/JuMP.jl/0.18/
    * Convex.jl (disciplined convex): https://convexjl.readthedocs.io/en/latest/
  * Solvers/algorithms
    * JuliaStochOpt: https://github.com/JuliaStochOpt
      * Including: discrete-time stochastic control: https://github.com/JuliaStochOpt/StochDynamicProgramming.jl
    * SDDP (stochastic dual dynamic prog): https://github.com/odow/SDDP.jl
      * Very nice documentation with tutorials: https://odow.github.io/SDDP.jl/latest/index.html
    * SDDiP (SDDP with integer variables): https://github.com/lkapelevich/SDDiP.jl
    * StructJuMP (2-stage stochastic programs): https://github.com/StructJuMP/StructJuMP.jl
    * DSP (stochastic mixed-integer): https://github.com/Argonne-National-Laboratory/DSPsolver.jl
    * Complementarity.jl: https://github.com/chkwon/Complementarity.jl
      * Mixed-complementarity and math programs with equilibrium problems
    * CLP - COIN-OR LP solver: https://github.com/JuliaOpt/Clp.jl
  * Other math
    * Differential equations: http://juliadiffeq.org/
  * Plots: http://docs.juliaplots.org/latest/
  * Timer outputs: https://github.com/KristofferC/TimerOutputs.jl
* SQL
  * Sequel Pro (for Mac): https://www.sequelpro.com/
* MATLAB
  * FAST (open-source): https://web.stanford.edu/~lcambier/fast/index.php
    * Stochastic dual dynamic programming
  * Optimization (paid): https://www.mathworks.com/products/optimization.html
  * Global optimization (paid): https://www.mathworks.com/products/global-optimization.html

### Math programming software
* Overviews
  * From Math Opt Society (Sept 2017) http://www.mathopt.org/Optima-Issues/optima103.pdf
  * Convex MINLP solver comparison (Jun 2018): http://www.optimization-online.org/DB_FILE/2018/06/6650.pdf
  * Benchmarks
    * Linear programs - simplex (Mittelmann) http://plato.asu.edu/ftp/lpsimp.html
* Solvers
  * Commercial
    * CPLEX (free for academics): https://www.ibm.com/products/ilog-cplex-optimization-studio
    * Gurobi (free for academics): http://www.gurobi.com/
    * Xpress:
      * http://www.fico.com/en/products/fico-xpress-optimization
      * https://community.fico.com/community/fico-optimization-community
    * MOSEK: https://www.mosek.com/
      * Esp. SOCP, SDP
  * Non-commercial
    * GLPK (LP, MIP): https://www.gnu.org/software/glpk/
    * SCIP (MIP, MINLP, constraint IP): http://scip.zib.de/
    * Bonmin (MINLP): https://projects.coin-or.org/Bonmin
    * Couenne (Non-convex MINLP): https://projects.coin-or.org/Couenne
    * NEOS:
      * https://neos-server.org/neos/
      * https://neos-guide.org/
    * OpenSolver: https://opensolver.org/
      * Excel add-in (extends the standard Excel solver)
    * Ipopt (nonlinear, local): https://projects.coin-or.org/Ipopt
    * BiqBin (Binary quadratic): http://biqbin.fis.unm.si/
    * DSP (Stochastic mixed-integer programs): https://github.com/Argonne-National-Laboratory/DSP
    * ECOS (Second-order conic programs): https://github.com/embotech/ecos, https://www.embotech.com/ECOS
    * OSQP (Operator Splitting Quadratic Program): https://osqp.org/
    * Mini-CP (Constraint programming): https://minicp.bitbucket.io/
  * OR-Tools from Google: https://developers.google.com/optimization/
* Modeling lanugages
  * SolverStudio (free): http://solverstudio.org/
    * Excel add-on, useful when OpenSolver not big enough
    * Can call commercial solvers
  * AMPL: https://ampl.com/
  * OPL: https://www.ibm.com/analytics/data-science/prescriptive-analytics/optimization-modeling
  * LP add-on for Google sheets: https://developers.google.com/optimization/lp/add-on
* Application specific
  * Facility location
    * SITATION: https://daskin.engin.umich.edu/software/
  * Agent-based
    * NetLogo: https://ccl.northwestern.edu/netlogo/


### Math programming resources
* Textbooks available for free
  * _A First Course in Linear Optimization v3.0_ by [@jon77lee](https://github.com/jon77lee/): https://github.com/jon77lee/JLee_LinearOptimizationBook/blob/master/JLee.3.0.pdf
  * _Convex Optimization_ (Stephen Boyd and Lieven Vandenberghe) http://www.seas.ucla.edu/~vandenbe/cvxbook.html
  * _MOSEK Modeling Cookbook_ https://themosekblog.blogspot.dk/2018/05/new-modeling-cookbook.html
    * Conic optimization, not specific to MOSEK solver
  * _Foundations and Methods of Stochastic Simulation_  (Barry Nelson) http://users.iems.northwestern.edu/~nelsonb/IEMS435/
  * _Intro to Applied Linear Algebra_ (Stephen Boyd and Lieven Vandenberghe): https://web.stanford.edu/~boyd/vmls/
  * Myths and Counterexamples (Harvey Greenberg): https://glossary.informs.org/myths/CurrentVersion/myths.pdf
* Communities / forums
  * OR Exchange: https://www.or-exchange.org/
  * Google groups
    * AMPL: https://groups.google.com/forum/#!forum/ampl
    * Gurobi: https://groups.google.com/forum/#!forum/gurobi
    * AIMMS: https://groups.google.com/forum/#!forum/aimms
    * Pyomo: https://groups.google.com/forum/#!forum/pyomo-forum
  * Stack Overflow: https://stackoverflow.com/
  * IE faculty listserv: https://lists.clemson.edu/mailman/listinfo/iefac.list
    * E.g., job postings, etc.
* Overviews
  * Glossary: https://glossary.informs.org/ver2/mpgwiki/index.php?title=Main_Page
  * OR Notes (JE Beasley): http://people.brunel.ac.uk/~mastjjb/jeb/or/orweb.html
* Models
  * GAMS model library: https://www.gams.com/latest/gamslib_ml/libhtml/
* Algorithms
  * List/explanation from the folks at NEOS: https://neos-guide.org/algorithms
* Test sets
  * MIPLIB: http://miplib.zib.de/
  * OR Library: http://people.brunel.ac.uk/~mastjjb/jeb/info.html
* Course resources
  * Math Programming (Dimitris Bertsimas):
    - Lecture notes (Fall 2009) - https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-251j-introduction-to-mathematical-programming-fall-2009/lecture-notes/
  * Convex Optimization (Lieven Vandenberghe):
    * Lecture slides: http://www.seas.ucla.edu/~vandenbe/cvxbook/bv_cvxslides.pdf
  * Stochastic programming
    * From Papavasiliou: http://uclengiechair.be/operations-research-linma-2491/
      * Videos, slides
    * From Shapiro, Dentcheva, Ruszczynski: https://www2.isye.gatech.edu/people/faculty/Alex_Shapiro/SPbook.pdf
      * Lecture notes
    *  From Warren Powell (Fall 2017)
      * Readings: https://castlelab.princeton.edu/orf-544/
  * Optimal Learning
    - Various materials (Warren Powell): http://optimallearning.princeton.edu/
* Other
  * IFORS Developing Countries page: http://ifors.org/developing_countries/index.php?title=Main_Page
    * A variety of open-source resources
  * OR societies around the world: http://people.brunel.ac.uk/~mastjjb/jeb/or/orweb.html
  * COIN-OR Foundation: https://www.coin-or.org/
    * Resources: https://www.coin-or.org/resources/
* Benders Decomposition
  * Using callbacks to avoid rebuilding the scenario tree by [@parubin](https://twitter.com/parubin): https://orinanobworld.blogspot.com/2011/10/benders-decomposition-then-and-now.html
  * Examples:
    * In AMPL: https://ampl.com/NEW/LOOP2/
    * With callbacks by [@vitaut](https://github.com/vitaut): http://www.zverovich.net/2013/09/01/modern-benders-decomposition-in-ampl.html
* How to...
  * Linearize product of variables: https://www.leandro-coelho.com/linearization-product-variables/
  * Linearize max/max/absolute value: https://www.leandro-coelho.com/how-to-linearize-max-min-and-abs-functions/
  * Linearize max(0,y) by [@prubin73](https://github.com/prubin73): https://orinanobworld.blogspot.com/2010/12/lps-and-positive-part.html
  * Remember primal / dual conversion
    * Sensible-odd-bizarre (SOB) method: https://math.stackexchange.com/questions/83844/simplex-method-duality-by-bazaraa?answertab=oldest#tab-top
    * Citing: https://www.math.hmc.edu/~benjamin/papers/sob.pdf

### Operations research-adjacent material
* Linear Algebra
  * Intro course lectures from Gilbert Strang: https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/
  * Review and reference (Kolter and Do): http://cs229.stanford.edu/section/cs229-linalg.pdf
  * Intro to matrix algebra (handout, Carey): http://ibgwww.colorado.edu/%7Ecarey/p7291dir/handouts/matrix.algebra.pdf
* Game theory
  * Intro course lectures from Ben Polak: https://oyc.yale.edu/economics/econ-159
* Networks
  * Bayes nets
    * Tutorial (Netica): https://www.norsys.com/tutorials/netica/secA/tut_A1.htm
    * Intro slides (CMU): https://www.cs.cmu.edu/afs/cs/academic/class/15381-s07/www/slides/032707bayesNets1.pdf
* Data Science
  * How to get started
    * Blog post by [@kierisi](https://github.com/kierisi): https://www.jessemaegan.com/post/data-science-with-r-how-do-i-start/
    * Plan (Kross): http://seankross.com/notes/data-science-from-scratch/
  * Applied data science course readings from [@hadley](https://github.com/hadley/) https://github.com/hadley/stats337#readings
  * Directory of lots of data science material: http://www.datasciguide.com/content/
  * Podcast
    * DataFramed from DataCamp: https://www.datacamp.com/community/podcast
  * Intro to data ethics (Shannon Vallor): https://www.scu.edu/ethics/focus-areas/technology-ethics/resources/an-introduction-to-data-ethics/
    * Module could include in courses
* Machine Learning
  * Communities
    * Google group: https://groups.google.com/forum/#!forum/ml-news/categories
    * CrossValidated: https://stats.stackexchange.com/
  * Textbooks
    * _Intro to Statistical Learning_ (James et al.) https://www-bcf.usc.edu/~gareth/ISL/
    * _Elements of Statistical Learning_ (Hastie, Tibshirani, Friedman) https://web.stanford.edu/~hastie/ElemStatLearn/
      * More technical than James et al. book
    * _Statistical Learning with Sparsity_ (Hastie, Tibshirani, Wainwright): https://web.stanford.edu/~hastie/StatLearnSparsity/index.html
    * _A Brief Intro to ML for Engineers_ (Simeone) https://arxiv.org/abs/1709.02840
    * _Fairness in ML_ (Barocas, Hardt, Narayanan) http://fairmlbook.org/
      * Book in progress
  * Technical notes - ML and AI from [@chrisalbon](https://github.com/chrisalbon)
    * Website: https://chrisalbon.com/#machine_learning
    * On github: https://github.com/chrisalbon/notes
  * ML flashcards from [@chrisalbon](https://github.com/chrisalbon)
    * https://machinelearningflashcards.com/
    * Scrape off Twitter for free, code from [@Dpananos](https://github.com/Dpananos): https://github.com/Dpananos/GetCards
  * Course
    * Applied ML [@amueller](https://github.com/amueller): http://www.cs.columbia.edu/~amueller/comsw4995s18/schedule/
      * Includes lecture recordings and slides
    * Course notes (Clayton Scott): http://web.eecs.umich.edu/~cscott/past_courses/eecs545f15/index.html
  * Topics
    * How decision trees work (Rohrer): https://brohrer.github.io/how_decision_trees_work.html
    * Taxonomy of reproducibility: http://www.rctatman.com/files/2018-7-14-MLReproducability.pdf
    * Intro to Monte Carlo tree search: https://int8.io/monte-carlo-tree-search-beginners-guide/
* Compilation of ML/CS/Math resources (Vodrahalli): https://kiranvodrahalli.github.io/links/
* Statistics
  * 10 rules to use stats (comp biology): https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004961
  * Document and avoid these problems (biostat): http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist
  * StatPrimer (Gerstman): http://www.sjsu.edu/faculty/gerstman/StatPrimer/
  * What test should I use? https://stats.idre.ucla.edu/other/mult-pkg/whatstat/
    * With examples in R, Stata, SAS, SPSS
  * Odds ratios
    * Best practices from JAMA (Norton, Dowd, Maciejewski) https://jamanetwork.com/journals/jama/fullarticle/2686777
      * Maybe paywall
  * Specific topics
  * Notes on Dirichlet processes by [@tdhopper](https://github.com/tdhopper): http://dp.tdhopper.com/
  * Experimental design
    * Warning signs (Norvig): http://norvig.com/experiment-design.html
* Probability
  * Review of Probability Theory (Maleki and Do): https://www.cs.mcgill.ca/~dprecup/courses/ML/Materials/prob-review.pdf
* Mathematics
  * Primers (Kun): https://jeremykun.com/primers/
* Computer science
  * Frequently asked questions about C: http://c-faq.com/index.html
* Other
  * Blockchain overview (2 hr video): https://www.youtube.com/watch?v=qOVAbKKSH10
  * Gentle intro to graph theory (Joshi): https://medium.com/basecs/a-gentle-introduction-to-graph-theory-77969829ead8
  * Habits of highly mathematical people (Kun): https://medium.com/@jeremyjkun/habits-of-highly-mathematical-people-b719df12d15e

### Data visualization
* Free Textbooks
  * _Fundamentals of Data Visualization_ by [@clauswilke](https://github.com/clauswilke): http://serialmentor.com/dataviz/
  * _Data Visualization: A Practical Introduction_ by [@kjhealy](https://github.com/kjhealy): http://socviz.co/
* Guide to using color (Rost): https://blog.datawrapper.de/colorguide/
* Networks
  * Overview of software, etc.: https://www.lib.ncsu.edu/measuring-research-impact/visualizing-impact
  * Gephi: https://gephi.org/
    * Tutorial to create citation network: https://www.lib.ncsu.edu/sites/default/files/ResearchImpactNetworkGuide.pdf
  * Citation network example from Neal Caren (Python & d3.js): http://nealcaren.web.unc.edu/a-sociology-citation-network/
  * Graphviz (python): http://graphviz.readthedocs.io/en/stable/index.html
    * Examples: http://graphviz.readthedocs.io/en/stable/examples.html
    * Force-directed graph (json/html): https://bl.ocks.org/mbostock/4062045
* Community
  * Data viz book club: https://blog.datawrapper.de/bookclub-tufte/
    * On Twitter: https://twitter.com/datavisclub

### Datasets/databases
* Note: health-related data is in this [section](#healthcare)
* Search engine: https://toolbox.google.com/datasetsearch
* Compilations
  * Data.gov: https://www.data.gov/
  * From Vanderbilt Biostats: http://biostat.mc.vanderbilt.edu/wiki/Main/DataSets
  * Kaggle: https://www.kaggle.com/datasets
  * Public data sources:
   https://blog.bigml.com/list-of-public-data-sources-fit-for-machine-learning/
    * Targeted towards machine learning
  * Google Public Data Explorer: https://www.google.com/publicdata/directory
  * Public datasets: https://github.com/awesomedata/awesome-public-datasets
  * Compilation of datasets available via various R packages: https://vincentarelbundock.github.io/Rdatasets/datasets.html
  * Network datasets
    * From [@kateto](https://github.com/kateto): http://kateto.net/2016/05/network-datasets/
    * From [@profjure](https://github.com/profjure): https://snap.stanford.edu/data/
  * Time series
    * Compilation (DataMarket): https://datamarket.com/data/list/?q=provider:tsdl
    * Economic (from Fed Reserve): https://fred.stlouisfed.org/
  * Good, small datasets (Vicki Boykis): http://veekaybee.github.io/2018/07/23/small-datasets/
* Specific sources
  * Bureau of Labor Statistics: https://www.bls.gov/data/
    * E.g., Consumer Price Index (inflation): https://www.bls.gov/cpi/data.htm
  * US Census Bureau https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml
  * Pew Research Center
    * Data: http://www.pewresearch.org/download-datasets/
    * Overview of how to analyze in R: https://medium.com/pew-research-center-decoded/how-to-analyze-pew-research-center-survey-data-in-r-f326df360713
  * Neighborhood atlas: https://www.neighborhoodatlas.medicine.wisc.edu/
    * Could use for disparities / deprivation work
    * Perspective about it in NEJM (paywall?): https://www.nejm.org/doi/full/10.1056/NEJMp1802313
  * FiveThirtyEight
    * List of available data: https://data.fivethirtyeight.com/
    * Data for their analyses: https://github.com/fivethirtyeight/data
    * R package https://github.com/rudeboybert/fivethirtyeight
  * European statistics: http://ec.europa.eu/eurostat/data/database
  * IMF: http://www.imf.org/en/Data
  * WHO: http://www.who.int/gho/en/
  * Quandl: https://docs.quandl.com/docs/python
    * Financial / economic data - some are free
    * Python and R packages available
* Literature
  * PubMed: https://www.ncbi.nlm.nih.gov/pubmed/
  * Scopus: https://www.scopus.com/search/form.uri?display=basic
  * Web of Science: https://clarivate.com/products/web-of-science/web-science-form/web-science-core-collection/
  * Embase: https://www.elsevier.com/solutions/embase-biomedical-research
  * CENTRAL (Cochrane reviews) http://www.cochranelibrary.com/about/central-landing-page.html
  * Google Scholar: https://scholar.google.com/

### Communication/dissemination
* Sharing data (guide by [@jtleek](https://github.com/jtleek)): https://github.com/jtleek/datasharing
* How to choose open-source license: https://choosealicense.com/
* Manuscripts
  * How to write
    * Your first paper (guide by [@jtleek](https://github.com/jtleek), biostat): https://github.com/jtleek/firstpaper
    * 12 steps to writing: https://thehealthresearchjourney.wordpress.com/2014/12/05/the-12-steps-to-writing-a-paper-and-staying-sane/
    * Healthcare-focused:
      * Welch, 1999 paper (Prepping for Submission to a Medical Journal)
       https://medicine.umich.edu/sites/default/files/content/downloads/Welch%20Manuscripts.pdf
      * Ibrahim and Dimick (Writing for Impact)
       https://medicine.umich.edu/sites/default/files/content/downloads/WritingResearchPaper_Ibrahim_0.pdf
      * Policy papers in clinical journals (UM CHEAR): https://sph.umich.edu/cehr/pdf/Manuscript_Guide.pdf
    * Reporting guidelines: https://www.equator-network.org/reporting-guidelines/
  * Run a "paper sprint" https://sph.umich.edu/cehr/pdf/Paper_Sprint_Manual.pdf
  * Picking a journal (health-focused): http://jane.biosemantics.org/
  * Staying organized - publication planner (Pacheco-Vega): http://www.raulpacheco.org/2016/06/designing-and-implementing-a-publications-planner/
  * Types of reviews (Temple U): http://guides.temple.edu/c.php?g=78618&p=4156607
    * Systematic, scoping, etc.
* Visual abstracts
  * https://static1.squarespace.com/static/5854aaa044024321a353bb0d/t/5a527aa89140b76bbfb2028a/1515354827682/VisualAbstract_Primer_v4_1.pdf
* Policy
  * How to use research to effect policy (Oxfam): https://www.nature.com/articles/s41599-018-0176-7
  * Connecting research to policy (blog) https://www.healthaffairs.org/do/10.1377/hblog20180403.254308/full/#.Ws43706twu0.twitter
  * More than a press release (Videos): https://theincidentaleconomist.com/wordpress/a-press-release-is-not-enough-videos/
* Working with the media
  * http://senseaboutscienceusa.org/media-guide-for-scientists/
* Writing for lay outlets
  * For "The Conversation" (slides, Chang and Czuhajewski): https://www.slideshare.net/cczuhajewski/writing-for-the-conversation-106342981
* Writing help
  * Lots of resources from Purdue: https://owl.purdue.edu/owl/purdue_owl.html
* Reference software
  * Zotero: https://www.zotero.org/
  * Mendeley: https://www.mendeley.com/
  * EndNote: http://endnote.com/
* LaTeX
  * Getting started: https://nilesjohnson.net/latex.html
    * Code: https://gitlab.com/nilesjohnson/latex_starter
  * Overview (Wilkins): https://www.maths.tcd.ie/~dwilkins/LaTeXPrimer/
  * Collaboration
    * ShareLaTeX: https://www.sharelatex.com/
  * Example style template for journals https://www.leandro-coelho.com/default-latex-article-style-modifications/
  * Thesis templates:
    * U Wolverhamptom: https://github.com/snim2/phdtemplate
    * Michigan: http://clasp.engin.umich.edu/pages/current/dissertation-template
  * Beamer tips and tricks by [@paulgp](https://github.com/paulgp)
    * Presentation: https://github.com/paulgp/beamer-tips/blob/master/slides.pdf
    * Source code: https://github.com/paulgp/beamer-tips
  * Graphics
    * Tikz and PGF: http://www.texample.net/tikz/
  * Indicating math mode
    * Using /( /) vs $: https://tex.stackexchange.com/questions/510/are-and-preferable-to-dollar-signs-for-math-mode

### Healthcare
* Guides
  * Healthcare Industry (largely UM students only) https://kresgeguides.bus.umich.edu/healthcarebiotechhome
  * Health management and policy: http://guides.lib.umich.edu/hmp
  * Finding health statistics
    * From UM: http://guides.lib.umich.edu/healthstats
    * From Wisconsin-Madison: http://researchguides.ebling.library.wisc.edu/c.php?g=293234
* Datasets / databases
  * Public
    * Medicare Part B
      * National summary files: https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Part-B-National-Summary-Data-File/Overview.html
      * Carrier summary files: https://www.cms.gov/Research-Statistics-Data-and-Systems/Downloadable-Public-Use-Files/Part-B-Carrier-Summary-Data-File/Overview.html
      * Not free:
        * CCW https://www.ccwdata.org/web/guest/home
    * CDC data/stats: https://www.cdc.gov/DataStatistics/
      * Chronic disease datasets: https://chronicdata.cdc.gov/
      * E.g., Maternal and child health: https://chronicdata.cdc.gov/browse?category=Maternal+%26+Child+Health
  * Other
    * Clinical trials: https://clinicaltrials.gov/
    * Tufts Cost-Effectiveness Analysis Registry: http://healtheconomics.tuftsmedicalcenter.org/cear4/Home.aspx
  * Major surveys
    * NHANES (in person): https://www.cdc.gov/nchs/nhanes/index.htm
    * BRFSS (phone): https://www.cdc.gov/brfss/annual_data/annual_data.htm
      * Pronounced "Burfiss"
* Newsletters
  * CDC's MMWR: https://www.cdc.gov/mmwr/index.html
    * Morbidity and Mortality Weekly Report
    * I think most people I know working in public health subscribe to this

### Jobs/Summer schools
* Jobs
  * Companies that hire folks to work on OR problems/methods from [@dirkschumacher](https://github.com/dirkschumacher): https://github.com/dirkschumacher/or-companies/
  * Infectious disease dynamics listserv: http://iddjobs.org/jobs/
  * United Nations (UN) jobs: https://unjobhunt.com/
    * Website from [@dirkschumacher](https://github.com/dirkschumacher), not affiliated with UN
  * National labs
    * Sandia
      * Links for fellowships/postdocs: http://www.sandia.gov/careers/students_postdocs
    * National Renewable Energy Lab (NREL)
      * https://www.nrel.gov/careers/
      * Director's Postdoc Fellowship: https://www.nrel.gov/careers/directors-fellowship.html?mc_cid=6e3282f94d&mc_eid=079dfe7593
    * Oak Ridge
      * Postdocs https://www.ornl.gov/content/ornl-s-postdoctoral-program
      * Weinberg Fellowship: https://www.ornl.gov/careers/alvin-m-weinberg-fellowship
      * Householder Fellowship: https://www.ornl.gov/careers/alston-s-householder-fellowship
  * Twitter feeds with job postings
    * R stats: https://twitter.com/rjoblistings
    * Data science: https://twitter.com/NewDataSciJobs
* Career prep
  * Questions to think through career goals [@benlangmead](https://github.com/benlangmead): https://github.com/BenLangmead/langmead-lab/blob/master/postdoc_questionnaire.md
    * Slightly expanded from [@jtleek](https://github.com/jtleek): https://github.com/jtleek/careerplanning
  * Academic jobs
    * Tons of resources compiled by UM CRLT: http://crlt.umich.edu/PFF_Resources
* Winter Schools
  * List compiled by Thiago Serra (Winter 2018-19):
   https://thiagoserra.com/2018/08/27/winter-2018-2019-schools-on-algorithms-big-data-data-science-discrete-math-optimization-and-other-relevant-orms-topics/

### Twitter
* Communities I appreciate
  * [#orms](https://twitter.com/hashtag/orms?src=hash)
  * [#rstats](https://twitter.com/hashtag/rstats?src=hash)
  * [#phdchat](https://twitter.com/hashtag/phdchat?src=hash)
  * [#AcWri](https://twitter.com/hashtag/acwri?src=hash)
  * [#scicomm](https://twitter.com/hashtag/scicomm?src=hash)
* Not related to what I do but fun to watch
  * [#girlmedtwitter](https://twitter.com/hashtag/girlmedtwitter?src=hash)
* Hashtags that have included interesting discussions at some point
  * [#hiddencurriculum](https://twitter.com/hashtag/hiddencurriculum?src=hash)
  * [#phdtips](https://twitter.com/hashtag/phdtips?src=hash)
* Other
  * CV without Twitter (Auriel Fournier): http://aurielfournier.github.io/cv-without-twitter/

### Funding
* Compilations
  * For early career researchers (JHU): https://research.jhu.edu/rdt/funding-opportunities/early-career/
  * From _Science_: http://www.sciencemag.org/careers/where-search-funding
  * From USC: https://research.usc.edu/for-investigators/funding/federal/
* Federal grants: https://www.grants.gov/
* Specific
  * FDA (Generic drug-related): https://www.fda.gov/Drugs/ResourcesForYou/Consumers/BuyingUsingMedicineSafely/GenericDrugs/ucm585566.htm

### Teaching
* Guidebook from UM CRLT: http://www.crlt.umich.edu/gsis/gsi_guide
* Diversity and inclusion in the classroom (Laura Albert): https://punkrockor.com/2016/04/21/what-i-do-for-diversity-and-inclusion-in-the-classroom/

### Blogs I like (and read occasionally)
* Operations research-ish
    * Punk Rock OR by [@lauraalbertphd](https://twitter.com/lauraalbertphd): https://punkrockor.com/
    * OR in an OB World by [@prubin73](https://github.com/prubin73): https://orinanobworld.blogspot.com/
    * Yet Another Math Programming Consultant (Kalvelagen): http://yetanothermathprogrammingconsultant.blogspot.com/
    * Geraint Palmer's blog [@geraintpalmer](https://github.com/geraintpalmer): http://www.geraintianpalmer.org.uk/blog/
    * Thiago Serra's blog: https://thiagoserra.com/blog/
    * Reckoning Risk by [@TomMLogan](https://github.com/tommlogan) and [@t-g-williams](https://github.com/t-g-williams): http://reckoningrisk.com/
* Other
    * Math3Ma by [@math3ma](https://twitter.com/math3ma) (math): http://www.math3ma.com/
    * Math Intersect Programming (Kun): https://jeremykun.com/
    * Azimuth (various STEM fields trying to save the planet): https://johncarlosbaez.wordpress.com/
      * Index of entries: http://www.azimuthproject.org/azimuth/show/Azimuth+Blog
    * Armchair Ecology (Poisot, computational biology): https://armchairecology.blog/
* Humor
    * Math with Bad Drawings: https://mathwithbaddrawings.com/
    * Lego Grad Student: https://brickademics.com/
    * PhD Comics: http://phdcomics.com/comics/most_popular.php

### Various advice
* Grad students
  * For new grad students (Dorsa Amir): https://medium.com/@dorsaamir/modest-advice-for-new-graduate-students-b0be6b8dbc22
  * Guide to grad school (Adam Marcus, CS): http://marcua.net/writing/gradschool-guide/
  * Guidebook for succeeding in the PhD (Alex Eble, econ): https://static1.squarespace.com/static/55c143d9e4b0cb07521c6d17/t/5b4f409f575d1ff83c2f12d8/1531920545061/PhDGuidebook.pdf
    * If that link gets broken, perhaps also available on this page: http://www.alexeble.com/advice/
  * Succeeding in the PhD (Dredze, Wallach; computer science): http://www.cs.jhu.edu/~mdredze/publications/HowtoBeaSuccessfulPhDStudent.pdf
  * Advisor/PhD student dynamics: https://chroniclevitae.com/news/1793-handling-your-imperfect-adviser
  * For female grad students (political science): https://docs.google.com/document/d/1DMoSXf7pGRLMN1VP5-36nu2mkNBFEsJtERCi-AERwKk/edit
    * Google doc - compiled by [@dianazobrien](https://twitter.com/dianazobrien)
  * Attending big conferences (Kieran Healy, sociology): https://kieranhealy.org/blog/archives/2003/08/27/conference-advice/
  * The Professor Is In (Karen Kelsky): http://theprofessorisin.com/
    * Blog with various academic advice
  * Compilations
    * Doing research (Arinivas Akella, CS): https://webpages.uncc.edu/sakella/advice.html
    * Grad school, technical writing, etc. (Mihir Bellare, CS): http://cseweb.ucsd.edu/~mihir/education.html
* Applying to grad school
  * Website with lots of advice: https://kcklett.wixsite.com/phduo
* New faculty
  * The 7 Year Postdoc https://blogs.scientificamerican.com/guest-blog/the-awesomest-7-year-postdoc-or-how-i-learned-to-stop-worrying-and-love-the-tenure-track-faculty-life/
    * Counter thoughts: http://mathbionerd.blogspot.com/2017/07/not-awesomest-7-year-postdoc.html
  * If the 3rd year review goes poorly (Albertson): https://www.chronicle.com/article/Operation-Keep-My-Job-/235535
* Job search
  * Academic search (Nagi): http://publish.illinois.edu/engr-mavis/files/2014/09/Academic-Job-Search-2016.pdf
  * Data science jobs by [@robinsones](https://github.com/robinsones): http://hookedondata.org/Advice-for-Applying-to-Data-Science-Jobs/
  * Vitae https://chroniclevitae.com/
    * Database, advice, etc.
  * Job market mistakes (humanities): https://www.chronicle.com/article/5-Big-Picture-Mistakes-New/243475
* Various
  * 8 tips for saying no by [@APottegard](https://twitter.com/APottegard): http://www.antonpottegaard.dk/download/HowToSayNo.pdf
  * The Pac-Man rule (Holscher): http://ericholscher.com/blog/2017/aug/2/pacman-rule-conferences/
    * Always leave room for someone to join the group
  * An econ prof (Hal Varian) describes his work style: http://people.ischool.berkeley.edu/~hal/Papers/how.pdf
  * Various advice posts on Chris Blattman's blog (econ prof) https://chrisblattman.com/
    * Links on right-hand side of blog
  * When your data science project doesn't work: https://medium.com/@skyetetra/so-your-data-science-project-isnt-working-7bf57e3f12f1
* Skills
  * Reading papers by [@jtleek](https://github.com/jtleek): https://github.com/jtleek/readingpapers
  * Writing lit reviews (Raul Pacheco-Vega): http://www.raulpacheco.org/resources/literature-reviews/
  * Organizing data in a spreadsheet (Broman and Woo, open access): https://www.tandfonline.com/doi/full/10.1080/00031305.2017.1375989
    * Not always the best idea, but here are some tips
  * How to review a paper by [@jtleek](https://github.com/jtleek): https://github.com/jtleek/reviews
  * Coding
    * Writing production-level code (Pappakrishnan) https://www.datascience.com/blog/production-level-code-for-data-science
    * How to Report Bugs Effectively (Simon Tatham): https://www.chiark.greenend.org.uk/~sgtatham/bugs.html
      * Perhaps helpful to send to your users
  * Debugging
    * Infeasible models (Kalvelagen): http://yetanothermathprogrammingconsultant.blogspot.com/2018/08/the-best-way-to-debug-infeasible-models.html
    * Rubber ducky method: https://rubberduckdebugging.com/
      * Explain in detail to an inanimate object
    * Wolf-fence algorithm: http://coreygoldberg.blogspot.com/2008/12/wolf-fence-debugging.html
      * Basically binary search with fun description
      * Original paper (paywall): https://dl.acm.org/citation.cfm?id=358695

### Eclectic
* CV of failures
  * https://www.princeton.edu/~joha/Johannes_Haushofer_CV_of_Failures.pdf
  * https://www.washingtonpost.com/news/wonk/wp/2016/04/28/it-feels-really-good-to-read-about-this-princeton-professors-failures/
* On the "hidden curriculum" of grad school: https://scatter.wordpress.com/2018/07/24/guest-post-grad-schools-hidden-curriculum/
* List of "awesome" lists https://github.com/sindresorhus/awesome
  * Very meta. But also potentially helpful.
* Azimuth Project: http://www.azimuthproject.org/azimuth/show/HomePage
  * Collaboration of scientists and engineers who want to save the planet
* Guide to Bad Data
  * Github: https://github.com/Quartz/bad-data-guide
  * Article on Quartz: https://qz.com/572338/the-quartz-guide-to-bad-data/#user-content-there-are-inexplicable-outliers
* Technical / scientific debt: http://varianceexplained.org/r/scientific-debt/
   * Interesting take from [@dgrtwo](https://github.com/dgrtwo) on managing shortcuts/assumptions/etc. in the project development process
* Types of validity (Amy Bucher):  http://www.amybucherphd.com/statistical-validity-types/
* Testing: https://towardsdatascience.com/testing-to-learn-part-1-16a7968d2ba3
* Various software
  * Convert figure to (x,y) data: https://www.digitizeit.de/
  * Compare pdf files: https://draftable.com/compare
  * Accessibility
     * Convert screen to what a color blind person would see: http://colororacle.org/
  * Poll meeting availability
    * When2Meet: https://www.when2meet.com/
    * When is good: http://whenisgood.net/
* Fun OR (or related) applications
  * 2048 using MDPs [@jdleesmiller](https://github.com/jdleesmiller): http://jdlm.info/articles/2018/03/18/markov-decision-process-2048.html
  * Chutes & Ladders as a Markov chain [@jakevdp](https://github.com/jakevdp): https://jakevdp.github.io/blog/2017/12/18/simulating-chutes-and-ladders/#Fundamental-Matrix
  * Mario Kart drivers - Pareto efficiency [@hinnefe2](https://github.com/hinnefe2): http://hinnefe2.github.io/python/tools/2015/09/21/mario-kart.html
  * Text mining on country music lyrics (Miller): https://www.johnwmillr.com/trucks-and-beer/
* OR/Programming/etc. in Industry
  * Netflix: https://medium.com/netflix-techblog/notebook-innovation-591ee3221233
* 15 important algorithms (McFadden): https://interestingengineering.com/15-of-the-most-important-algorithms-that-helped-define-mathematics-computing-and-physics
* 100 days of algorithms (Bouda): https://medium.com/100-days-of-algorithms
  * Code: https://github.com/coells/100days
* Beer game using AI: https://beergame.opexanalytics.com/#/
* Websites
  * (Free) Hosted by github: https://pages.github.com/
    * Themes: https://github.com/topics/jekyll-theme
    * Simple one for academics https://github.com/academicpages/academicpages.github.io
      * Example of what it looks like: https://academicpages.github.io/
    * Template for labs: http://www.allanlab.org/aboutwebsite.html
  * (Free/Paid) Wix: https://www.wix.com
  * (Free) Google Sites: https://sites.google.com/
* Icons: https://www.iconsdb.com/
  * E.g., the Google Scholar logo
* Download GoogleMaps to use offline: https://support.google.com/maps/answer/6291838
* Humor
  * Top 10 Illegitimate Proof Techniques https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/lecture-3-strong-induction/MIT6_042JF10_proof.pdf
    * (I think the original version of this list came from Dana Angluin)
  * "The best way to write secure and reliable applications" https://github.com/kelseyhightower/nocode
  * Add coffee stains to your LaTeX files: http://hanno-rein.de/archives/349
  * Guide to interpreting faculty feedback: https://kieranhealy.org/blog/archives/2013/08/16/academic-feedback/
  * Spurious correlations: http://www.tylervigen.com/spurious-correlations
    * Make your own: http://tylervigen.com/discover
  * Create parody O'Reilly book covers: https://dev.to/rly
  * Computer science research topic generator: https://www.cs.purdue.edu/homes/dec/essay.topic.generator.html
  * Gettysburg address via powerpoint: http://norvig.com/Gettysburg/index.htm

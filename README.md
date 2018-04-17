# Resources

Consider this a public bookmark bar. These are resources I've found useful or think might be one day. Not comprehensive, links may not work, in no particular order.

# Python
* Overview
  * Whirlwind tour from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/WhirlwindTourOfPython
  * Overview from [@drvinceknight](https://github.com/drvinceknight): https://vknight.org/Introduction_to_OOP/OverviewOfPython/
* More extensive tutorials
  * Python Software Foundation: https://docs.python.org/3.6/tutorial/index.html
* Textbooks
  * (Free) _Think Python_ by [@AllenDowney](https://github.com/AllenDowney) http://greenteapress.com/wp/think-python-2e/
    * Beginners guide, programming exp. not necessary
  * (Free) _Python Data Science Handbook_ by [@jakevdp](https://github.com/jakevdp) https://jakevdp.github.io/PythonDataScienceHandbook/
* OR/MS-related Python packages: https://wiki.python.org/moin/PythonForOperationsResearch
* Topics
  * Simulation
    * (Book chapter) by Barry Nelson: http://users.iems.northwestern.edu/~nelsonb/IEMS435/PythonSim.pdf
  * ML
      * Flowchart: choosing the right estimator: http://scikit-learn.org/stable/tutorial/machine_learning_map/
      * Sklearn tutorial from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/sklearn_tutorial
  * Supply chain
    * https://github.com/KevinFasusi/supplychainpy
* Figures
  * R-style graphing
    * plotnine package: https://plotnine.readthedocs.io/en/stable/
    * ggplot package: https://www.r-bloggers.com/ggplot2-style-plotting-in-python/
  * Funny
    * XKCD-style figures: https://matplotlib.org/xkcd/examples/showcase/xkcd.html

# R
* Textbooks
  * (Free) _R for Data Science_ by [@hadley](https://github.com/hadley/) and [@garrettgman](https://github.com/garrettgman)
https://r4ds.had.co.nz/
    * Community to learn/walk through book together: https://medium.com/@kierisi/r4ds-the-next-iteration-d51e0a1b0b82
  * (Free) _Text Mining with R_ by [@juliasilge](https://github.com/juliasilge) and [@dgrtwo](https://github.com/dgrtwo/) https://www.tidytextmining.com/
* Explanation of topics
  * Pipe operator %>%
    * Short explanation from [@hadley](https://github.com/hadley/) https://github.com/hadley/healthyr_preamble
    * Longer from DataCamp: https://www.datacamp.com/community/tutorials/pipe-r-tutorial
* Packages (perhaps with corresponding tutorials)
  * Minor but helpful
    * GridExtra (paneling ggplot figures): https://www.r-bloggers.com/extra-extra-get-your-gridextra/
  * Larger
    * Epidemic network modeling: http://statnet.github.io/nme/index.html
    * dplyr
      * Selecting columns https://suzan.rbind.io/2018/01/dplyr-tutorial-1/
      * Filtering rows
        https://suzan.rbind.io/2018/02/dplyr-tutorial-3/
      * Summarizing and slicing https://suzan.rbind.io/2018/04/dplyr-tutorial-4/
  * Funny
    * Cowsay: https://cran.r-project.org/web/packages/cowsay/vignettes/cowsay_tutorial.html
      * Make animals say funny things (Yoda is my favorite)
    * Excel 2003 themed figures: https://cran.r-project.org/web/packages/ggthemes/vignettes/ggthemes.html
* Visualizations
  * Graphs and networks
    * DiagrammeR https://github.com/rich-iannone/DiagrammeR
  * Gantt charts
    * GanttR function: https://insileco.github.io/2017/09/20/gantt-charts-in-r/
    * Other options: https://stackoverflow.com/questions/3550341/gantt-charts-with-r
  * Interactive timelines
    * timevis: https://github.com/daattali/timevis
* Application-focused
  * Webscraping
    * http://www.interhacktives.com/2017/01/25/scrape-tweets-r-journalists/
    * http://utstat.toronto.edu/~nathan/teaching/sta4002/Class1/scrapingtwitterinR-NT.html
* Operations research
  * http://josilber.scripts.mit.edu/IAPEducationPaperDistribute.pdf

# GitHub
  * Beginner Tutorial: http://try.github.io/
  * Overview:
    * https://github.com/joshnh/Git-Commands
  * Markdown cheat sheet https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
  * Specifics (how to)
    * Undo: https://www.atlassian.com/git/tutorials/undoing-changes
    * Cloning: https://help.github.com/articles/cloning-a-repository/
    * Using cloned repo: https://stackoverflow.com/questions/14217406/why-i-cant-push-a-newly-cloned-repo
    * Save credentials (login):
    https://help.github.com/articles/caching-your-github-password-in-git/
  * Specifics (background)
    * What is a bare repository? http://www.saintsjd.com/2011/01/what-is-a-bare-git-repository/

# General coding practices
* Overview and slides from [@tommlogan](https://github.com/tommlogan): http://reckoningrisk.com/research-practice/2018/better-coding-practices/

# AMPL
* (Free) Book: https://ampl.com/resources/the-ampl-book/chapter-downloads/
* Google group (help forum): https://groups.google.com/forum/#!forum/ampl
* Specifics
  * Dynamic set definitions
    https://groups.google.com/forum/#!msg/ampl/Wr_KxvKWBpM/FGeILLXGZzAj
    * E.g., AVAIL vs. AVAIL_all


# Math programming software
* Solvers
  * Commercial
    * CPLEX (free for academics): https://www.ibm.com/products/ilog-cplex-optimization-studio
    * Gurobi (free for academics): http://www.gurobi.com/
    * Xpress: http://www.fico.com/en/products/fico-xpress-optimization
  * GLPK: https://www.gnu.org/software/glpk/
  * SCIP: http://scip.zib.de/
  * NEOS: https://neos-guide.org/
  * OpenSolver (free): https://opensolver.org/
    * Excel add-in (extends the standard Excel solver)
* Formulation
  * SolverStudio (free): http://solverstudio.org/
    * Excel add-in, useful when OpenSolver not big enough
    * Can call commercial solvers
  * AMPL: https://ampl.com/
  * OPL: https://www.ibm.com/analytics/data-science/prescriptive-analytics/optimization-modeling
* Test sets
  * MIPLIB: http://miplib.zib.de/
* List of solvers
  * Commercial: https://ampl.com/products/solvers/solvers-we-sell/
  * Free: https://ampl.com/products/solvers/open-source/
* Application specific
  * Facility location
    * SITATION: https://daskin.engin.umich.edu/software/
  * Agent-based
    * NetLogo: https://ccl.northwestern.edu/netlogo/

# Math programming textbooks
* (Free) _A First Course in Linear Optimization v3.0_ by [@jon77lee](https://github.com/jon77lee/): https://github.com/jon77lee/JLee_LinearOptimizationBook/blob/master/JLee.3.0.pdf
* (Free) _Foundations and Methods of Stochastic Simulation_  (Barry Nelson) http://users.iems.northwestern.edu/~nelsonb/IEMS435/

# Algorithms
* List/explanation from the folks at NEOS: https://neos-guide.org/algorithms

# Operations research-adjacent material
* Course lectures
  * Linear Algebra (Gilbert Strang): https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/
  * Intro Game Theory (Ben Polak): https://oyc.yale.edu/economics/econ-159

# Data visualization
* Textbooks
  * [@clauswilke](https://github.com/clauswilke): http://serialmentor.com/dataviz/
  * [@kjhealy](https://github.com/kjhealy): http://socviz.co/

# Datasets
* Network datasets
  * Compilation from [@kateto](https://github.com/kateto): http://kateto.net/2016/05/network-datasets/
  * Compilation from [@profjure](https://github.com/profjure): https://snap.stanford.edu/data/
* General Compilations
  * Kaggle: https://www.kaggle.com/datasets
  * Public data sources:
   https://blog.bigml.com/list-of-public-data-sources-fit-for-machine-learning/
    * Targeted towards machine learning
  * Google Public Data Explorer: https://www.google.com/publicdata/directory
  * Public datasets: https://github.com/awesomedata/awesome-public-datasets
* Specific sources
  * European statistics: http://ec.europa.eu/eurostat/data/database
  * IMF: http://www.imf.org/en/Data
  * WHO: http://www.who.int/gho/en/

# Math-y shortcuts
  * Linearize product of variables: https://www.leandro-coelho.com/linearization-product-variables/
  * Linearize max/max/absolute value: https://www.leandro-coelho.com/how-to-linearize-max-min-and-abs-functions/

# Communication / dissemination
* Reference software
  * Zotero: https://www.zotero.org/
  * Mendeley: https://www.mendeley.com/
  * EndNote: http://endnote.com/
* LaTeX
  * Example style template for journals https://www.leandro-coelho.com/default-latex-article-style-modifications/
* Manuscripts
  * Writing manuscripts (Healthcare-focused):
    * Welch, 1999 paper (Prepping for Submission to a Medical Journal)
     https://medicine.umich.edu/sites/default/files/content/downloads/Welch%20Manuscripts.pdf
    * Ibrahim and Dimick (Writing for Impact)
     https://medicine.umich.edu/sites/default/files/content/downloads/WritingResearchPaper_Ibrahim_0.pdf
    * Policy papers in clinical journals: https://sph.umich.edu/cehr/pdf/Manuscript_Guide.pdf
      * Writing guide from the UM Center for Evaluating Health Reform
  * Guide to running "paper sprints" https://sph.umich.edu/cehr/pdf/Paper_Sprint_Manual.pdf
    * I.e., getting a team together and writing a paper really fast
* Visual abstracts
  * https://static1.squarespace.com/static/5854aaa044024321a353bb0d/t/5a527aa89140b76bbfb2028a/1515354827682/VisualAbstract_Primer_v4_1.pdf
* Policy
  * (Blog) Connecting Research to Policy https://www.healthaffairs.org/do/10.1377/hblog20180403.254308/full/#.Ws43706twu0.twitter

# Healthcare
* Healthcare Industry guide (largely UM students only) https://kresgeguides.bus.umich.edu/healthcarebiotechhome
* Health management and policy guide
  * http://guides.lib.umich.edu/hmp
* Guide to finding health statistics
 * UM: http://guides.lib.umich.edu/healthstats
 * Wisconsin-Madison: http://researchguides.ebling.library.wisc.edu/c.php?g=293234

# Jobs
* Infectious disease dynamics listserv: http://iddjobs.org/jobs/

# Summer schools
* List compiled by Thiago Serra:
  * 2018 Version: https://thiagoserra.com/2018/01/28/summer-2018-schools-on-algorithms-combinatorics-data-science-machine-learning-optimization-and-other-relevant-orms-topics/

# Teaching
* Guidebook from UM CRLT: http://www.crlt.umich.edu/gsis/gsi_guide

# Website creation
* (Free) Hosted by github: https://pages.github.com/
  * Themes: https://github.com/topics/jekyll-theme
  * I use: https://github.com/academicpages/academicpages.github.io
  * Template for labs: http://www.allanlab.org/aboutwebsite.html
* (Free/Paid) Wix: https://www.wix.com
* (Free) Google Sites: https://sites.google.com/

# Blogs I like (and read occasionally)
* http://www.math3ma.com/
* https://punkrockor.com/
* https://chrisblattman.com/
  * His advice posts (links on right-hand side of blog) are interesting
* http://reckoningrisk.com/
* Humor
  * Math with Bad Drawings: https://mathwithbaddrawings.com/
  * Lego Grad Student: https://brickademics.com/


# Various advice
* For new grad students: https://medium.com/@dorsaamir/modest-advice-for-new-graduate-students-b0be6b8dbc22

# Eclectic
* CV of failures
  * https://www.princeton.edu/~joha/Johannes_Haushofer_CV_of_Failures.pdf
  *  https://www.washingtonpost.com/news/wonk/wp/2016/04/28/it-feels-really-good-to-read-about-this-princeton-professors-failures/?noredirect=on&utm_term=.c5a450e68610
* List of "awesome" lists https://github.com/sindresorhus/awesome
  * Very meta. But also potentially helpful.
* Guide to Bad Data
  * Github: https://github.com/Quartz/bad-data-guide
  * Article on Quartz: https://qz.com/572338/the-quartz-guide-to-bad-data/#user-content-there-are-inexplicable-outliers
* Testing: https://towardsdatascience.com/testing-to-learn-part-1-16a7968d2ba3
* Sites to poll meeting availability:
  * When2Meet: https://www.when2meet.com/
  * When is good: http://whenisgood.net/
* Humor
  * Top 10 Illegitimate Proof Techniques https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/lecture-3-strong-induction/MIT6_042JF10_proof.pdf
    * (I think the original version of this list came from Dana Angluin)

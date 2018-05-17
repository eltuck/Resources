# Resources

Consider this a public bookmark bar. These are resources I've found useful or think might be one day. Not comprehensive, links may not work, in no particular order.

### Python
* Overview
  * Whirlwind tour from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/WhirlwindTourOfPython
  * Overview from [@drvinceknight](https://github.com/drvinceknight): https://vknight.org/Introduction_to_OOP/OverviewOfPython/
* Textbooks
  * (Free) _Think Python_ by [@AllenDowney](https://github.com/AllenDowney) http://greenteapress.com/wp/think-python-2e/
    * Beginners guide, programming exp. not necessary
  * (Free) _Python Data Science Handbook_ by [@jakevdp](https://github.com/jakevdp) https://jakevdp.github.io/PythonDataScienceHandbook/
* Community
  * Slack channel to learn data science in Python: https://py4ds.slack.com
* Overall tutorial
  * Python Software Foundation: https://docs.python.org/3.6/tutorial/index.html
* Topics/packages
  * List of OR/MS-related packages: https://wiki.python.org/moin/PythonForOperationsResearch
  * Altair (visualizations)
    * Notebooks with example code: https://github.com/altair-viz/altair_notebooks
    * Video tutorial from [@jakevdp](https://github.com/jakevdp) https://www.youtube.com/watch?v=ms29ZPUKxbU&t=2431s
      * First ~40 min are a nice walkthrough; didn't watch the rest
  * Pandas (data processing)
    * Beginner tutorial from [@gjreda](https://github.com/gjreda) http://gregreda.com/2013/10/26/intro-to-pandas-data-structures/
    * Intermediate tutorial from [@tomaugspurger](https://github.com/tomaugspurger) http://tomaugspurger.github.io/modern-1-intro
  * NetworkX https://github.com/networkx/networkx
    * Tutorial: network analysis (humanities data) https://programminghistorian.org/lessons/exploring-and-analyzing-network-data-with-python
    * Tutorial: Chinese postman problem https://www.datacamp.com/community/tutorials/networkx-python-graph-tutorial
    * Network simplex https://networkx.github.io/documentation/networkx-1.9.1/reference/generated/networkx.algorithms.flow.network_simplex.html
  * Simulation
    * (Book chapter) by Barry Nelson: http://users.iems.northwestern.edu/~nelsonb/IEMS435/PythonSim.pdf
  * ML
      * Flowchart: choosing the right estimator: http://scikit-learn.org/stable/tutorial/machine_learning_map/
      * Sklearn tutorial from [@jakevdp](https://github.com/jakevdp): https://github.com/jakevdp/sklearn_tutorial
  * Supply chain
    * Supplychainpy: https://github.com/KevinFasusi/supplychainpy
* Figures
  * R-style graphing
    * plotnine package: https://plotnine.readthedocs.io/en/stable/
    * ggplot package: https://www.r-bloggers.com/ggplot2-style-plotting-in-python/
  * Funny
    * XKCD-style figures: https://matplotlib.org/xkcd/examples/showcase/xkcd.html

### R
* Textbooks
  * (Free) _R for Data Science_ by [@hadley](https://github.com/hadley/) and [@garrettgman](https://github.com/garrettgman)
https://r4ds.had.co.nz/
  * (Free) _Text Mining with R_ by [@juliasilge](https://github.com/juliasilge) and [@dgrtwo](https://github.com/dgrtwo/) https://www.tidytextmining.com/
* Learn R
  * Community to walk through _R for Data Science_ book together: https://medium.com/@kierisi/r4ds-the-next-iteration-d51e0a1b0b82
  * Tidy Tuesdays - a weekly data viz project https://github.com/rfordatascience/tidytuesday/blob/master/README.md
  * Collection of tutorials
    * UC Business Analytics: http://uc-r.github.io/
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
* Markdown/reports
  * Tufte style for markdown: https://github.com/rstudio/tufte
* Tutorials
  * Webscraping
    * http://www.interhacktives.com/2017/01/25/scrape-tweets-r-journalists/
    * http://utstat.toronto.edu/~nathan/teaching/sta4002/Class1/scrapingtwitterinR-NT.html
  * K-means
    * https://uc-r.github.io/kmeans_clustering
* Operations research
  * Using R for OR: http://josilber.scripts.mit.edu/IAPEducationPaperDistribute.pdf
  * Optplot from [@dirkschumacher](https://github.com/dirkschumacher): https://github.com/dirkschumacher/optplot
    * Plot optimization models
* How to...
  * Rearrange categories in a plot https://trinkerrstuff.wordpress.com/2012/10/15/how-do-i-re-arrange-ordering-a-plot/
  * Save high resolution figures: https://www.r-bloggers.com/high-resolution-graphics-with-r/
  * Iteratively make plots by [@dpananos](https://github.com/Dpananos) https://dpananos.github.io/posts/2018/04/blog-post-8/
  * Fit distributions: http://www.di.fc.ul.pt/~jpn/r/distributions/fitting.html
  * Write an R package by [@jtleek](https://github.com/jtleek): https://github.com/jtleek/rpackages

### GitHub
  * Beginner Tutorial: http://try.github.io/
  * Guide to Git with R: http://happygitwithr.com/
    * Haven't read it but heard it's a good one
  * Overview:
    * https://github.com/joshnh/Git-Commands
  * Cheat sheets
    * Overall: https://chrisalbon.com/software_engineering/cloud_computing/github_cheatsheet/
    * Markdown: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
  * How to...
    * Undo: https://www.atlassian.com/git/tutorials/undoing-changes
    * Clone a repo: https://help.github.com/articles/cloning-a-repository/
    * Use cloned repo: https://stackoverflow.com/questions/14217406/why-i-cant-push-a-newly-cloned-repo
    * Save credentials (i.e., username/password):
    https://help.github.com/articles/caching-your-github-password-in-git/
  * Specifics (background)
    * What is a bare repository? http://www.saintsjd.com/2011/01/what-is-a-bare-git-repository/

### General coding practices
* Overview and slides from [@tommlogan](https://github.com/tommlogan): http://reckoningrisk.com/research-practice/2018/better-coding-practices/
* Best practices from [@marcio-mourao](https://github.com/marcio-mourao): https://rawgit.com/marcio-mourao/Programming-Best-Practices/master/Workshop.html

### AMPL
* (Free) Book: https://ampl.com/resources/the-ampl-book/chapter-downloads/
* Google group (help forum): https://groups.google.com/forum/#!forum/ampl
* Specifics
  * Dynamic set definitions
    https://groups.google.com/forum/#!msg/ampl/Wr_KxvKWBpM/FGeILLXGZzAj
    * E.g., AVAIL vs. AVAIL_all


### Math programming software
* Solvers
  * Commercial
    * CPLEX (free for academics): https://www.ibm.com/products/ilog-cplex-optimization-studio
    * Gurobi (free for academics): http://www.gurobi.com/
    * Xpress:
      * http://www.fico.com/en/products/fico-xpress-optimization
      * https://community.fico.com/community/fico-optimization-community
    * MOSEK: https://www.mosek.com/
      * Esp. SOCP, SDP
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

### Math programming resources
* Free Textbooks
  * _A First Course in Linear Optimization v3.0_ by [@jon77lee](https://github.com/jon77lee/): https://github.com/jon77lee/JLee_LinearOptimizationBook/blob/master/JLee.3.0.pdf
  * _Foundations and Methods of Stochastic Simulation_  (Barry Nelson) http://users.iems.northwestern.edu/~nelsonb/IEMS435/
  * _MOSEK Modeling Cookbook_ https://themosekblog.blogspot.dk/2018/05/new-modeling-cookbook.html
    * Conic optimization, not specific to MOSEK solver
* Communities / forums
  * OR Exchange: https://www.or-exchange.org/
  * Stack Overflow: https://stackoverflow.com/
* Algorithms
  * List/explanation from the folks at NEOS: https://neos-guide.org/algorithms
* Models
  * GAMS model library: https://www.gams.com/latest/gamslib_ml/libhtml/
* Course resources
  * Intro to Math Programming - lecture notes (grad level taught by Dimitris Bertsimas in Fall 2009): https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-251j-introduction-to-mathematical-programming-fall-2009/lecture-notes/
  * Stochastic Optimization - readings (grad level taught by Warren Powell in Fall 2017): https://castlelab.princeton.edu/orf-544/
  * Optimal Learning - various materials (Warren Powell): http://optimallearning.princeton.edu/
* Other
  * IFORS Developing Countries page: http://ifors.org/developing_countries/index.php?title=Main_Page
    * A variety of open-source resources
* Drawing scenario trees
  * GAMS/SCENRED https://www.gams.com/latest/docs/T_SCENRED.html
    * Workshop: https://www.gams.com/fileadmin/community/contrib/financial/ngk_scenred.pdf
    * Presentation: http://old.gams.com/presentations/present_informs08_scenred.pdf
  * Plotly (python): https://plot.ly/python/tree-plots/
  * Graphviz (python): http://graphviz.readthedocs.io/en/stable/index.html
    * Examples: http://graphviz.readthedocs.io/en/stable/examples.html
  * Networkx (python): https://networkx.github.io/
  * Force-directed graph (json/html): https://bl.ocks.org/mbostock/4062045
* How to...
  * Linearize product of variables: https://www.leandro-coelho.com/linearization-product-variables/
  * Linearize max/max/absolute value: https://www.leandro-coelho.com/how-to-linearize-max-min-and-abs-functions/

### Operations research-adjacent material
* Linear Algebra
  * Intro course lectures from Gilbert Strang: https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/
* Game theory
  * Intro course lectures from Ben Polak: https://oyc.yale.edu/economics/econ-159
* Data Science
  * How to get started - blog post by [@kierisi](https://github.com/kierisi): https://www.jessemaegan.com/post/data-science-with-r-how-do-i-start/
  * Applied data science course readings from [@hadley](https://github.com/hadley/) https://github.com/hadley/stats337#readings
  * Technical notes - ML and AI from [@chrisalbon](https://github.com/chrisalbon)
    * Website: https://chrisalbon.com/#machine_learning
    * On github: https://github.com/chrisalbon/notes
  * ML flashcards from [@chrisalbon](https://github.com/chrisalbon)
    * https://machinelearningflashcards.com/
    * Scrape off Twitter for free, code from [@Dpananos](https://github.com/Dpananos): https://github.com/Dpananos/GetCards
  * Applied ML course [@amueller](https://github.com/amueller): http://www.cs.columbia.edu/~amueller/comsw4995s18/schedule/
    * Includes lecture recordings and slides
  * Directory of lots of data science material: http://www.datasciguide.com/content/

### Data visualization
* Textbooks
  * _Fundamentals of Data Visualization_ by [@clauswilke](https://github.com/clauswilke): http://serialmentor.com/dataviz/
  * _Data Visualization: A Practical Introduction_ by [@kjhealy](https://github.com/kjhealy): http://socviz.co/
* Networks
  * Gephi: https://gephi.org/

### Datasets / databases
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
* Literature
  * PubMed: https://www.ncbi.nlm.nih.gov/pubmed/
  * Scopus: https://www.scopus.com/search/form.uri?display=basic
  * Web of Science: https://clarivate.com/products/web-of-science/web-science-form/web-science-core-collection/
  * Embase: https://www.elsevier.com/solutions/embase-biomedical-research
  * CENTRAL (Cochrane reviews) http://www.cochranelibrary.com/about/central-landing-page.html
  * Google Scholar: https://scholar.google.com/

### Communication / dissemination / manuscripts
* Sharing data (guide by [@jtleek](https://github.com/jtleek)): https://github.com/jtleek/datasharing
* Reference software
  * Zotero: https://www.zotero.org/
  * Mendeley: https://www.mendeley.com/
  * EndNote: http://endnote.com/
* LaTeX
  * Example style template for journals https://www.leandro-coelho.com/default-latex-article-style-modifications/
  * Thesis templates:
    * U Wolverhamptom: https://github.com/snim2/phdtemplate
    * Michigan: http://clasp.engin.umich.edu/pages/current/dissertation-template
  * Beamer tips and tricks by [@paulgp](https://github.com/paulgp)
    * Presentation: https://github.com/paulgp/beamer-tips/blob/master/slides.pdf
    * Source code: https://github.com/paulgp/beamer-tips
* Manuscripts
  * How to write your first paper (guide by [@jtleek](https://github.com/jtleek)): https://github.com/jtleek/firstpaper
    * Biostatistician
  * Writing manuscripts (Healthcare-focused):
    * Welch, 1999 paper (Prepping for Submission to a Medical Journal)
     https://medicine.umich.edu/sites/default/files/content/downloads/Welch%20Manuscripts.pdf
    * Ibrahim and Dimick (Writing for Impact)
     https://medicine.umich.edu/sites/default/files/content/downloads/WritingResearchPaper_Ibrahim_0.pdf
    * Policy papers in clinical journals: https://sph.umich.edu/cehr/pdf/Manuscript_Guide.pdf
      * Writing guide from the UM Center for Evaluating Health Reform
  * Guide to running "paper sprints" https://sph.umich.edu/cehr/pdf/Paper_Sprint_Manual.pdf
    * I.e., getting a team together and writing a paper really fast
  * How to review a paper by [@jtleek](https://github.com/jtleek) https://github.com/jtleek/reviews
    * Biostatistician
* Visual abstracts
  * https://static1.squarespace.com/static/5854aaa044024321a353bb0d/t/5a527aa89140b76bbfb2028a/1515354827682/VisualAbstract_Primer_v4_1.pdf
* Policy
  * (Blog) Connecting Research to Policy https://www.healthaffairs.org/do/10.1377/hblog20180403.254308/full/#.Ws43706twu0.twitter
* More than a press release (Videos): https://theincidentaleconomist.com/wordpress/a-press-release-is-not-enough-videos/

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
  * Private
    * IQVIA (formerly IMS Health): https://www.iqvia.com/solutions/real-world-value-and-outcomes/realworld-data
      * Considered the gold standard for volume data but expensive
  * Other
    * Clinical trials: https://clinicaltrials.gov/
    * Link to CDC data/stats: https://www.cdc.gov/DataStatistics/
  * Major surveys
    * NHANES (in person): https://www.cdc.gov/nchs/nhanes/index.htm
    * BRFSS (phone): https://www.cdc.gov/brfss/annual_data/annual_data.htm
      * Pronounced "Burfiss"
    * Census: https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml
      * Not really healthcare but still useful
* Newsletters
  * CDC's MMWR: https://www.cdc.gov/mmwr/index.html
    * Morbidity and Mortality Weekly Report
    * I think most people I know working in public health subscribe to this

### Jobs / Summer schools
* Jobs
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
* Summer schools
  * List compiled by Thiago Serra (2018 Version):  https://thiagoserra.com/2018/01/28/summer-2018-schools-on-algorithms-combinatorics-data-science-machine-learning-optimization-and-other-relevant-orms-topics/
* Career prep
  * Questions to think through career goals [@benlangmead](https://github.com/benlangmead): https://github.com/BenLangmead/langmead-lab/blob/master/postdoc_questionnaire.md
    * Slightly expanded from [@jtleek](https://github.com/jtleek): https://github.com/jtleek/careerplanning
  * Academic jobs
    * Tons of resources compiled by UM CRLT: http://crlt.umich.edu/PFF_Resources

### Grants/fellowships
* FDA Generic Drug-related: https://www.fda.gov/Drugs/ResourcesForYou/Consumers/BuyingUsingMedicineSafely/GenericDrugs/ucm585566.htm

### Teaching
* Guidebook from UM CRLT: http://www.crlt.umich.edu/gsis/gsi_guide

### Websites
* Sites
  * (Free) Hosted by github: https://pages.github.com/
    * Themes: https://github.com/topics/jekyll-theme
      * Simple one for academics https://github.com/academicpages/academicpages.github.io
    * Template for labs: http://www.allanlab.org/aboutwebsite.html
  * (Free/Paid) Wix: https://www.wix.com
  * (Free) Google Sites: https://sites.google.com/
* Resources
  * Icons: https://www.iconsdb.com/
    * E.g., the Google Scholar logo

### Blogs I like (and read occasionally)
* http://www.math3ma.com/
* https://punkrockor.com/
* http://reckoningrisk.com/
* Humor
  * Math with Bad Drawings: https://mathwithbaddrawings.com/
  * Lego Grad Student: https://brickademics.com/

### Various advice
* Grad students
  * For new grad students: https://medium.com/@dorsaamir/modest-advice-for-new-graduate-students-b0be6b8dbc22
  * Advisor/PhD student dynamics: https://chroniclevitae.com/news/1793-handling-your-imperfect-adviser
* Various
  * An econ prof (Hal Varian) describes his work style: http://people.ischool.berkeley.edu/~hal/Papers/how.pdf
  * Various advice posts on Chris Blattman's blog (econ prof) https://chrisblattman.com/
    * Links on right-hand side of blog
  * When your data science project doesn't work: https://medium.com/@skyetetra/so-your-data-science-project-isnt-working-7bf57e3f12f1
* Skills
  * Reading papers by [@jtleek](https://github.com/jtleek): https://github.com/jtleek/readingpapers

### Eclectic
* CV of failures
  * https://www.princeton.edu/~joha/Johannes_Haushofer_CV_of_Failures.pdf
  *  https://www.washingtonpost.com/news/wonk/wp/2016/04/28/it-feels-really-good-to-read-about-this-princeton-professors-failures/?noredirect=on&utm_term=.c5a450e68610
* List of "awesome" lists https://github.com/sindresorhus/awesome
  * Very meta. But also potentially helpful.
* Guide to Bad Data
  * Github: https://github.com/Quartz/bad-data-guide
  * Article on Quartz: https://qz.com/572338/the-quartz-guide-to-bad-data/#user-content-there-are-inexplicable-outliers
* Technical / scientific debt: http://varianceexplained.org/r/scientific-debt/
   * Interesting take from [@dgrtwo](https://github.com/dgrtwo) on managing shortcuts/assumptions/etc. in the project development process
* Testing: https://towardsdatascience.com/testing-to-learn-part-1-16a7968d2ba3
* Debugging
  * Rubber ducky method: https://rubberduckdebugging.com/
    * Explain in detail to an inanimate object
  * Wolf-fence algorithm: http://coreygoldberg.blogspot.com/2008/12/wolf-fence-debugging.html
    * Basically binary search with fun description
    * Original paper (paywall): https://dl.acm.org/citation.cfm?id=358695
* Sites to poll meeting availability:
  * When2Meet: https://www.when2meet.com/
  * When is good: http://whenisgood.net/
* Fun OR applications
  * 2048 using MDPs [@jdleesmiller](https://github.com/jdleesmiller): http://jdlm.info/articles/2018/03/18/markov-decision-process-2048.html
  * Chutes & Ladders as a Markov chain [@jakevdp](https://github.com/jakevdp): https://jakevdp.github.io/blog/2017/12/18/simulating-chutes-and-ladders/#Fundamental-Matrix
* Humor
  * Top 10 Illegitimate Proof Techniques https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/lecture-3-strong-induction/MIT6_042JF10_proof.pdf
    * (I think the original version of this list came from Dana Angluin)
  * "The best way to write secure and reliable applications" https://github.com/kelseyhightower/nocode
  * Add coffee stains to your LaTeX files: http://hanno-rein.de/archives/349
  * Guide to interpreting faculty feedback: https://kieranhealy.org/blog/archives/2013/08/16/academic-feedback/

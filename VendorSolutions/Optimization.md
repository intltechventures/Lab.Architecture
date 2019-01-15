
Optimization Solution Resources
====

### Gurobi
* https://www.gurobi.com/
  * https://www.gurobi.com/resources/examples/example-models-overview
  * https://www.crunchbase.com/organization/gurobi-optimization#section-overview
  * https://en.wikipedia.org/wiki/Gurobi
* Documentation
  * http://www.gurobi.com/documentation/
  * https://www.gurobi.com/documentation/8.1/examples/examples.html
* Tutorials, Resources, Articles
  * https://www.gurobi.com/resources/examples/example-models-overview
  * http://www.gurobi.com/resources/seminars-and-videos/seminars-videos
  * ArchLinux
    * https://aur.archlinux.org/packages/gurobi/
  * MVNRepository
    * https://mvnrepository.com/artifact/gurobi
  * C#
    * https://www.gurobi.com/documentation/8.1/examples/cs_examples.html
  * C++
    * https://www.gurobi.com/documentation/8.1/examples/cpp_examples.html
    * https://www.leandro-coelho.com/how-to-compile-c-with-gurobi-in-linux/
  * Java
    * https://www.gurobi.com/documentation/8.1/examples/java_examples.html
  * Julia
    * https://discourse.julialang.org/search?q=gurobi
    * https://github.com/JuliaOpt/Gurobi.jl
      * This package is a wrapper of the Gurobi solver (through its C interface). Currently, this package supports the following types of problems (KM: as of 2019-01-15):
        * Linear programming (LP)
        * Mixed Integer Linear Programming (MILP)
        * Quadratic programming (QP)
        * Mixed Integer Quadratic Programming (MIQP)
        * Quadratically constrained quadratic programming (QCQP)
        * Second order cone programming (SOCP)
        * Mixed integer second order cone programming (MISOCP)
  * R
    * https://www.gurobi.com/documentation/8.1/examples/r_examples.html
    * https://cran.r-project.org/web/packages/prioritizr/vignettes/gurobi_installation.html
  * Rust
    * https://docs.rs/gurobi/0.3.3/gurobi/
  * Python
    * https://www.gurobi.com/documentation/8.1/examples/python_examples.html
    * https://anaconda.org/search?q=gurobi
      * https://anaconda.org/Gurobi/gurobi
    * [Optimization Modeling in Python: PuLp, Gurobi, and CPLEX](https://medium.com/opex-analytics/optimization-modeling-in-python-pulp-gurobi-and-cplex-83a62129807a)
    * [Python III Webinar, Optimization and Heuristics](http://www.gurobi.com/resources/seminars-and-videos/python-III-webinar)
  * YouTube Channel: GurobiVideos    
    [Getting Started with Gurobi part 1 of 3](https://www.youtube.com/watch?v=oBTJNRXyUu0)
    [Getting Started with Gurobi part 2 of 3](https://www.youtube.com/watch?v=O0_ZPT2pd-M)
    [Getting Started with Gurobi part 3 of 3](https://www.youtube.com/watch?v=BtNWKb2Y_08)
  * COMP331/557: Optimization, Introduction to Gurobi
    * http://cgi.csc.liv.ac.uk/~gairing/COMP557/slides/gurobi.pdf
* Community Forums
  * https://groups.google.com/forum/#!forum/gurobi
* Releases
  * 8.1
    * http://www.gurobi.com/products/whats-new/whats-new-in-the-latest-version?mkt_tok=eyJpIjoiTUdWbU9HVmlZbUU0Tm1KaiIsInQiOiJvUW1jRkdJcWR0akVxUk5BYm5JY1NVdHlEN1hKTzNmRSs5d3JMaUg2Y0ZaZ2poUVwveFRiTGY1Ukg3S0QrOUxQRnI5U2VUMmxjWjJGZEJycWpBYkNYbHZRS1p4eE9uUnhoSjNlTjVZcEROeUpOQ3pnellxKzdVMUdveEh0cUhDcHoifQ%3D%3D
    * http://yetanothermathprogrammingconsultant.blogspot.com/2018/10/gurobi-81.html
      * re: MIQP, "More than a factor of 6x faster on difficult models that take more than 100 seconds to solve."
* Third-Party Products
  * SOlverStudio: Excel Integration
    * https://solverstudio.org/languages/gurobi/
    * "SolverStudio allows you to build models inside Excel using Gurobi’s Python modelling language. SolverStudio manages all the access to data on the spreadsheet, making it easy to build and run models within Excel."
* News
  * https://twitter.com/gurobi?lang=en
  * 2018
    * https://www.pehub.com/2018/01/thompson-street-invests-in-gurobi-optimization/#
  * 2017
    * https://www.tscp.com/press-release/thompson-street-capital-partners-recapitalizes-gurobi-optimization/


### SOlverStudio
* https://solverstudio.org/
* SolverStudio is an add-in for Excel 2007 and later on Windows that allows you to build and solve optimisation models in Excel using any of the following optimisation modelling languages:
  * PuLP, an open-source Python-based COIN-OR modelling language developed by Stu Mitchell. PuLP is included with SolverStudio.
  * COOPR/Pyomo, an open source COIN-OR modelling language for Python which extends Pulp with abstract models, support for stochastic programming, and a larger range of solvers.
  * AMPL, a commercial modelling language. SolverStudio either requires AMPL to be installed by the user, or can automatically install a free “demo” version of AMPL.  (The
    Demo comes with 11 solvers; AMPL’s variable/constraint limits are 500 for linear and 300 for nonlinear, though 4 of the solvers are limited to 10.) We have a tutorial on using AMPL with SolverStudio. We also support running AMPL models in the cloud using the excellent NEOS server; see AMPL on NEOS. See our SolverStudio AMPL page for more information.
  * GMPL (GNU MathProg Language), an open source AMPL look-alike developed as part of GLPK (GNU Linear Programming Kit). GMPL is included with SolverStudio.
  * GAMS, a commercial modelling language. SolverStudio requires GAMS to be installed by the user. GAMS provide a free trial version. Support for solving GAMS models using the NEOS server is working in our new beta version.
  * Gurobi, a commercial solver which can be accessed from SolverStudio using the Gurobi Python modelling interface. This requires the Gurobi solver be installed. SolverStudio provides a license manager to help manage Gurobi licenses.
  * CMPL, an open source COIN-OR  modelling language that also includes a remote server for solving on external computers. Also available from Python.
  * SimPy, an open source Python simulation language, which is now included with the SolverStudio download.
  * Any other Python software that runs under either IronPython or standard Python (i.e ‘CPython‘). IronPython comes built in, while the user needs to install their own choice of CPython.
  * We hope to add Zimpl in the near future, and allow GMPL to be used with CBC.



### Interesting Articles
* 2018
  * https://medium.com/opex-analytics/optimization-modeling-in-python-pulp-gurobi-and-cplex-83a62129807a


### Academic Research
* Hans D. Mittleman, Ph.D., School of Mathematical and Statistical Sciences, ASU
  * http://plato.asu.edu/
  * http://plato.asu.edu/guide.html
* Leandro C. Coelho, Ph.D., Canada Research Chair in Integrated Logistics, Operations and Decision Systems Department, Faculty of Administration Sciences
Université Laval, Québec, Canada,
  * https://www.leandro-coelho.com/
  * https://twitter.com/leandro_cc




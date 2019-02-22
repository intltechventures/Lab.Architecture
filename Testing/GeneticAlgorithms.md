
Resources for Genetic Algorithms to Auto-Generate Test Cases (and/or Test Data)
====

### Background Reading
* 2017
  * [Genetic Algorithm Approach For Test Case Generation Randomly: A Review](https://www.researchgate.net/publication/320038807_Genetic_Algorithm_Approach_For_Test_Case_Generation_Randomly_A_Review)
    * International Journal of Computer Trends and Technology (IJCTT) – Volume 49 Number 4 July 2017
    * Abstract: "The quality of software is dependent  on testing as per user specifications and requirements. So  it  is quite  challenging  to  design,  prioritize and optimize  test  cases  to  achieve  quality.  Different testing tools can be used for software testing either manually or automatically. During the recent studies it is found that automated software testing is better than manual testing by using heuristic search. In this paper  presents  a  survey  on  genetic  algorithm approach  for  random  generation  of  test  cases  in functional software testing"
    * "Likelihood,  close  to  Boundary  Value  and  Branch Coverage are essential factors for a fitness function. Selection methods are of six different types such as roulette wheel, stochastic universal sampling, linear rank,  exponential  rank,  binary  tournament  and truncation."

  * [Path-oriented test cases generation based adaptive genetic algorithm](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0187471)
    * Authors: Xiaoan Bao, Zijian Xiong, Na Zhang , Junyan Qian, Biao Wu, Wei Zhang
    * Abstract: "The automatic generation of test cases oriented paths in an effective manner is a challenging problem for structural testing of software. The use of search-based optimization methods, such as genetic algorithms (GAs), has been proposed to handle this problem. This paper proposes an improved adaptive genetic algorithm (IAGA) for test cases generation by maintaining population diversity. It uses adaptive crossover rate and mutation rate in dynamic adjustment according to the differences between individual similarity and fitness values, which enhances the exploitation of searching global optimum. This novel approach is experimented and tested on a benchmark and six industrial programs. The experimental results confirm that the proposed method is efficient in generating test cases for path coverage."

* 2013 
  * [Automatic Test Case Generation Using Genetic Algorithm](https://ijser.org/researchpaper/Automatic-Test-Case-Generation-Using-Genetic-Algorithm.pdf)
    * International Journal of Scientific & Engineering Research, Volume 4, Issue 6, June-2013 
    * Abstract: " Software testing is most effort consuming phase in software development. One would like to minimize the efforts and maximize
the number of faults detected. Hence test case generation may be treated as an optimization problem. One of the major difficulties in sftware testing is the automatic generation of test data that satisfy a given adequacy criterion. Generating test cases automatically will reduce cost and efforts significantly. In this paper, test case data is generated automatically using Genetic Algorithms and results are compared with Random Testing. It is observed that Genetic Algorithms outperforms Random Testing."
    * "Boundary value analysis focuses on the boundary of the input space to identify test cases. So the basic idea is to select five values, minimum, just above the minimum, nominal value, just below the maximum and the maximum. So the test case values lying for Boundary value analysis are shown in Figure 3."


* 2012
  * [Automatic test case generation based on genetic algorithm and mutation analysis](https://ieeexplore.ieee.org/document/6487127)
    * Abstract: "This paper proposes a method that automatically generates software test cases based on a genetic algorithm and mutation analysis. Our method combines random generation and refinement. Each test case is generated randomly in the first step, and then a set of test cases is refined by the genetic algorithm. To measure the adequacy of the test case set, we use mutation scores, which are based on the mutation analysis of software testing. Our proposed method, which is applied to a C programing language program, automatically generated test case sets with 100% branch and boundary value coverages. The generation time of one test case set was approximately 130 ms"

  * [Automatic Test Case Generation using Genetic Algorithm with Antirandom Population](https://pdfs.semanticscholar.org/659f/08350460d7fc9bb459447ba94dbaed6eb764.pdf)
    * IJACE • January-June 2012 • Volume 5 • Issue 1
      * Authors: Kulvinder SINGH, , Iqbal KAUR, and Rakesh KUMAR
      * Abstract: "Reliability is a most important quality attribute of software which is to be achieved thorough software testing, the most effort consuming activity, success of which depends upon the adequacy of the data and all the criteria discussed in the literature are incomplete. There is the need of automatic test case generation so that the cost of testing can be reduced. In this research paper, Genetic Algorithm is used to automatically generate the test cases using the antirandom testing technique and the results are verified using n-versions of the module. Mutation adequacy is used to verify the completeness. The results of the Genetic Algorithm with random population and hamming code
are compared and improvements have been observed over random and hamming code testing."
    * "In N-version programming, the software module is implemented in a number of different versions by different teams, using common specification. These versions are executed in parallel. There outputs are compared using a voting system and inconsistent outputs are rejected. At least three versions of the module should be available. The assumption is that it is unlikely that different teams will make the same design or programming errors. [7, 8] describes this approach as fault avoidance. In Back-to-back testing, using lessons learned from N-version programming, [9] and [10] have suggested that that N version of the software be developed even when only a single version will be used.
      * KM Commentary: ```In what universe, other than space exploration, nuclear engineering, medical procedures - or other critical life-or-death businesses is it feasible to justify implementing three variations of the same solution?```
    * "The proposed technique using GA with antirandom population and employing n-version testing has shown the average 20% and maximum 40% improvement over the random test case generation."
    * "Although the cost incurred in producing N versions of the same module will be large but by using the technique judiciously in those modules only where a high level of reliability is required, the benefits accrued override the cost incurred."
      * KM Commentary: ```Where is the data and anlaysis to support this opinion, statd as fact?```

* 2010
  * [Using genetic algorithms for test case generation and selection optimization, Izzat Alsmadi](https://ieeexplore.ieee.org/document/5575262)
    * Abstract: "Genetic Algorithms (GAs) are adaptive search techniques that imitate the processes of evolution to solve optimization problems when traditional methods are considered too costly in terms of processing time and output effectiveness. In This research, we will use the concept of genetic algorithms to optimize the generation of test cases from the application user interfaces. This is accomplished through encoding the location of each control in the GUI graph to be uniquely represented and forming the GUI controls' graph. After generating a test case, the binary sequence of its controls is saved to be compared with future sequences. This is implemented to ensure that the algorithm will generate a unique test case or path through the GUI flow graph every time"


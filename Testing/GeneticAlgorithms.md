
Resources for Genetic Algorithms to Auto-Generate Test Cases (and/or Test Data)
====

### TO-DO
* Add DOI citation to each academic paper entry
* Organize academic papers, within year, by publication date, in descending order



### Background Reading
* https://en.wikipedia.org/wiki/Genetic_algorithm
  * "In computer science and operations research, a genetic algorithm (GA) is a metaheuristic inspired by the process of natural selection that belongs to the larger class of evolutionary algorithms (EA). Genetic algorithms are commonly used to generate high-quality solutions to optimization and search problems by relying on bio-inspired operators such as mutation, crossover and selection.[1] John Holland introduced genetic algorithms in 1960 based on the concept of Darwin’s theory of evolution; afterwards, his student Goldberg extended GA in 1989.[2]"

* https://en.wikipedia.org/wiki/Evolutionary_algorithm
  * "In artificial intelligence, an evolutionary algorithm (EA) is a subset of evolutionary computation,[1] a generic population-based metaheuristic optimization algorithm. An EA uses mechanisms inspired by biological evolution, such as reproduction, mutation, recombination, and selection. Candidate solutions to the optimization problem play the role of individuals in a population, and the fitness function determines the quality of the solutions (see also loss function). Evolution of the population then takes place after the repeated application of the above operators."
  * "Evolutionary algorithms often perform well approximating solutions to all types of problems because they ideally do not make any assumption about the underlying fitness landscape. Techniques from evolutionary algorithms applied to the modeling of biological evolution are generally limited to explorations of microevolutionary processes and planning models based upon cellular processes. In most real applications of EAs, computational complexity is a prohibiting factor.[2] In fact, this computational complexity is due to fitness function evaluation. Fitness approximation is one of the solutions to overcome this difficulty. However, seemingly simple EA can solve often complex problems[citation needed]; therefore, there may be no direct link between algorithm complexity and problem complexity."

* https://en.wikipedia.org/wiki/All-pairs_testing
  * "Using carefully chosen test vectors, this can be done much faster than an exhaustive search of all combinations of all parameters, by "parallelizing" the tests of parameter pairs."

* https://en.wikipedia.org/wiki/Orthogonal_array_testing
  * "Orthogonal array testing is a black box testing technique that is a systematic, statistical way of software testing.[1][2] It is used when the number of inputs to the system is relatively small, but too large to allow for exhaustive testing of every possible input to the systems.[1] It is particularly effective in finding errors associated with faulty logic within computer software systems.[1] Orthogonal arrays can be applied in user interface testing, system testing, regression testing, configuration testing and performance testing. The permutations of factor levels comprising a single treatment are so chosen that their responses are uncorrelated and therefore each treatment gives a unique piece of information. *```The net effects of organizing the experiment in such treatments is that the same piece of information is gathered in the minimum number of experiments```*."
  * "Testing cycle time is reduced and analysis is simpler."
  * "Test cases are balanced, so it's straightforward to isolate defects and assess performance. This provides a significant cost savings over pair-wise testing."



### Software Libraries/Frameworks (TBD...)
* C/C++
* C#
* Java
* JavaScript
* Python
* R



### Interesting Githoub Resources
* TBD...



### Background Reading, Academic Papers: Still need to read, select, sort & organize 
* Path-oriented test cases generation based adaptive genetic algorithm
  * https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0187471
* A Review of Random Test Case Generation using Genetic Algorithm
  * http://www.indjst.org/index.php/indjst/article/viewFile/107654/81470
* Path Coverage Test Case Generation Using Genetic Algorithms
  * http://journal.utem.edu.my/index.php/jtec/article/viewFile/2230/1348
* Test Data Generation Using Genetic Algorithms
  * https://www.cc.gatech.edu/~harrold/6340/cs6340_fall2009/Readings/pga.pdf
* Optimization of Test Case Generation using Genetic Algorithm (GA)
  * https://arxiv.org/ftp/arxiv/papers/1612/1612.08813.pdf
* Efficient Software Test Case Generation Using Genetic Algorithm Based Graph Theory
  * https://dl.acm.org/citation.cfm?id=1445617
* Genetic Algorithm-Based Test Data Generation for Multiple Paths via Individual Sharing
  * https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4323069/
* Automatic Generation of Test Case based on GATS Algorithm
  * https://www.computer.org/csdl/proceedings/grc/2009/4830/00/05255070.pdf
* Generating Test Case for Object-Oriented Software Using Genetic Algorithm and Mutation Testing Method
  * https://econpapers.repec.org/article/iggjamc00/v_3a3_3ay_3a2012_3ai_3a1_3ap_3a15-23.htm
* An Empirical Evaluation of Evolutionary Algorithms for Unit Test Suite Generation
  * http://www.evosuite.org/wp-content/uploads/2018/07/INFSOF_2017_336_Original_V1.pdf



### Background Reading, Academic Papers
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

  * [Generating Test Case for Object-Oriented Software Using Genetic Algorithm and Mutation Testing Method](https://www.igi-global.com/article/generating-test-case-object-oriented/64641)
    * Authors: Yamina Mohamed Ben Ali (University of Badji Mokhtar, Algeria) and Fatma Benmaiza (University of Badji Mokhtar, Algeria)
    * International Journal of Applied Metaheuristic Computing (IJAMC) 3(1)
    * Abstract "This paper presents an automatic creation of software test cases based on the use of a genetic algorithm and a mutation testing technique. The aim of this work is then the optimization of a score function in order to give the best set of optimal test case needed for testing an oriented-object program. Therefore, the proposed search-based approach generates in a first time a set of mutants according to an input program for testing the output of methods belonging in the tested class. On the second time, the output of the mutants and the input program are compared to evaluate the performance of all chromosomes in the genetic population. Finally, at the end of the chromosomes evolution the best test case in retrieved as the optimal one"


* 2011
  * [Generation of Test Data and Test Cases for Software Testing: A Genetic Algorithm Approach (PH.D Research Plan Proposal](https://shodhgangotri.inflibnet.ac.in/bitstream/123456789/1984/1/shveta%20parnami_rpp_generation%20of%20test%20data%20and%20test%20cases%20for%20software%20testing%20a%20genetic%20algorithm%20appro.pdf)
    * Author: Shveta Parnami
    * 

* 2010
  * [Using genetic algorithms for test case generation and selection optimization, Izzat Alsmadi](https://ieeexplore.ieee.org/document/5575262)
    * Abstract: "Genetic Algorithms (GAs) are adaptive search techniques that imitate the processes of evolution to solve optimization problems when traditional methods are considered too costly in terms of processing time and output effectiveness. In This research, we will use the concept of genetic algorithms to optimize the generation of test cases from the application user interfaces. This is accomplished through encoding the location of each control in the GUI graph to be uniquely represented and forming the GUI controls' graph. After generating a test case, the binary sequence of its controls is saved to be compared with future sequences. This is implemented to ensure that the algorithm will generate a unique test case or path through the GUI flow graph every time"


* 2008
  * [Efficient Software Test Case Generation Using Genetic Algorithm Based Graph Theory](https://www.computer.org/csdl/proceedings/icetet/2008/3267/00/3267a298-abs.html)
    * Emerging Trends in Engineering & Technology, International Conference on (2008)
    * Authors: Velur Rajappa, Arun Biradar, Satanik Panda
    * Abstract: "In orthodox software testing approach we generally use modeling based testing approach for generating the test cases of a given problem. This leads to confusion of the test input and the expected output for a given test case. More over we also can miss some of the test cases due to lack of clarity in the test paths. To over come such sort of predictive modeling we propose graph theory based genetic approach to generate test cases for software testing. At first we will create a directed graph of all the intermediate state of the system for the expected behavior of the system. Then we will create a population of all the nodes of the graph as the base population of genetic algorithm. From this population we can find a pair of node the parents and perform genetic crossover and mutation on them for the getting the optimum child nodes as the out put. We should continue this process of genetic operation until all the nodes are covered or any of the nodes, which are visited more than once, should be discarded form the population. Then follow the same process for the generation of test case in the real time system. This technique will be more concrete in case of network testing or any of the system testing where the predictive model based tests are not optimized to produced the out put."



### Academic Paper to Locate
* Berndt, D.; Fisher, J.; Johnson, L.; Pinglikar, J. and Watkins, A.(2003), Breeding Software Test Cases With Genetic Algorithms, Proceeding of the 36th Annual Hawaii International Conference on System Sciences, Track 9, Volume 9, ISBN: 0-7695-1874-5, pp.10.

* Chen Yong, Zhong Yong, Tingting Shi1, Liu Jingyong, (2009), “Comparison of Two Fitness Functions for GA-based Path-Oriented Test Data Generation” , Fifth International Conference on
Natural Computation, IEEE 2009.

* Ghiduk, Ahmed S and Girgis, Moheb R.(2010), Using Genetic Algorithms and Dominance Concepts for Generating Reduced Test Data, Informatica (Slovenia), Volume 34, Number 3, pp.377-385

* Haichang Gao, Boqin Feng and Li Zhu(2005), A Kind of SAaGA Hybrid Meta-heuristic algorithm for the automatic Test Data Generation, International Conference on Neural Network’s and Brain, pp.111-114.

* Michael, C.C., McGraw, G.E., Schatz, M.A. and Walton, C.C.,(1997), Genetic algorithms for dynamic test data generation, International Conference on Automated Software Engineering, 1
st– 5th November 1997, Incline Village, NV, USA, ISBN: 0-8186-7961-1, pp. 307-308.

* Rajappa V. , Biradar A.and Panda S.(2008), Effective Software Test Case Generation Using Genetic Algorithm Based Graph Theory, First International Conference on Emerging Trends in Engineering & Technology, pp.298-303.

* Rauf A., Anwar S., Jaffer M.A.and Shahid A.A.(2010), ```Automated GUI Test Coverage Analysis Using GA```, 7th International Conference on Information Technology New Generations, pp. 1057-1062.

* Srivastava P.R and Tai-hoon Kim(2009), Application of Genetic Algorithm in Software Testing, International Journal of Software Engineering and its Applications, October 2009, Vol. 3, No. 4

* Aljahdali S.H , Ghiduk A.S and Telbemy M.(2010), The limitations of Genetic algorithms in software testing, International Conference on Computer Systems and Applications, held at Ham    mamet from 16th  May to 19th May 2010, ISBN: 978-1-4244-7716-6, pp: 1-7.



The tool can used by opening visual Studio by using the shortcut on the dektop. 

Covana is used for Precise Identification of Problems for Structural Test Generation 
==========================================================================

Project Summary:
The process of achieving high structural coverage of the program under test can be automated using tools built for automated test-generation approaches. When applied on complex programs in practice, these approaches face various problems in generating test inputs to achieve high structural coverage. Our preliminary study identified two main types of problems: (1) external-method-call problem (EMCP), where the method calls from external libraries throw exceptions to abort test executions or their return values are used to decide subsequent branches, causing the branches not to be covered; (2) object-creation problem (OCP), where tools fails to generate method-call sequences to produce desirable object states. Since these automated tools could not be powerful enough to deal with these various problems in testing complex programs, we advocate cooperative developer testing, where developers provide guidance to help tools achieve higher structural coverage. To reduce the efforts of developers in providing guidance to tools, in this paper, we propose a novel approach, called Covana, to precisely identify and report problems that prevent the tools from achieving high structural coverage by computing data dependency between problem candidates and not-covered branches. We provide two techniques to instantiate Covana to identify EMCPs and OCPs. To show the effectiveness of Covana, we conduct evaluations on two open source projects. Our results show that Covana effectively identifies 43 EMCPs out of 1610 EMCP candidates with only 1 false positive and 2 false negative, and 155 OCPs out of 451 OCP candidates with 20 false positives and 28 false negatives.

Project website:
http://research.csc.ncsu.edu/ase/projects/covana/

Once inside Visual Studio follw the follwing instructions:
1.Open Visual Studio
2.Open Covana from recent projects.
3.From the Benchmarks folder select ExceptionThrownbyExternalMethodsTest.cs file.
4. Right click on the method and select "Run PEx Explorations".
5.After Pex finish exploration, launch the project "CovanaAnalysisForm" using the run icon. A main window of Covana will show up.(as in youtube video)
6. Click the "Analyse" button to get result.

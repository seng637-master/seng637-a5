**SENG 637 - Dependability and Reliability of Software Systems**

**Assignment 5**

**Software Reliability Assesssment**

Instructor: Dr. Behrouz Far (far@ucalgary.ca)

Teaching Assistants:

Yousef Mehrdad Bibalan
([yousef.mehrdadbibala@ucalgary.ca](mailto:yousef.mehrdadbibala@ucalgary.ca))

Department of Electrical and Computer Engineering

University of Calgary

**Summary:**

-   Install a reliability assessment (reliability growth and reliability
    demonstration chart) tool.

-   Run the tool and feed the provided data into it.

-   Display and discuss the results.

>   **Due Date: TBD**

**INTRODUCTION**

>   This lab includes analysis of integration test data using reliability
>   assessment tools. There are two ways to assess failure data:

1.  Reliability growth testing

2.  Reliability assessment using Reliability Demonstration Chart (RDC)

    Both will be practiced in this lab.

    **PART 1) RELIABILITY GROWTH TESTING**

    **1.1 OBJECTIVES**

    The purpose of this assignment is to give students hands-on experience on
    assessing the reliability of a hypothetical system given its failure data
    collected during integration testing. To do this, students will need to
    install a reliability growth assessment tool, such as CASRE or SRTAT, and
    create plots of failure rate and reliability of SUT.

    After completing this part, students will:

    -   gain an understanding of what reliability growth testing is and why it
        is useful.

        -   be able to measure the failure rate, MTTF and reliability of the SUT
            through analyzing the test data.

        -   become familiar with the features and usage of a reliability growth
            testing tool.

            **1.2 TESTING TOOLS**

            The testing tool to be used in this part, is either CASRE (freeware
            running on 32bit systems) or START (open source, developed by Dr.
            Far’s Lab, running on various OS including 32bit and 64bit Windows
            and Linux). When using CASRE, Dr. Far’s Lab has developed a Dosbox
            environment for it that allows it run on 32-bit and 64bits Windows
            OS.

            **1.3 SYSTEM UNDER TEST**

            The system to be tested for this part is a hypothetical system and
            its failure data will be distributed via the D2L. There will be a
            few test data files and the students should select one of them.

            **1.4 FAMILIARIZATION**

            1.4.1 INSTALL CASRE

            1.  Get the CASRE30.exe (self-extracting archive) and its manual
                CASRE3UG.pdf from D2L.

            2.  Get the CASRE-DOSBOX.zip from D2L.

            3.  If you are running 32-bit Windows operating system, follow the
                installation process for CASRE30 and run it.

            4.  If you are running 64-bit Windows operating system you need to
                install CASRE-DOSBOX.zip by:

                -   unzip the CASRE-DOSBOX.zip

                -   run DOSBoxinst.exe

                    This will create C:\\Win3HD and install DOSBOX and CASRE in
                    it (if these are not already in the package

                -   run the inst.bat

                -   go to Win3HD folder in your C:\\Win3HD drive in your
                    computer --or-- the \\Win3HD that is in the unpacked DOSBOX
                    package

                -   run CASRE from either of the Win3HD folders

**Note:** If the models do not show up in the model selection menu when running
CASRE, you should copy the casrev3.ini file from CASRE-DOSBOX.zip package
(located at the root directory of this package) to C:\\Win3HD\\WINDOWS and start
CASRE again.

>   Alternatively

>   1.4.2 INSTALL STRAT

1.  Get SRTAT-SRE-tool.zip from D2L.

    1.  It is a Java package that has 4 variations for different operating
        systems. Install the appropriate version on your system.

        1.  Run and verify its functionalities.

**1.5 INSTRUCTIONS**

![](media/99bd5ae86174f8d52c55ad61c2ccb4f0.emf)

**1.5.1 Running CASRE**

Computer-Aided Software Reliability Estimation Tool. CASRE provides operations
to transform or smooth the failure data; the user can select and/or define
multiple models for application to the data and make reliability predictions
based on the best model.

1.  Run CASRE

2.  Import failure data

3.  Select a set of models that would provide the best fit for the project data
    using model ranking

4.  Select the range of useful data using Laplace or other tests

5.  Display time-between-failures, failure intensity and reliability graphs

6.  Discuss the acceptable range of failure rate for the test data

**1.5.2 Running SRTAT**

Software Reliability and Testing Analysis Tool.

1.  Run SRTAT

2.  Execute steps 2-6 same as above

Note:

If none of the above mentioned tools work for you, try to find other tools that
may work.

A list of those tools (freeware) are given below:

<https://sasdlc.org/lab/assets/projects/srt.html>

1.  Software Defect Estimation Tool (SweET)

GITHUB: <https://github.com/LanceFiondella/SwEET>

1.  Software Failure and Reliability Assessment Tool (SFRAT)

GITHUB: <https://github.com/LanceFiondella/srt.core>

>   **Part 2) ASSESSMENT USING RELIABILITY DEMIONSTRATION CHART**

1.  **OBJECTIVES**

    Reliability Demonstration Chart (RDC) is an efficient way of checking
    whether the target failure rate or MTTF is met or not. It is based on
    collecting failure data at time points. The main objective of this part of
    the assignment is to familiarize students with RDC tool and its usage during
    reliability assessment.

    We usually use RDC when failure data is limited to a few failures, time of
    failures are known, and we want to find out what is the trend for
    reliability of the system.

    After completing this part, students will:

    -   be able to decide upon adequacy of testing for a given MTTF of the SUT
        through plotting the test data.

        -   become familiar with the features and usage of an RDC tool.

            **2.2 TESTING TOOLS**

            In this assignment, you will use either SRTAT or RDC-11 (an EXCEL
            worksheet and macro) tool to analyze the test data provided.

            **2.3 SYSTEM UNDER TEST**

            The system to be tested for this part is a hypothetical system and
            its failure data will be distributed via the D2L. There will be a
            few test data files and the students should select one of them.

>   **2.4 FAMILIARIZATION**

>   2.4.1 INSTALL RDC

1.  Get Reliability-Demonstration-Chart.xls and its manual RDC-xls-Overview.pdf
    from D2L.

    1.  Open the excel sheet and verify that it works by setting various risk
        factors, i.e. check whether the right chart will be generated.

        1.  Read the document explaining its functionality.

            1.  ![Picture1](media/a17167c26c1c8fe6dd5b4136561fb660.png)If you
                are running 64-bit Windows operating system, install the
                CASRE-DOSBOX and then install and run CASRE.

>   Alternatively

>   2.4.2 INSTALL STRAT (as in 1.4.2, RDC is included in SRTAT tool as an option
>   tab)

1.  Get SRTAT-SRE-tool.zip from D2L.

    1.  It is a Java package that has 4 variations for different operating
        systems. Install the appropriate version on your system.

        1.  Run and verify its functionalities.

1.  **INSTRUCTIONS**

1.  Make yourself familiar with the RDC. Try to understand how it works.
    Vertical axis is failure number (n), horizontal axis is normalized failure
    data (Tn), i.e., failure time divided by MTTF.

2.  How to use RDC? You need to input the failure data (failure number and
    failure time); identify the target MTTF and anticipated confidence levels;
    and draw the failure points on the graph and analyze the trend. Consult with
    the examples in the lecture slides and RDC manual.

3.  You can experiment with “what-if” scenarios by setting various values for
    MTTF and draw the plot.

4.  Select the minimum MTTFmin for which the SUT becomes acceptable. Set MTTF to
    twice and half MTTFmin and plot the failure data.

5.  Document the results at the end of your report file.

**Submission:**

Submit the results for part 1 and part 2.

1.  Document the results (plot/diagrams as well as explanation of each).

2.  Compare the results of Part1 and Part 2 and justify the case that each
    technique can be used.

# Evaluation Criteria:

**Demo (15%)**

>   The objectives for the demo are a) Preparing you for technical
>   presentations, b) an early assessment of your work to give you a second
>   chance to submit a high-quality report, and c) making sure everybody in the
>   team contributes evenly.

>   It is mandatory for all team members to attend the demo session and explain
>   the TAs in the lab what they have done for this assignment. For this
>   particular assignment, **Lab10** is the demo day. You are expected to almost
>   finish the assignment by the lab hour. All the team members should attend
>   the lab. The TAs will go through the groups and each group must demonstrate
>   the results of each part of the assignment.

## NOTE: Student who miss the demo session or are unable to demo what is detailed above are considered as less- contributors and may lose up to the entire assignment’s mark.

**Lab report (85%)**

>   Students will be required to submit a report on their work in the lab as a
>   group. To be consistent, please use the template Word file
>   “Assignment5-ReportTemplate.doc” provided online under the Assignment 5
>   folder. If desired, feel free to rename the sections, as long as the
>   headings are still descriptive and accurate.

## 

>   A portion of the grade for the lab report will be allocated to organization
>   and clarity. The report marking scheme is as follows:

| **Reliability Growth Testing (40)**                                                                      |    |
|----------------------------------------------------------------------------------------------------------|----|
| Result of model comparison (selecting top two models)                                                    | 5  |
| Result of range analysis (an explanation of which part of data is good for proceeding with the analysis) | 5  |
| Plots for failure rate and reliability of the SUT for the test data provided                             | 15 |
| A discussion on decision making given a target failure rate                                              | 10 |
| A discussion on the advantages and disadvantages of reliability growth analysis                          | 5  |
| **RDC Testing (30)**                                                                                     |    |
| 3 plots for MTTFmin, twice and half of it for your test data                                             | 15 |
| Explain your evaluation and justification of how you decide the MTTFmin                                  | 10 |
| A discussion on the advantages and disadvantages of RDC                                                  | 5  |
| **Other (15)**                                                                                           |    |
| Comparison of the results with the Part 1                                                                | 10 |
| A discussion on similarity and difference of the two techniques. Any lessons learned in this lab?        | 5  |

**REFERENCES**

1.  Open Channel Foundation

    <http://www.openchannelsoftware.org/discipline/Reliability_Analysis>

2.  ReliaSoft (commercial software)

    <http://www.reliasoft.com/products.htm>

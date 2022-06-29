# 关于软件配置错误研究过程

## 相关论文

## Survey & Empical study

- 《An Empirical Study on Configuration Errors in Commercial and Open Source Systems》[Link](http://opera.ucsd.edu/paper/sosp11-yin.pdf) (SOSP, 2011)   配置错误定义、分类

- 《Systems Approaches to Tackling Configuration Errors: A Survey》[Link](https://tianyin.github.io/pub/csur.pdf)（2015）

- 《An Evolutionary Study of Configuration Design and Implementation in Cloud Systems》（2021，ICSE，**开源**）

## Error Injection

- 《Proactive Detection of Inadequate Diagnostic Messages for Software Configuration Errors》[Link](https://homes.cs.washington.edu/~mernst/pubs/inadequate-diagnostics-issta2015.pdf)  （Tool Name：ConfDiagDetector，ISSTA，2015，[开源](https://github.com/zhang-sai/config-errors)）

- 《ConfErr: A tool for assessing resilience to human configuration errors》[Link](https://infoscience.epfl.ch/record/129043/files/conferr.pdf ) （Tool Name：ConfErr，DSN，2008，[开源](https://github.com/lokeller/conferr)）

- 《ConfTest: Generating Comprehensive Misconfiguration for System Reaction Ability Evaluation》[Link](https://dl.acm.org/doi/abs/10.1145/3084226.3084244)

- 《ConfVD: System Reactions Analysis and Evaluation Through Misconfiguration Injection》[Link](https://ieeexplore.ieee.org/abstract/document/8470110)

- 《Do Not Blame Users for Misconfigurations》[https://tianyin.github.io/pub/spex.pdf](https://tianyin.github.io/pub/spex.pdf)（SOSP，2013）

## Detection

- 《Automated Reasoning and Detection of Specious Configuration in Large Systems with Symbolic Execution》[Link](https://www.usenix.org/system/files/osdi20-hu.pdf) (OSDI, 2020)
- 《Rex: Preventing Bugs and Misconfiguration in Large Services Using Correlated Change Analysis》[Link](https://www.usenix.org/system/files/nsdi20-paper-mehta.pdf) (NSDI, 2020) - Correlated-change analysis for Microsoft Office 365 and Azure
- 《PracExtractor: Extracting Configuration Good Practices from Manuals to Detect Server Misconfigurations》[Link](https://www.usenix.org/conference/atc20/presentation/xiang) (USENIX, 2020，**不开源**) - Using NLP to learn good practices and detect bad practices
- 《EnCore: Exploiting System Environment and Correlation Information for Misconfiguration Detection》[Link](https://tianyin.github.io/pub/encore.pdf) (ASPLOS, 2014) - Checking correlations between configuration values and the deployment environment (VM images)  **简单复现**：[Link](https://github.com/Czw007/EnCore)
- 《Context-based Online Configuration-Error Detection》[Link](https://www.usenix.org/legacy/event/atc11/tech/final_files/Yuan.pdf) (USENIX ATC, 2011) - Detecting abnormal configuration event sequences

- 《Automated Diagnosis of Software Configuration Errors》[Link](https://homes.cs.washington.edu/~mernst/pubs/configuration-errors-icse2013.pdf) (ICSE, 2013) - Identify behavior deviation caused by misconfiguration
- 《X-ray: Automating Root-Cause Diagnosis of Performance Anomalies in Production Software》[Link](https://www.usenix.org/conference/osdi12/technical-sessions/presentation/attariyan) (OSDI, 2012) - Inferring causality between performance anomalies and configuration values
- 《Precomputing Possible Configuration Error Diagnoses》[Link](https://asrabkin.bitbucket.io/papers/ase11.pdf) (ASE, 2011)
- 《Automating configuration troubleshooting with dynamic information flow analysis》[Link](https://www.usenix.org/legacy/events/osdi10/tech/full_papers/Attariyan.pdf) (OSDI, 2010) - Inferring causality between failures and configuration values
- 《Configuration Debugging as Search: Finding the Needle in the Haystack》[Link](https://www.usenix.org/legacy/publications/library/proceedings/osdi04/tech/full_papers/whitaker/whitaker.pdf) (OSDI, 2004) - Debugging by time traveling
- 《Automatic Misconfiguration Troubleshooting with PeerPressure》[Link](https://www.usenix.org/legacy/events/osdi04/tech/full_papers/wang/wang.pdf) (OSDI, 2004) - Integrated in Windows troubleshooting toolkit for Windows registry
- 《Synthesizing Configuration File Specifications with Association Rule Learning》（OOPSLA，2017，[开源](https://github.com/ConfigV/ConfigV)）

## Fixed



## 其他开源项目

### Dateset

大量的配置文件

https://github.com/tianyin/configuration_datasets

### fuzz

变异配置的项目

https://github.com/confuzz-code/confuzz-code

### security detect

安全配置检查

https://github.com/birhanum/SCAAMP 

https://github.com/sektioneins/pcc 利用已有安全策略检查配置项



## 个人工作

实证研究
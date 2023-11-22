# SYSMOD IncQuery Validator Demo Repository 

This repository showcases the github action integration of IncQuery Validator for Enterprise Architect to check our model against the built-in rules of the [SYSMOD methodology](https://mbse4u.com/sysmod/).

Download Systems Modeling Toolbox (SYSMOD) from LieberLieber https://www.lieberlieber.com/en/expertise/model-based-systems-engineering/#SYSMOD

> The real strength of MBSE is not the diagrams, but that tools can read the data and support the engineers in their work. A validator is a nice application of this. Modeling SysML without validation is like programming without running the compiler. The SYSMOD validator shows where the model does not follow the SYSMOD procedure. (Tim Weilkiens)

## GitHub Action to deploy and run IncQuery Validator for Enterprise Architect

This repository uses a GitHub Action for deploying and running *IncQuery Validator for Enterprise Architect*. The repository also contains a workflow demonstrating how to use the action.

### What does this action do?

This action downloads and installs *IncQuery Validator for Enterprise Architect* (if not already installed on the GitHub Runner), then executes a model analysis with the specified analysis suite on the specified Enterprise Architect model. The result of the analysis will be available in the artifacts of the workflow. If the workflow is triggered on a branch which has a pull request, then a comment is posted about the summary of the analysis. A basic pass-fail criteria is also configurable.

### About IncQuery Validator

IncQuery Validator is a powerful tool that provides Automated Quality Gates as an integral part of your next-generation MBSE workflow. Running either as a stand-alone desktop application, or as a server-side automated pipeline, it can generate rich validation reports including a high-level Quality Score, as well as detailed rule violation breakdowns, that give information on the general context, severity, and impact of each quality issue.

For more information visit [https://incquery.io/validator](https://incquery.io/validator).

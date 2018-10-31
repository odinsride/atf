---
layout: default
---
# OOB Automated Testing
[![Discord](https://img.shields.io/discord/289994252241338369.svg)](https://discord.gg/QaMwnGd)
[![GitHub issues](https://img.shields.io/github/issues/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/issues)
[![GitHub forks](https://img.shields.io/github/forks/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/network)
[![GitHub stars](https://img.shields.io/github/stars/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/stargazers) 
[![GitHub pull requests](https://img.shields.io/github/issues-pr/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/pulls/)

OOB Automated Testing is a scoped app to capture tests for all the Out of Box 
servicenow applications.  With this you have a place to start your own tests 
instead of starting from scratch.  Once installed you'll be able to run a batch
of tests against the instance.  One key detail about all of these tests, they
are all self-contained.  Meaning, you don't need to load up any demo users,
companies or groups to try these tests.  They are all included in this scoped
application.  
![Demo](/assets/demo.gif)

## Installation

If you just want to try it out, follow these steps;

1. Due to this being a Scoped Application, to make this work with simplifying 
   tests, one modification must be made in Global Scope.  On 
   `/sys_db_object.do?sysparm_query=name=sys_user_group`
   under "Application Access", check "Can create", "Can update", "Can delete", 
   and save.
   ![Update Group Permission](/assets/group-permissions.gif)
2. Import `https://github.com/jacebenson/x_8821_atf.git` to source control 
   within Studio.

## Usage

After it's installed you can run the tests by going to Test Suites, OOB Tests
and then run it.  

### Features

Below is the desired organization of test suites.  Some of these are closed 
because there is no good way to test things.  Some of these are closed because
someone has done some of the work.  As work continues I'll add notes to these
issues.  A key feature of these tests is that they are all self contained.
Meaning they rely on no outside data.

- API Testing
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/1.svg)](https://github.com/jacebenson/x_8821_atf/issues/1) Agent Intelligence
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/2.svg)](https://github.com/jacebenson/x_8821_atf/issues/2) Aggregate API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/3.svg)](https://github.com/jacebenson/x_8821_atf/issues/3) Application Service API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/4.svg)](https://github.com/jacebenson/x_8821_atf/issues/4) Attachment API 
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/5.svg)](https://github.com/jacebenson/x_8821_atf/issues/5) CI Lifecycle Mangement API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/6.svg)](https://github.com/jacebenson/x_8821_atf/issues/6) Clotho Time Series API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/7.svg)](https://github.com/jacebenson/x_8821_atf/issues/7) CMDB Instance API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/8.svg)](https://github.com/jacebenson/x_8821_atf/issues/8) CMDB Meta API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/29.svg)](https://github.com/jacebenson/x_8821_atf/issues/29) Email API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/9.svg)](https://github.com/jacebenson/x_8821_atf/issues/9) IdentifyReconcile API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/28.svg)](https://github.com/jacebenson/x_8821_atf/issues/28) Import Set API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/10.svg)](https://github.com/jacebenson/x_8821_atf/issues/10) Interaction Management API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/11.svg)](https://github.com/jacebenson/x_8821_atf/issues/11) Major Incident Management API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/12.svg)](https://github.com/jacebenson/x_8821_atf/issues/12) Performance Analytics API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/13.svg)](https://github.com/jacebenson/x_8821_atf/issues/13) Service Catalog API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/14.svg)](https://github.com/jacebenson/x_8821_atf/issues/14) Table API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/15.svg)](https://github.com/jacebenson/x_8821_atf/issues/15) Task Communication Management API
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/16.svg)](https://github.com/jacebenson/x_8821_atf/issues/16) User Role Maintenance API
- Customer Service Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/37.svg)](https://github.com/jacebenson/x_8821_atf/issues/37) Communities
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/38.svg)](https://github.com/jacebenson/x_8821_atf/issues/38) Customer Service
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/39.svg)](https://github.com/jacebenson/x_8821_atf/issues/39) Field Service
- Governance, Risk , and Compliance (GRC)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/25.svg)](https://github.com/jacebenson/x_8821_atf/issues/25) Audit
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/40.svg)](https://github.com/jacebenson/x_8821_atf/issues/40) Policy and Compliance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/33.svg)](https://github.com/jacebenson/x_8821_atf/issues/33) Risk
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/34.svg)](https://github.com/jacebenson/x_8821_atf/issues/34) Vendor Risk
- HR Service Delivery
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/41.svg)](https://github.com/jacebenson/x_8821_atf/issues/41) Case and Knowledge
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/42.svg)](https://github.com/jacebenson/x_8821_atf/issues/42) Employee Document
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/43.svg)](https://github.com/jacebenson/x_8821_atf/issues/43) Employee Service Center
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/44.svg)](https://github.com/jacebenson/x_8821_atf/issues/44) Enterpise Onboarding and Transistions
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/45.svg)](https://github.com/jacebenson/x_8821_atf/issues/45) HR Integrations
- IT Business Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/46.svg)](https://github.com/jacebenson/x_8821_atf/issues/46) Agile Development 
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/47.svg)](https://github.com/jacebenson/x_8821_atf/issues/47) Business Planning Portal
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/48.svg)](https://github.com/jacebenson/x_8821_atf/issues/48) Cost
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/49.svg)](https://github.com/jacebenson/x_8821_atf/issues/49) Enterprise Release Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/50.svg)](https://github.com/jacebenson/x_8821_atf/issues/50) Financial
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/51.svg)](https://github.com/jacebenson/x_8821_atf/issues/51) Project Portfolio
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/52.svg)](https://github.com/jacebenson/x_8821_atf/issues/52) Scaled Agile Frameworkf (SAFe)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/53.svg)](https://github.com/jacebenson/x_8821_atf/issues/53) Test Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/54.svg)](https://github.com/jacebenson/x_8821_atf/issues/54) Time Card
- IT Operations Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/55.svg)](https://github.com/jacebenson/x_8821_atf/issues/55) Cloud Management (Will require active accounts on azure/aws to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/56.svg)](https://github.com/jacebenson/x_8821_atf/issues/56) Discovery (Will require setting up a mid, and other infrastructure to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/57.svg)](https://github.com/jacebenson/x_8821_atf/issues/57) Event Management (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/58.svg)](https://github.com/jacebenson/x_8821_atf/issues/58) Operational Intelligence (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/59.svg)](https://github.com/jacebenson/x_8821_atf/issues/59) Service Mapping (Unsure how to test)
- IT Service Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/30.svg)](https://github.com/jacebenson/x_8821_atf/issues/30) Asset
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/60.svg)](https://github.com/jacebenson/x_8821_atf/issues/60) Benchmarks
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/19.svg)](https://github.com/jacebenson/x_8821_atf/issues/19) Change
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/61.svg)](https://github.com/jacebenson/x_8821_atf/issues/61) Continual Improvement
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/62.svg)](https://github.com/jacebenson/x_8821_atf/issues/62) Contract
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/63.svg)](https://github.com/jacebenson/x_8821_atf/issues/63) Expense Line
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/17.svg)](https://github.com/jacebenson/x_8821_atf/issues/17) Incident
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/18.svg)](https://github.com/jacebenson/x_8821_atf/issues/18) Incident Communications
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/64.svg)](https://github.com/jacebenson/x_8821_atf/issues/64) ITSM Virtual Agent
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/65.svg)](https://github.com/jacebenson/x_8821_atf/issues/65) On-call Scheduling 
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/20.svg)](https://github.com/jacebenson/x_8821_atf/issues/20) Problem
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/66.svg)](https://github.com/jacebenson/x_8821_atf/issues/66) Procurement
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/67.svg)](https://github.com/jacebenson/x_8821_atf/issues/67) Product Catalog
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/68.svg)](https://github.com/jacebenson/x_8821_atf/issues/68) Release
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/21.svg)](https://github.com/jacebenson/x_8821_atf/issues/21) Request 
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/22.svg)](https://github.com/jacebenson/x_8821_atf/issues/22) Service Catalog
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/69.svg)](https://github.com/jacebenson/x_8821_atf/issues/69) Service Desk
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/70.svg)](https://github.com/jacebenson/x_8821_atf/issues/70) Service Level
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/71.svg)](https://github.com/jacebenson/x_8821_atf/issues/71) Service Portfolio
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/72.svg)](https://github.com/jacebenson/x_8821_atf/issues/72) Vendor Performance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/73.svg)](https://github.com/jacebenson/x_8821_atf/issues/73) Walk-up Experience
- Now Platform
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/74.svg)](https://github.com/jacebenson/x_8821_atf/issues/74) Agent Intelligence
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/75.svg)](https://github.com/jacebenson/x_8821_atf/issues/75) CMDB
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/76.svg)](https://github.com/jacebenson/x_8821_atf/issues/76) Compliance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/77.svg)](https://github.com/jacebenson/x_8821_atf/issues/77) Connect (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/78.svg)](https://github.com/jacebenson/x_8821_atf/issues/78) Content Management System
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/79.svg)](https://github.com/jacebenson/x_8821_atf/issues/79) Data Certification
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/80.svg)](https://github.com/jacebenson/x_8821_atf/issues/80) Dependency Views
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/81.svg)](https://github.com/jacebenson/x_8821_atf/issues/81) Flow Designer (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/82.svg)](https://github.com/jacebenson/x_8821_atf/issues/82) IntegrationHub (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/83.svg)](https://github.com/jacebenson/x_8821_atf/issues/83) Interaction Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/84.svg)](https://github.com/jacebenson/x_8821_atf/issues/84) Knowledge Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/85.svg)](https://github.com/jacebenson/x_8821_atf/issues/85) Live Feed
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/86.svg)](https://github.com/jacebenson/x_8821_atf/issues/86) Managed Documents
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/87.svg)](https://github.com/jacebenson/x_8821_atf/issues/87) MetricBase
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/88.svg)](https://github.com/jacebenson/x_8821_atf/issues/88) Notifications
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/89.svg)](https://github.com/jacebenson/x_8821_atf/issues/89) Notify
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/90.svg)](https://github.com/jacebenson/x_8821_atf/issues/90) Orchestration (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/91.svg)](https://github.com/jacebenson/x_8821_atf/issues/91) Password Reset (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/92.svg)](https://github.com/jacebenson/x_8821_atf/issues/92) Service Administration
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/93.svg)](https://github.com/jacebenson/x_8821_atf/issues/93) Service Portal
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/95.svg)](https://github.com/jacebenson/x_8821_atf/issues/95) Subscription Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/94.svg)](https://github.com/jacebenson/x_8821_atf/issues/94) Survey Management (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/96.svg)](https://github.com/jacebenson/x_8821_atf/issues/96) Task Communication Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/97.svg)](https://github.com/jacebenson/x_8821_atf/issues/97) Virtual Agent (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/98.svg)](https://github.com/jacebenson/x_8821_atf/issues/98) Visual Task Boards (Unsure how to test)
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/99.svg)](https://github.com/jacebenson/x_8821_atf/issues/99) Workflow (Unsure how to test)
- Security Operations
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/100.svg)](https://github.com/jacebenson/x_8821_atf/issues/100) Configuration Compliance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/101.svg)](https://github.com/jacebenson/x_8821_atf/issues/101) Security Incident Response
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/102.svg)](https://github.com/jacebenson/x_8821_atf/issues/102) Threat Intelligence
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/103.svg)](https://github.com/jacebenson/x_8821_atf/issues/103) Trusted Security Circles
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/104.svg)](https://github.com/jacebenson/x_8821_atf/issues/104) Vulnerability Response
- Service Management
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/35.svg)](https://github.com/jacebenson/x_8821_atf/issues/35) Coaching Loops
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/36.svg)](https://github.com/jacebenson/x_8821_atf/issues/36) Facilities 
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/105.svg)](https://github.com/jacebenson/x_8821_atf/issues/105) Finance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/106.svg)](https://github.com/jacebenson/x_8821_atf/issues/106) Legal
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/107.svg)](https://github.com/jacebenson/x_8821_atf/issues/107) Marketing
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/108.svg)](https://github.com/jacebenson/x_8821_atf/issues/108) Planned Maintenance
  - [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/109.svg)](https://github.com/jacebenson/x_8821_atf/issues/109) Structured Problem Analysis
- [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/26.svg)](https://github.com/jacebenson/x_8821_atf/issues/26) Software Asset Management
 

## Contributing

Pull requests are welcome. For major changes, please open an issue first to 
discuss what you would like to change.

However there are a lot of issues for everything I could find in servicenow.
If you know that application feel free to fill out the issue and comment on it.

### Setting up a pdi (personal developer instance)

Create an account on [https://developer.servicenow.com/](https://developer.servicenow.com/).
Than Request a Personal Developer Instance.

### Setting up the repo

1.  [Fork this project](https://github.com/jacebenson/x_8821_atf/fork)
2.  Follow the [installation](#installation) steps, but use your repository.

### Actually Contributing

1.  Fork it (https://github.com/jacebenson/x_8821_atf/fork)
2.  Install it from source 
    ![](/assets/install-application.png)
3.  Create your feature branch
    ![](/assets/create-feature-branch.png)
3.  Do you changes.  Things to remember, your username from your instance will
    show up as who made the changes, so leave it admin, or make it custom but
    don't make it something you'll regret.
4.  Commit your changes
    ![](/assets/commit-changes-1.png)
    ![](/assets/commit-changes-2.png)
5.  Push to the branch
6.  Create a new Pull Request

## Resources

* If you need to `set fields` but cannot find 
  you're field, this script might be useful;
  ```js
  var gr = new GlideRecord('sys_atf_step');
  gr.get('f1a43c15db0123008096a455ca961915');
  var fields = gr.inputs.field_values.toString();
  gs.info(fields);
  fields = fields.replace('^EQ','^kb_knowledge_base=dfc19531bf2021003f07e2c1ac0739ab^EQ');
  gs.info(fields);
  gr.inputs.field_values = fields;
  gr.update();
  ```

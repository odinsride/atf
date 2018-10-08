# OOB Automated Testing ![Discord](https://img.shields.io/discord/289994252241338369.svg) [![Discord Invite](https://img.shields.io/badge/discord-invite-green.svg)](https://discord.gg/QaMwnGd)

OOB Automated Testing is a scoped app to 
capture tests for all the Out of Box 
servicenow applications.

## Installation

* servicenow instance London or newer
* Import `https://github.com/jacebenson/x_8821_atf.git` 
  to source control within Studio.

## Features

Tests will exist for and already exist for some of servicenow.

Below is the suite hierarcy.  If checked done.

- [ ] API Testing
- [ ] HR Service Delivery
  - [ ] Case and Knowledge
  - [ ] Employee Service Center
  - [ ] Enterpise Onboarding and Transistions
  - [ ] Employee Document
  - [ ] HR Integrations
- [ ] Customer Service Management
  - [ ] Customer Service
  - [ ] Communities
  - [ ] Field Service
- [ ] Governance, Risk , and Compliance (GRC)
  - [ ] Policy and Compliance
  - [ ] Risk
  - [ ] Audit
  - [ ] Vendor Risk
- [ ] Software Asset Management
- [ ] Security Operations
  - [ ] Security Incident Response
  - [ ] Vulnerability Response
  - [ ] Configuration Compliance
  - [ ] Threat Intelligence
  - [ ] Trusted Security Circles
- [ ] IT Business Management
  - [ ] Project Portfolio
  - [ ] Financial
  - [ ] Time Card
  - [ ] Enterprise Release Management
  - [ ] Agile Development
  - [ ] Scaled Agile Frameworkf (SAFe)
  - [ ] Test Management
  - [ ] Business Planning Portal
  - [ ] Cost
- [ ] IT Operations Management
  - [ ] Discovery
  - [ ] Service Mapping
  - [ ] Event Management
  - [ ] Operational Intelligence
  - [ ] Cloud Management
- [ ] IT Service Management
  - [ ] Asset
  - [ ] Contract
  - [ ] Procurement
  - [ ] Product Catalog
  - [ ] Benchmarks
  - [ ] Change
  - [ ] Continual Improvement
  - [ ] Expense Line
  - [ ] ITSM Virtual Agent
  - [ ] Walk-up Experience
  - [x] Incident
  - [ ] Incident Communications
  - [ ] On-call Scheduling
  - [ ] Problem
  - [ ] Release
  - [ ] Request
  - [ ] Service Catalog
  - [ ] Service Desk
  - [ ] Service Level
  - [ ] Service Portfolio
  - [ ] Vendor Performance
- [ ] Service Management
  - [ ] Planned Maintenance
  - [ ] Facilities
  - [ ] Finance
  - [ ] Legal
  - [ ] Marketing
  - [ ] Coaching Loops
  - [ ] Structured Problem Analysis

## Contributing

Pull requests are welcome. For major changes, 
please open an issue first to discuss what you 
would like to change.

### Setting up a pdi (personal developer instance)

Create an account on [https://developer.servicenow.com/](https://developer.servicenow.com/).
Than Request a Personal Developer Instance.

### Setting up the repo

1.  Fork this project
2.  Log into your PDI
3.  Open Studio
4.  Import your Forked Repo's `https` url

### Actually Contributing

1.  Comment on the issue
2.  Ensure you're in the OOB Automated Testing application
3.  Create the tests and suites appropriate to test the application
4.  Put your tests in the appropriate suites
4.  Commit your repo
5.  Comeback onto github, and make a Pull Request from your repo.

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
* [Issues](https://github.com/jacebenson/x_8821_atf/issues)
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
- [ ] Customer Service Management
  - [ ] Communities
  - [ ] Customer Service
  - [ ] Field Service
- [ ] Governance, Risk , and Compliance (GRC)
  - [ ] Audit
  - [ ] Policy and Compliance
  - [ ] Risk
  - [ ] Vendor Risk
- [ ] HR Service Delivery
  - [ ] Case and Knowledge
  - [ ] Employee Document
  - [ ] Employee Service Center
  - [ ] Enterpise Onboarding and Transistions
  - [ ] HR Integrations
- [ ] IT Business Management
  - [ ] Agile Development
  - [ ] Business Planning Portal
  - [ ] Cost
  - [ ] Enterprise Release Management
  - [ ] Financial
  - [ ] Project Portfolio
  - [ ] Scaled Agile Frameworkf (SAFe)
  - [ ] Test Management
  - [ ] Time Card
- [ ] IT Operations Management
  - [ ] Cloud Management
  - [ ] Discovery
  - [ ] Event Management
  - [ ] Operational Intelligence
  - [ ] Service Mapping
- [ ] IT Service Management
  - [ ] Asset
  - [ ] Benchmarks
  - [ ] Change
  - [ ] Continual Improvement
  - [ ] Contract
  - [ ] Expense Line
  - [x] Incident
  - [ ] Incident Communications
  - [ ] ITSM Virtual Agent
  - [ ] On-call Scheduling
  - [ ] Problem
  - [ ] Procurement
  - [ ] Product Catalog
  - [ ] Release
  - [ ] Request
  - [ ] Service Catalog
  - [ ] Service Desk
  - [ ] Service Level
  - [ ] Service Portfolio
  - [ ] Vendor Performance
  - [ ] Walk-up Experience
- [ ] Security Operations
  - [ ] Configuration Compliance
  - [ ] Security Incident Response
  - [ ] Threat Intelligence
  - [ ] Trusted Security Circles
  - [ ] Vulnerability Response
- [ ] Service Management
  - [ ] Coaching Loops
  - [ ] Facilities
  - [ ] Finance
  - [ ] Legal
  - [ ] Marketing
  - [ ] Planned Maintenance
  - [ ] Structured Problem Analysis
- [ ] Software Asset Management

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
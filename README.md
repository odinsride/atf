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

| Application                             | Issues                                                                                                                                                                                              |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| API Testing                             | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-api.svg?style=for-the-badge&label=API&colorB=red)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-api)       |
| Customer Service Management             | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-csm.svg?style=for-the-badge&label=CSM&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-csm)       |
| Governance, Risk , and Compliance (GRC) | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-grc.svg?style=for-the-badge&label=GRC&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-grc)       |
| HR Service Delivery                     | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-hr.svg?style=for-the-badge&label=HR&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-hr)         |
| IT Business Management                  | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-itbm.svg?style=for-the-badge&label=ITBM&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-itbm)     |
| IT Operations Management                | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-itom.svg?style=for-the-badge&label=ITOM&colorB=red)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aissue+label%3Atest-itom)               |
| IT Service Management                   | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-itsm.svg?style=for-the-badge&label=ITSM&colorB=orange)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-itsm)     |
| Now Platform                            | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-now.svg?style=for-the-badge&label=NOW&colorB=orange)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-now)       |
| Security Operations                     | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-secops.svg?style=for-the-badge&label=SECOPS&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-secops) |
| Service Management                      | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-sm.svg?style=for-the-badge&label=SM&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-sm)         |
| Software Asset Management               | [![GitHub issues by-label](https://img.shields.io/github/issues/jacebenson/x_8821_atf/test-sam.svg?style=for-the-badge&label=SAM&colorB=green)](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3Atest-sam)       |

 

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

1.  [Fork it](https://github.com/jacebenson/x_8821_atf/fork)
2.  Install it from source 

    ![](/assets/install-application.png)
2.  Do you changes.  Things to remember, your username from your instance will
    show up as who made the changes, so leave it admin, or make it custom but
    don't make it something you'll regret.
3.  Commit your changes
    
    ![](/assets/commit-changes-1.png)
    ![](/assets/commit-changes-2.png)
4.  Push to the your repo
5.  Create a new Pull Request

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

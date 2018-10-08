# OOB Automated Testing ![Discord](https://img.shields.io/discord/289994252241338369.svg) [![Discord Invite](https://img.shields.io/badge/discord-invite-green.svg)](https://discord.gg/QaMwnGd)

OOB Automated Testing is a scoped app to capture tests for all the Out of Box servicenow applications.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

You'll need to take the following steps to contribute.

* Spin up a servicenow developer instance [https://developer.servicenow.com/](https://developer.servicenow.com/)
* Log in to your instance
* Goto Studio
* Import from source control
* Paste your forked repo https address
* Import
* Select the OOB Automated Testing Application
* Go back to the standard UI as Test aren't listed in the Studio editor
* Goto automated test, and create Suites and tests as appropriate

## Resources

* If you need to `set fields` but cannot find you're field, this script might be useful;
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
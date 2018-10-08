# OOB Automated Testing ![Discord](https://img.shields.io/discord/289994252241338369.svg) [![Discord Invite](https://img.shields.io/badge/discord-invite-green.svg)](https://discord.gg/QaMwnGd)

OOB Automated Testing is a scoped app to 
capture tests for all the Out of Box 
servicenow applications.

## Installation

* servicenow instance London or newer
* Import `https://github.com/jacebenson/x_8821_atf.git` 
  to source control within Studio.

## Contributing

Pull requests are welcome. For major changes, 
please open an issue first to discuss what you 
would like to change.

Follow the [contributing guide](CONTRIBUTING.md) 
to contribute for specific instructions

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
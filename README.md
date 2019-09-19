### mkdocs
---
https://github.com/mkdocs/mkdocs/

https://www.mkdocs.org/

```py
// mkdocs/tests/plugin_tests.py

class DummyPlugin(plugins.BasePlugin):
  config_scheme = (
    ('foo', config.config_optoins.Type(utils.string_types, default='default foo')),
    ('bar', config.config_options.Type(int, default=0)),
    ('dir', config.config_options.Dir(exists=False)),
  )
  
  def on_pre_page(self, content, **kwargs):
    return '{} {}'.format(self.config['foo'], content)
  
  def on_nav(self, item, **kwargs):
    return None
  
  def on_page_read_source():
  
  def on_pre_build()
  
class TestPluginClass(unittest.TestCase):

  def test_valid_plugin_options(self):
  
  def test_invalid_plugin_options(self):
  
class TestPluginCollection(unittest.TestCase):









```

```
```

```
```


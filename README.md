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








@mock.patch('pkg_resource.iter_entry_points', return_value=[MockEntryPoint])
class TestPluginConfig(unittest.TestCase):

  def test_plugin_config_without_options(self, mock_class):
  
  def test_plugin_config_with_options():
  
  def test_plugin_config_none_with_default(self, mock_class):
  
  def test_plugin_config_unistalled(self, mock_class):
  
  def test_plugin_config_not_list(self, mock_class):
  
  def test_plugin_config_multivalue_dict(self, mock_class):
  
  def test_plugin_config_not_string_or_dict(self, mock_class):
  
  def test_plugin_config_options_not_dict(self, mock_class):
    
    cfg = {
      'plugins': [{
        'simple': 'not a dict'
      }]
    }
    option = config.config_options.Plugins()
    self.assertRaises(config.base.ValidationError, option.validate, cfg['plugins'])
```

```
```

```
```


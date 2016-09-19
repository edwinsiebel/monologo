# Development Site Banner

*Note: Alpha software, in development - please don't use yet*

This is a simple package to display a banner at the top of all pages on your website displaying key dev information:

* Environment
* Git branch
* Last commit
 
## Usage
 
You first need to set the current environment name for your application in the variable ```$environmentName``` 
 
Then output the site banner via:
 
```
$banner = new \Studio24\SiteBanner($environmentName);
echo $banner->getBanner();
```

### Development

Example test code

```
include '/path/to/dev-site-banner/vendor/autoload.php';
use Studio24\SiteBanner;

$banner = new SiteBanner('development');
echo $banner->getBanner();
```

 
## Credits

Credit to Sebastian Bergmann, the lightweight Git reading functionality in this package is based from his work in https://github.com/sebastianbergmann/git

Warning icon from Open Iconic — www.useiconic.com/open

## Twig Environment

A very simple Twig environment to build static sites. No WordPress, no nothing.

#### Setup
1. Download or fork this repo
2. Set your MAMP directory to the resulting folder
3. `index.php` is ready-to-go (loading `index.twig`). If you want to create a new file you'll need...
```php
	require_once('loader.php');
	$data = array('name' => 'Grant', 'cat' => 'Pica');
	echo $twig->render('my-twig-file.twig', $data);
```

4. Your Twig files are powered by the wonderful world of [Twig functions, filters](http://twig.sensiolabs.org/doc/templates.html), etc. However they do NOT have Timber things like `|resize`, `|wpautop`, etc.

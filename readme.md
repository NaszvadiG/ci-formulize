# CodeIgniter Library: New form items

**ci-formulize**

## About this library

This CodeIgniter's Library is used to create custom new form elements.

The markup is prepared to use [Bootstrap framework](http://getbootstrap.com/), [Bootstrap wysiwyg editor](http://jhollingworth.github.io/bootstrap-wysihtml5/) and [jQuery UI](http://jqueryui.com/). I use this elements in my custom CMS.  
You can modify and adapt the HTML output through the view files in the `/application/views/formulize/` folder.

Its usage is recommended for CodeIgniter 2 or greater.  

## Usage

Load the library in the controller:

```php
$this->load->library('formulize');
```

In the view:

```php
// $this->formulize->create($name, $varname, $type, $value);
// $type could be 'txt', 'html', 'date', 'file' or 'checkbox'
// $value paramter is optional.

echo $this->formulize->create('Title', 'title', 'txt', 'New post')->render();

echo $this->formulize->create('Text', 'text', 'html')->render();

echo $this->formulize->create('Date', 'date', 'date')->render();

echo $this->formulize->create('Picture', 'picture', 'file')->render();

echo $this->formulize->create('Display', 'display', 'checkbox')->render();
```

You'll have to add the `/application/views/formulize/` folder in your project.

![Ale Mohamad](http://alemohamad.com/github/logo2012am.png)

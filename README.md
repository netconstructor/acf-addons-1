These are some addons for the AFC Wordpress plugin http://www.advancedcustomfields.com/

Categories is custom field that generates a drop down field with all the categories from your wordpress site.
Unique Key is custom field that generates a unique key for you to use it as a unique number or as a password.

To use it in your theme just copy categories.php and/or unique_key.php in your themes folder or subfolder and in your <strong>functions.php</strong> paste the following code:
<h1>Usage</h1>
<pre>if (function_exists('register_field')) { 
  register_field('Categories_field', dirname(__File__) . '/categories.php'); 
  register_field('Unique_key_field', dirname(__File__) . '/unique_key.php'); 
}</pre>
If you decide to put the files in a sub folder then you can use something like that
<pre>if (function_exists('register_field')) { 
  register_field('Categories_field', dirname(__File__) . '/subfolder_name/categories.php'); 
  register_field('Unique_key_field', dirname(__File__) . '/subfolder_name/unique_key.php');
}</pre>
<h1>Added</h1>
<h2>05-07-2012</h2>
<h3>Categories now have two more options</h3>
<ol>
		<li><em><strong>Show All</strong></em>. When you have the display type to '<em>drop_down</em>', then it will return '<em>all</em>'. <br />
			When you have the display type to '<em>checkboxes</em>' it will return all the categories.</li>
		<br />
		<li><em><strong>Show None</strong></em>. When you have the display type to '<em>drop_down</em>' or '<em>checkboxes</em>', then it will return '<em>none</em>'.</li>
	</ol>
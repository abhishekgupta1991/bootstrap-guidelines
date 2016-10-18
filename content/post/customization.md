+++
date = "2016-10-08T16:26:52+05:30"
draft = false
title = "Customization"

+++
<p>Sometime, we need to customize the bootstrap classes property. There are different approaches to achieve it. The best approach is 'Do not modify the bootstrap.css file'.
<br/>
If you make changes to the bootstrap.css file, things will get complicated very fast. The whole design will break when you want to upgrade Bootstrap files. You can overwrite in your own stylesheet default bootstrap colors, styles, margins, paddings, everything. There is no need to touch the bootstrap.css stylesheet at all.
<br/>
Create your new CSS selector, use it in the HTML, and as long you declare your CSS classes after Bootstrap styles, your definitions will overwrite Bootstrap defaults.</p>

<h4>Example :</h4>
<p>Suppose you want to add background color to the container. You can declare CSS class and give the property to it.</p>
<code>&lt;div class="container container-background"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12 col-sm-6 col-md-4"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>
<div class="container-fluid container-background">
  <p>Customize bootstrap class property.</p>
</div>
<hr/>
Sometime we have to customize bootstrap grid values, font sizes, plugin we need to use etc. Go to bootstrap customize <a href="http://getbootstrap.com/customize/">link</a> customize the values and uncheck the plugin which is not required and click 'Compile and Download' button to get custom version of bootstrap.

+++
date = "2016-10-08T16:26:52+05:30"
draft = false
title = "Customization"

+++
<h3>How do you customize bootstrap to make it look and feel like your site?</h3>
<p>There are multiple ways to customize bootstrap. The preferred way would be through the customize page on the Bootstrap site. This allows you to build and include a custom version of Bootstrap into your project and include only those styles and JavaScript components that you need.</p>

<ul>
  <li>Using the customize page - <a href="http://getbootstrap.com/customize/" target="blank">http://getbootstrap.com/customize/</a></li>
  <ul>
    <li>This is the recommended approach to customize the bootstrap package. We can include our own fonts, decide on the specific colors, decide on spacing including padding and margins and also the specific plugins that will be included within the Bootstrap package.</li>
  </ul>
  <li>Over writing the Bootstrap CSS by using custom CSS:</li>
  <ul>
    <li>o	This can be done but will require you to overwrite a lot of styles as all the classes, elements and states within bootstrap.css will need to be overwritten.</li>
  </ul>
  <li>Over writing the Bootstrap CSS by making edits to the bootstrap.css file:</li>
  <ul>
    <li>This is not recommended and should be avoided. This will not work if we need to upgrade to a newer version of Bootstrap.</li>
  </ul>
</ul>

<h4>Example :</h4>
<p>Suppose you want to add background color to the container. You can declare CSS class and give the property to it.</p>
<code>&lt;div class="container container-background"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12 col-sm-6 col-md-4"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>


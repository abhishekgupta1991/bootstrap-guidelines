+++
date = "2016-10-14T16:26:52+05:30"
draft = false
title = "Grid System"

+++

Bootstrap's include mobile first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases. It includes predefined classes for easy layout options. Bootstrap grid system allows up to 12 columns across the page. Basically it divides the page into 12 equal parts.

<h3>Bootstrap grid system</h3>
<p>Bootstrap’s grid system is made up of 3 things:</p>
<ul>
  <li>Container</li>
  <li>Rows</li>
  <li>Columns</li>
</ul>
<hr/>
<h4>Creating Container or Container Fluid</h4>
<p>Bootstrap’s grid system needs a container or container-fluid to hold rows and columns. A container is a simple <div> element with a class of .container or .container-fluid. The container is used to provide a proper width for the layout, acting as a wrapper for the content. <br/> Containers have padding of 15px on the left and right sides.</p>
<ul>
  <li>The .container class provides a responsive fixed width container. It has specific pixel width values that change its width value with the help of media queries.</li>
  <li>The .container-fluid class provides a full width container, spanning the entire width of the viewport. It has 100% width.</li>
</ul>
<h4>Why we use container or container fluid?</h4>
<p>The .row has a negative left and right margin equal to the left/right padding value of the col-*-*, that is why there are horizontal scrollbars. To overcome the negative spacing we are using container or container fluid above the row.</p>
<h4>Example :</h4>
<h5>Container</h5>
<code>&lt;div class="container"&gt;&lt;/div&gt;</code>
<div class="container example-container">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed lobortis est eget tristique vestibulum. Fusce et pulvinar erat, id viverra sem. Vivamus porttitor, sapien nec mattis fermentum, sem augue ornare erat, vitae interdum ante sapien id libero. Vestibulum luctus augue pretium purus posuere.</p>
</div>
<h5>Container Fluid</h5>
<code>&lt;div class="container-fluid"&gt;&lt;/div&gt;</code>
<div class="container-fluid example-container">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed lobortis est eget tristique vestibulum. Fusce et pulvinar erat, id viverra sem. Vivamus porttitor, sapien nec mattis fermentum, sem augue ornare erat, vitae interdum ante sapien id libero. Vestibulum luctus augue pretium purus posuere.</p>
</div>
<hr/>
<h4>Creating Rows</h4>
<p>A row acts like a wrapper around the columns. Columns create gutters (gaps between column content) via padding. That padding is offset in rows for the first and last column via negative margin on '.rows'.</p>
<h4>Example :</h4>
<h5>Without Row : In this demo, you can see the text is not touching the left edge of the container element. This is because the container’s padding.</h5>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;p&gt;Bootstrap Grid demo with row&lt;/p&gt;<br/>&lt;/div&gt;</code>
<div class="container example-container">
  <p>Bootstrap Grid demo with row</p>
</div>
<h5>With Row : In this demo, you can see the text touching the left edge of the container. This is because the container’s padding has been removed by the row due to the negative margins on the row.</h5>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;p&gt;Bootstrap Grid demo with row&lt;/p&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>
<div class="container example-container">
  <div class="row">
    <p>Bootstrap Grid demo with row</p>
  </div>
</div>
<hr/>
<h4>Creating Columns</h4>
<p>Bootstrap uses different column class prefixes for different sized devices. The classes can be combined to create more dynamic and flexible layouts.
 These prefixes are shown in the table below:</p>
<table class="table">
  <tbody>
    <tr class="bg-success">
      <td>.col-xs-$</td>
      <td>Extra Small</td>
      <td>Phones Less than 768px</td>
    </tr>
    <tr class="bg-info">
      <td>.col-sm-$</td>
      <td>Small Devices</td>
      <td>Tablets 768px and Up</td>
    </tr>
    <tr class="bg-warning">
      <td>.col-md-$</td>
      <td>Medium Devices</td>
      <td>Desktops 992px and Up</td>
    </tr>
    <tr class="bg-danger">
      <td>.col-lg-$</td>
      <td>Large Devices</td>
      <td>Large Desktops 1200px and Up</td>
    </tr>
  </tbody>
</table>
<h4>Example :</h4>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-$ col-sm-$ col-md-$ col-lg-$"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
    <div class="col-xs-1 example-wrapper-col">
      <p>.col-xs-1 .col-sm-1 .col-md-1 .col-lg-1</p>
    </div>
  </div>
</div>
<hr/>
<h4>Best Approach to use columns</h4>
<p>With a mobile-first approach at its core, designers has to create sites for small screens, then scale designs up from there. We don't need to add extra classes. It will help speeding up the application.</p>
<h4>Example :</h4>
<p>If we are using the 12 columns for all the screens we can follow like this:</p>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>

<p>Suppose we need 12 columns grid for mobile and 6 columns for the rest of the screen we can follow like this:</p>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12 col-sm-6"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>

<p>Suppose we need 12 columns grid for mobile, 6 columns for tablet and 4 column for the rest of the screen we can follow like this:</p>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12 col-sm-6 col-md-4"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>

<p>Suppose we need 12 columns grid for mobile, 6 columns for tablet, 4 column for desktop and 2 column for larger desktop we can follow like this:</p>
<code>&lt;div class="container"&gt;<br/>&nbsp;&lt;div class="rows"&gt;<br/>&nbsp;&nbsp;&lt;div class="col-xs-12 col-sm-6 col-md-4 col-lg-2"&gt;&lt;/div&gt;<br/>&nbsp;&lt;/div&gt;<br/>&lt;/div&gt;</code>

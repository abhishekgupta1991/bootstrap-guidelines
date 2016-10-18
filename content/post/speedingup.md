+++
date = "2016-10-06T16:26:52+05:30"
draft = false
title = "Speeding Up"

+++
<p>Make sure you do not end-up writing tons of duplicated code creating too many styles for the same case each time over and over again when translating new designs to the code. Keeping the UI development consistent and well documented with UI style guides can also add a couple of knots.</p>

<p>Use bootstrap helper classes rather than write your custom class to do something.</p>
<ul>
  <li>
    When centering text or divs, use text-center or center-block<br/>
    <code>&lt;p class="text-center"&gt;I am centered text&lt;/p&gt;<br /></code>
    <code>&lt;div class="center-block"&gt;I am centered text&lt;/div&gt;</code>
  </li>
  <br/>
  <li>
    Use a single or combination of the available classes for toggling content across viewport breakpoints.<br/>
    <code>&lt;p class="visible-xs visible-sm visible-md visible-lg"&gt;I am centered text&lt;/p&gt;<br /></code>
    <code>&lt;p class="hidden-xs hidden-sm hidden-md hidden-lg"&gt;I am centered text&lt;/p&gt;<br /><br/></code>
    <table class="table">
      <tbody>
        <tr class="bg-success">
          <td>.visible-$-block</td>
          <td>display: block</td>
        </tr>
        <tr class="bg-warning">
          <td>.visible-$-inline</td>
          <td>display: inline</td>
        </tr>
        <tr class="bg-info">
          <td>.visible-$-inline-block</td>
          <td>display: inline-block</td>
        </tr>
      </tbody>
    </table>
  </li>
  <br/>
  <li>
    When clearing floats or forcing elements to self-clear its children<br/>
    <code>&lt;div class="clearfix"&gt;...&lt;/div&gt;</code>
  </li>
  <br/>
  <li>
    When floating and aligning items to the right or left<br/>
    <code>&lt;div class="pull-left"&gt;...&lt;/div&gt;</code><br/>
    <code>&lt;div class="pull-right"&gt;...&lt;/div&gt;</code><br/>
    <code>&lt;p class="text-left"&gt;...&lt;/p&gt;</code><br/>
    <code>&lt;p class="text-right"&gt;...&lt;/p&gt;</code><br/>
  </li>
  <br/>
  <li>
    When killing .row class margins use clearfix rather than row.<br/>
    <code>&lt;div class="clearfix"&gt;...&lt;/div&gt;</code>
  </li>
</ul>

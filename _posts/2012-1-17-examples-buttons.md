---
layout: example
title: Buttons

prettyprint: true
permalink: /examples/buttons
category: examples
---

CSS3 Button {: #example-title}
===========

<style type="text/css">
  /** The following are CSS styles for the example, with better compatability with all browsers (note the -ms- and -o- vendor tags, for Microsoft browsers and Opera) **/
  .result {
    cursor: pointer;
    display: inline-block;
    background-color: #e6e6e6;
    background-repeat: no-repeat;
    background-image: -webkit-gradient(linear, 0 0, 0 100%, from(#ffffff), color-stop(25%, #ffffff), to(#e6e6e6));
    background-image: -webkit-linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);
    background-image: -moz-linear-gradient(top, #ffffff, #ffffff 25%, #e6e6e6);
    background-image: -ms-linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);
    background-image: -o-linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);
    background-image: linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);
    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffff', endColorstr='#e6e6e6', GradientType=0);
    padding: 5px 14px 6px;
    text-shadow: 0 1px 1px rgba(255, 255, 255, 0.75);
    color: #333;
    font-size: 13px;
    line-height: normal;
    border: 1px solid #ccc;
    border-bottom-color: #bbb;
    -webkit-border-radius: 4px;
    -moz-border-radius: 4px;
    border-radius: 4px;
    -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.2), 0 1px 2px rgba(0, 0, 0, 0.05);
    -moz-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.2), 0 1px 2px rgba(0, 0, 0, 0.05);
    box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.2), 0 1px 2px rgba(0, 0, 0, 0.05);
    -webkit-transition: 0.1s linear all;
    -moz-transition: 0.1s linear all;
    -ms-transition: 0.1s linear all;
    -o-transition: 0.1s linear all;
    transition: 0.1s linear all;
  }
  .result:hover {
    background-position: 0 -15px;
    color: #333;
    text-decoration: none;
  }
  .result:focus {
    outline: 1px dotted #666;
  }
  .result:active {
    -webkit-box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
    -moz-box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
    box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
  }

  .blue {
    color: #ffffff;
    background-color: #0064cd;
    background-repeat: repeat-x;
    background-image: -khtml-gradient(linear, left top, left bottom, from(#049cdb), to(#0064cd));
    background-image: -moz-linear-gradient(top, #049cdb, #0064cd);
    background-image: -ms-linear-gradient(top, #049cdb, #0064cd);
    background-image: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #049cdb), color-stop(100%, #0064cd));
    background-image: -webkit-linear-gradient(top, #049cdb, #0064cd);
    background-image: -o-linear-gradient(top, #049cdb, #0064cd);
    background-image: linear-gradient(top, #049cdb, #0064cd);
    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#049cdb', endColorstr='#0064cd', GradientType=0);
    text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
    border-color: #0064cd #0064cd #003f81;
    border-color: rgba(0, 0, 0, 0.1) rgba(0, 0, 0, 0.1) rgba(0, 0, 0, 0.25);
  }

  .blue:hover {
    color: #FFF;
  }
  /** Stop here for the 2 colors **/
</style>

<figure class="centered">
  <input class="result" type="submit" value="Pick me!" />
  <input class="result blue" type="submit" value="No, pick me!" />
</figure>

First, the HTML. The text on the button is set with `value="Pick Me"`.

    <input class="button" type="submit" value="Pick me!" />
    <input class="button blue" type="submit" value="No, pick me!" />
{: .lang-html }

Next, the CSS, starting with the default gray button.

    .btn {
      /* This lets the user know you can click something. */
      cursor: pointer;

      /* Set a default background color in case the user doesn't see the gradient */
      background-color: #e6e6e6;
      background-repeat: no-repeat;
      background-image: -moz-linear-gradient(top, #ffffff, #ffffff 25%, #e6e6e6);
      background-image: -webkit-linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);
      background-image: linear-gradient(#ffffff, #ffffff 25%, #e6e6e6);

      /* Make the button larger (and easier to click) */
      padding: 5px 14px 6px;

      border: 1px solid #ccc;
      border-bottom-color: #bbb;

      /* Rounded corners */
      -webkit-border-radius: 4px;
      -moz-border-radius: 4px;
      border-radius: 4px;

      /* Emphasize the text slightly */
      text-shadow: 0 1px 1px rgba(255, 255, 255, 0.75);

      /* Fade in different different colors when a user hovers */
      -webkit-transition: 0.1s linear all;
      -moz-transition: 0.1s linear all;
      transition: 0.1s linear all;
    }

    .btn:hover {
      /* Slide the background gradient up, revealing the lighter background color below. */
      background-position: 0 -15px;
      color: #333;  
    }

    .btn:active {
      /* Darken the top of the button to make it look as though the button is being pressed. */
      -webkit-box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
      -moz-box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
      box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.25), 0 1px 2px rgba(0, 0, 0, 0.05);
    }
{: .lang-css}

This blue version builds off of the styles written above.

    .btn.blue {
      color: #FFF;
      background-color: #0064cd;
      background-image: -moz-linear-gradient(top, #049cdb, #0064cd);
      background-image: -webkit-linear-gradient(top, #049cdb, #0064cd);
      background-image: linear-gradient(top, #049cdb, #0064cd);
      text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
      border-color: #0064cd #0064cd #003f81;
      border-color: rgba(0, 0, 0, 0.1) rgba(0, 0, 0, 0.1) rgba(0, 0, 0, 0.25);

      text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
    }

    .btn.blue:hover {
      color: #FFF;
    }
{: .lang-css}

View the source to see additional gradients for older versions of Safari, Opera, and IE.

See the [Bootstrap library on Github](https://github.com/twitter/bootstrap/blob/master/bootstrap.css#L1873) for the full library's source.
---
title: Programming with Plotly
categories:
- Programming
aside: true

---

Here is a chart created with plotly.

First import the necessary libraries

{% highlight python %}
import plotly.graph_objects as go
import plotly.io as pio
{% endhighlight %}

Then go through the steps to create your figure. When it is ready you will need to write it to an html file.

{% highlight python %}
pio.write_html(fig, file='name-of-your-file.html', auto_open=True)
{% endhighlight %}

The auto_open argument opens the file in your browser from where it is saved. Unfortunately, github pages do not allow for iframes to be used. Instead we can insert images, doing so will require having an images folder as part of your site structure along kaleido as part of your python package.

{% highlight python %} fig.write_image('images/name-of-your-image.png') {% endhighlight %}

While, we cannot embed interactive iframes within github pages, we can insert static images:

(fix later)

And additionally, link to the interactive html chart:

[Interactive Covid Case Numbers for United States]({% link interactive_charts/covid.html %})

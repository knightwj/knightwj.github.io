---
layout: post
title:  "深圳公布的第1-416个covid-19病例"
date:   2020-03-06 10:25:27 +0800
categories: jekyll update
---
<p style="text-align:justify; text-justify:inter-ideograph;">
Thanks to the transparent and detailed data sharing of the individual covid-19 cases on a daily basis by the Shenzhen municipal health commision, we have access to the info regarding the infected people's age,gender,and which city is he/she from, relationship with other cases and so on.   
 </p>

<p style="text-align:justify; text-justify:inter-ideograph;">
Data visulization was done by Echarts, Baidu's interactive charting and visulization library,very versatile and handy to use. Relevant info of the library can be found here on the <a href="https://www.echartsjs.com/zh/index.html">Echarts website</a>.  
</p>



Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].



Here is the onset graph

{% include onset.html %}

<p style="text-align:justify; text-justify:inter-ideograph;"> 
Since the case descripitions report explicitly the relations between infected cases, I use network graph to demonstrate how cases are clusted and this kind of plot is helpful to give us a glimpse of how infectious the virus is.
<\p>

<center>
{% include graph_backup.html %}
</center>
  



[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/


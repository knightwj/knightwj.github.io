---
layout: post
title:  "深圳公布的第1-416个covid-19病例"
date:   2020-03-06 10:25:27 +0800
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

<center>

<table>
<tr>
<th rowspan="2">值班人员</th>
<th>星期一</th>
<th>星期二</th>
<th>星期三</th>
</tr>
<tr>
<td>李强</td>
<td>张明</td>
<td>王平</td>
</tr>
</table>

</center>

here is the onset graph

{% include onset.html %}
  
this is the graph showing the individual and clustering cases of covid19 in SZ.

{% include graph.html %}
  


<center>
<script src="https://cdn.bootcss.com/echarts/4.2.1-rc1/echarts.min.js"></script> 
<div id="timeline" style="width: 1000px;height:800px;margin:0;auto;"></div>
    <script type="text/javascript">
        // 基于准备好的dom，初始化echarts实例
        var myChart = echarts.init(document.getElementById('timline'));

        myChart.setOption(
    {
        baseOption: {
            timeline: {
                data: ["2008", "2009","2010","2011","2012","2013","2014"],
                autoPlay: true,
                axisType :"category",
                bottom: 0
            },
            title: {
                subtext: '数据来自国家统计局'
            },
            xAxis: [{
                'type':'category',
                'axisLabel':{'interval':0},
                'data':['北京', '天津', '河北', '山西', '内蒙古', '辽宁', '吉林', '黑龙江', '上海', '江苏', '浙江', '安徽', '福建', '江西', '山东', '河南', '湖北', '湖南', '广东', '广西', '海南', '重庆', '四川', '贵州', '云南', '西藏', '陕西', '甘肃', '青海', '宁夏', '新疆'],
                splitLine: {show: false}
            }],
            yAxis: [ {
                type: 'value',
                name: '剖宫产率（%）'
                // max: 53500
            
            }],
            series: [
                { // 系列一的一些其他配置
                    type: 'bar'
                }
              
               
            ]
        },
        options: [
                { // 这是'2002-01-01' 对应的 option
                title: {text: '2008年统计值'},
                series: [
        {data: [59.2, 68.4, 33.8, 16.0, 32.4, 49.4, 43.1, 49.0, 68.0, 44.2, 50.6, 28.6, 21.1, 20.0, 29.8, 25.9, 42.4, 30.7, 23.2, 14.1, 10.0, 32.5, 34.6, 12.2, 15.8, 1.8, 17.2, 10.6, 5.9, 14.8, 17.3] } 
                
                ]
            },
                {
                title: {text: '2009年统计值'},
                series: [
                    {data: [60.1,71.5,35.5,17.6,36.3,52.9,50.9,51.9,67.6,46.8,51.5,29.8,23.4,21.2,33.0,27.0,45.0,30.8,24.1,15.7,10.4, 35.2,38.3,13.9,18.1,2.3,19.6,11.2,5.7,16.1,18.7]} // 系列一的数据
                
                ]
            },
                { // 这是'2003-01-01' 对应的 option
                title: {
                    text: '2010年统计值'
                },
                series: [
                    {data: [59.2,67.9,37.1,20.9,40.0,56.2,57.3,56.5,67.1,46.7,52.4,32.7,25.0,21.4,34.4,29.6,46.1,31.7,25.4,16.9,11.2,36.7,39.3,15.9,20.4,2.4,23.0,13.3,7.8,17.0,19.4]},

                ]
            },
                { // 这是'2002-01-01' 对应的 option
                title: {
                    text: '2011年统计值'
                },
                series: [
                    {data: [53.6,60.5,38.8,24.1,42.4,57.4,61.1,58.2,62.0,48.4,49.2,35.8,25.6,23.2,35.0,31.2,47.6,33.0,25.2,17.7,12.5,39.3,38.9,17.7,20.0,2.7,25.3,13.5,9.1,18.0,21.3] } // 系列一的数据
                
                ]
            },
                { // 这是'2002-01-01' 对应的 option
                title: {text: '2012年统计值'},
                series: [
        {data: [50.6, 60.9, 38.4, 26.1, 44.8, 57.6, 53.1, 57.1, 57.9, 48.7, 47.7, 39.7, 26.9, 24.5, 36.4, 32.5, 48.8, 34.1, 25.9, 19.6, 13.2, 40.2, 40.5, 20.2, 20.9, 4.1, 27.7, 14.1, 9.7, 17.7, 21.0] } // 系列一的数据
                ]
            },
                { // 这是'2002-01-01' 对应的 option
                title: {text: '2013年统计值'},
                series: [
        {data: [48.9, 62.3, 39.0, 28.4, 46.7, 59.5, 53.0, 58.6, 56.1, 48.9, 46.9, 41.8, 27.9, 25.7, 36.8, 33.8, 48.3, 33.6, 26.4, 20.9, 15.3, 42.5, 39.2, 22.6, 21.1, 3.7, 29.5, 15.1, 10.8, 20.8, 20.9] } // 系列一的数据
                ]
            },
                            { // 这是'2002-01-01' 对应的 option
                title: {text: '2014年统计值'},
                series: [
        {data: [43.2, 57.8, 38.7, 28.8, 48.0, 55.8, 62.5, 58.8, 52.4, 48.8, 44.0, 40.8, 26.3, 26.3, 36.4, 37.1, 49.5, 33.9, 25.9, 21.4, 16.4, 43.3, 39.3, 24.6, 19.4, 4.0, 30.3, 16.2, 12.7, 22.1, 21.6] } // 系列一的数据
                ]
            }



        ]
    }
);
    </script>

</center>
  






[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

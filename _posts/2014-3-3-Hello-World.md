---
layout: post
title: You're up and running!
---

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.


<div style="width:100%;">
    <canvas id="deal_progress" height="200"></canvas>
</div>

<script>
new Chart(document.getElementById("deal_progress"), {
    type: 'line',
    data: {
        labels: ['201511','201512','201601','201602','201603','201604','201605','201606','201607','201608','201609','201610','201611','201612','201701','201702','201703','201704','201705','201706','201707','201708','201709','201710','201711','201712','201801','201802','201803','201804','201805','201806','201807','201808','201809','201810','201811','201812','201901','201902','201903','201904','201905','201906','201907','201908','201909','201910','201911','201912','202001','202002','202003','202004','202005','202006','202007','202008','202009','202010','202011'],
        datasets: [{
            label: '매매',
            pointRadius: 1,
            data: [9, 4, 5, 6, 13, 18, 15, 22, 16, 17, 16, 10, 10, 6, 8, 18, 16, 8, 11, 12, 12, 9, 9, 12, 11, 6, 30, 20, 17, 11, 15, 13, 13, 6, 13, 20, 12, 12, 9, 8, 13, 9, 12, 8, 21, 16, 14, 14, 10, 134, 9, 21, 21, 16, 20, 46, 25, 24, 22, 30, 14],
            borderColor: "rgba(255, 201, 14, 1)",
            backgroundColor: "rgba(255, 201, 14, 0.5)",
            fill: false,
            lineTension: 0
        },{
            label: '전월세',
            pointRadius: 1,
            data: [1, 5, 12, 16, 17, 7, 6, 10, 4, 9, 2, 6, 6, 7, 6, 15, 6, 20, 9, 5, 3, 6, 7, 5, 4, 6, 9, 9, 6, 15, 7, 6, 4, 4, 3, 4, 3, 9, 6, 17, 6, 17, 5, 3, 7, 0, 5, 3, 1, 6, 11, 7, 8, 5, 4, 7, 16, 13, 8, 5, 3],
            borderColor: "rgba(0, 141, 185, 1)",
            backgroundColor: "rgba(0, 141, 185, 0.5)",
            fill: false,
            lineTension: 0
        }
        ]
    },
    options: {
        responsive: true,
        title: {
            display: false
        },
        tooltips: {
            mode: 'index',
            intersect: false
        },
        hover: {
            mode: 'nearest',
            intersect: true
        },
        scales: {
            xAxes: [{
                display: true,
                scaleLabel: {
                    display: true,
                    labelString: '년/월'
                }
            }],
            yAxes: [{
                display: true,
                ticks: {
                    suggestedMin: 0,
                },
                scaleLabel: {
                    display: true,
                    labelString: '실거래 수'
                }
            }]
        }
    }
});

</script>
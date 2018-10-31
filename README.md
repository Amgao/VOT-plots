# VOT-plots
to generate the plots same/similar to the original VOT 2015/2016 papers

In vot-old, modify 'ranking_adaptation' in report/report_challenge.m (or report_article.m) to 'best' (min operation). Please see the 2nd paragraph in Sec. 3 of VOT 2015 paper for more details. 'Usepratical' can be set to false.

In vot-old, modify 'format = '%.3f'' in report/matrix2html.m.

In vot-old, modify  report/report_cache.m to accommodate the loading of cache files generated from other people.

In vot-old, 

打开fig，打开属性编辑器，导出设置到12cm*12cm，然后再调整页面，再设置打印预览，最后保存pdf

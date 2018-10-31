# VOT-plots
to generate the plots same/similar to the original VOT 2015/2016 papers

In vot-old, modify 'ranking_adaptation' in report/report_challenge.m (or report_article.m) to 'best' (min operation). Please see the 2nd paragraph in Sec. 3 of VOT 2015 paper for more details. 'Usepratical' can be set to false.

In vot-old, modify 'format = '%.3f'' in report/matrix2html.m.

In vot-old, modify  report/report_cache.m to accommodate the loading of cache files generated from other people.

In vot-old, 

In vot-toolkit-binary (2016), modify stacks/stack_vot2016.m to choose between 'ar' (report/report_ar.m) and 'ar_rank' (report/report_ar_rank.m).

In vot-toolkit-binary (2016), always set like this:

 - usetags = get_global_variable('report_tags', true);
 - usepractical = get_global_variable('report_ar_practical', false);
 - orderingplot = get_global_variable('report_ar_ordering', true);
 - hidelegend = get_global_variable('report_legend_hide', false);
 - arplot = get_global_variable('report_ar_arplot', true);
 - average = get_global_variable('report_ar_average', 'weighted_mean');
 - adaptation = get_global_variable('report_ar_adaptation', 'best');
 - sensitivity = get_global_variable('report_ar_sensitivity', 100);
 - alpha = get_global_variable('report_ar_alpha', 0.05);
 - table_format = get_global_variable('report_ar_table_format', 'accrob'); % joined, rankscores, accrob, fragmented
 - table_orientation = get_global_variable('report_ar_table_orientation', 'trackers'); % trackers, selectors, trackerscores, selectorscores

In vot-toolkit-binary (2016), modify report/plot_ar.m, report/plot_ranking, report/report_expected_overlap.m, report/report_overlap.m to get legends, ARrank plots, ARraw plots, EAO graph/curves, and AO curves.

打开fig，打开属性编辑器，导出设置到12cm*12cm，然后再调整页面，再设置打印预览，最后保存pdf

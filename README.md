# RacialWealthGap

This repo includes two csvs (scf.csv and forbes_400.csv) and a R file (Racial Wealth Gap Vizualization.R) that creates several visualizations in highcharteR – a R package that serves as a wrapper for highcharts.js. 

These visualization are outputted as HTML documents. There are two visualizations: 1) a visualization of overall wealth inequality in the US in 2019 and 2) a visualization of racial inequality in the US. 

The second visualization is actually a set of 6 prototype figures that are linked together. A user may navigate to all 6 figures through hyperlinks embedded in each visualization. 

Problems and notes: 
1) Figure 2b is the closest to what we discussed. However, I wonder if the data displayed is too confusing. Below I outline how the two variables are defined. It is a little weird (very very likely too weird).   
    
    * "Excess white net worth relative to demographic proportionality" = abs(df_quantiles$`White wealth if demographically proportional` - 
    df_quantiles$White
    
    * "Change in Black net worth needed for demographic proportionality" = df_quantiles$`Black wealth if demographically proportional` -
    df_quantiles$Black
    
2) It is difficult for a stacked bar graph to make sense. Figure 2b shows this. 
3) I like a lot about figure 2c. It is clear (especially if you remove two of the catergories) and it is pretty cool. 
4) I cannot find a way in highcharts for overlapped bars to also be grouped. Therefore, figure 2d shows all bars overlaid, but this chart does not use the 3d option so it is a lot less clear. 
5) Figure 2e may convey the change needed for wealth equality (while maintaining the class structure) most clearly. 

Overall, I believe that these charts do not as clearly "speak for themselves" as other charts tend to do (e.g., overall wealth inequality). I could imagine an interesting pairing of Figure 2c with a link to Figure 2e. 

# gr5206-homework-4-solved
**TO GET THIS SOLUTION VISIT:** [GR5206 Homework 4 Solved](https://www.ankitcodinghub.com/product/gr5206-homework-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94742&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;GR5206 Homework 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
In this homework you’ll explore transforming data with split/apply/combine and the plyr package.

Gross domestic product (GDP) is a measure of the total market value of all goods and services produced in a given country in a given year. The percentage growth rate of GDP in year t is

􏰎GDPt+1 −GDPt􏰏 100× GDP −100

An important claim in economics is that the rate of GDP growth is closely related to the level of government debt, specifically with the ratio of the government’s debt to the GDP. The file debt.csv on the class website contains measurements of GDP growth and of the debt-to-GDP ratio for twenty countries around the world, from the 1940s to 2010. Note that not every country has data for the same years, and some years in the middle of the period are missing data for some countries but not others. Throughout, use 3 significant digits for numerical answers!! (That is, signif(mydat,3) is your friend).

<pre>debt &lt;- read.csv("debt.csv", as.is = TRUE)
dim(debt)
head(debt)
</pre>
<ol>
<li>Calculate the average GDP growth rate for each country (averaging over years). This is a classic split/apply/combine problem, and you will use daply() to solve it.
<ol>
<li>Begin by writing a function, mean.growth(), that takes a data frame as its argument and returns the mean of the ‘growth‘ column of that data frame.</li>
<li>Use daply() to apply mean.growth() to each country in debt. Don’t use some- thing like mean(debt$growth[debt$Country==”Australia”]), except to check your work. You should not need to use a loop to do this. (The average growth rates for Australia and the Netherlands should be 3.72 and 3.03. Print these values.) Report the average GDP growth rates clearly.</li>
</ol>
</li>
<li>Using the same instructions as problem 1, calculate the average GDP growth rate for each year (now averaging over countries). (The average growth rates for 1972 and 1989 should be 5.63 and 3.19, respectively. Print these values in your output.) Make a plot of the growth rates (y-axis) versus the year (x-axis). Make sure the axes are labeled appropriately.
1
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ol start="3">
<li>The function cor(x,y) calculates the correlation coefficient between two vectors x and y.
<ol>
<li>Calculate the correlation coefficient between GDP growth and the debt ratio over the whole data set (all countries, all years). Your answer should be −0.1995.</li>
<li>Compute the correlation coefficient separately for each country, and plot a his- togram of these coefficients (with 10 breaks). The mean of these correlations should be −0.1778. Do not use a loop. (Hint: consider writing a function and then making it an argument to daply()).</li>
<li>Calculate the correlation coefficient separately for each year, and plot a histogram of these coefficients. The mean of these correlations should be −0.1906.</li>
<li>Are there any countries or years where the correlation goes against the general trend?</li>
</ol>
</li>
<li>Fit a linear model of overall growth on the debt ratio, using lm(). Report the intercept and slope. Make a scatter-plot of overall GDP growth (vertical) against the overall debt ratio (horizontal). Add a line to your scatterplot showing the fitted regression line.</li>
<li>There should be four countries with a correlation smaller than -0.5. Separately, plot GDP growth versus debt ratio from each of these four countries and put the coun- try names in the titles. This should be four plots. Call par(mfrow=c(2,2)) before plotting so all four plots will appear in the same figure.
(Think about what this shows: individual relationships at the country level are some- times concealed or ”smudged out” when data is aggregated over all groups (countries). This conveys the importance of careful analysis at a more granular group level, when such groupings are available!)
</li>
<li>Some economists claim that high levels of government debt cause slower growth. Other economists claim that low economic growth leads to higher levels of government debt. The data file, as given, lets us relate this year’s debt to this year’s growth rate; to check these claims, we need to relate current debt to future growth.
<ol>
<li>Create a new data frame which just contains the rows of debt for France, but contains all those rows. It should have 54 rows and 4 columns (print the dimen- sions of your data frame). Note that some years are missing from the middle of this data set.</li>
<li>Create a new column in your data frame for France, next.growth, which gives next year’s growth if the next year is in the data frame, or NA if the next year
2
</li>
</ol>
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
is missing. (next.growth for 1971 should be (rounded) 5.886, but for 1972 it should be NA. Print these two values.)

<ol start="7">
<li>Add a next.growth column, as in the previous question, to the whole of the debt data frame. Make sure that you do not accidentally put the first growth value for one country as the next.growth value for another. (The next.growth for France in 2009 should be NA, not 9.167. Print this value.) Hints: Write a function to encapsulate what you did in the previous question, and apply it using ddply().</li>
<li>Make a scatter-plot of next year’s GDP growth against this year’s debt ratio. Linearly regress next year’s growth rate on the current year’s debt ratio, and add the line to the plot. Report the intercept and slope to reasonable precision. How do they compare to the regression of the current year’s growth on the current year’s debt ratio?</li>
<li>Make a scatter-plot of next year’s GDP growth against the current year’s GDP growth. Linearly regress next year’s growth on this year’s growth, and add the line to the plot. Report the coefficients. Can you tell, from comparing these two simple regressions (from the current question, and the previous), whether current growth or current debt is a better predictor of future growth?</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>

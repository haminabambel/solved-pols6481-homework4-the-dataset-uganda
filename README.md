Download Link: https://assignmentchef.com/product/solved-pols6481-homework4-the-dataset-uganda
<br>
Download the dataset <strong><em>Uganda_ITN.txt</em></strong> which describes the behavior of nearly 2000 adult (ages 15-48) women in Uganda. Here is the codebook for this dataset:

Using this dataset, perform the following tasks:

<ol>

 <li>Estimate a probit model that uses the three continuous explanatory variables (<em>education</em>, <em>age</em>, and <em>altitude</em>) to predict whether women use insecticide treated mosquito nets. Show the results of your analysis. Identify which variables are statistically significant and explain their effects on <em>itn</em>.</li>

 <li>Plot the predicted probabilities that an individual used a mosquito net across the range of values of <em>age</em>; fix <em>education</em> and <em>altitude </em>equal to their mean or median values (be sure to state which).</li>

 <li>Re-estimate the probit model in 1., but drop the variable that had statistically insignificant effects and add three binary variables – <em>rural</em>, <em>pregnant</em>, and <em>infant</em>. Explain the effects of each variable.</li>

 <li>Plot the predicted probabilities that an individual used a mosquito net across the range of values of <em>age</em>; but now plot two lines – one with <em>rural</em> = 0 (18%) and the other with <em>rural </em>= 1 (82%).</li>

</ol>

Note that 10.4% of women in the sample were pregnant, and 18.4% of women in the sample had an infant at home; set <em>pregnant</em> and <em>infant </em>equal to their modes.

<ol start="5">

 <li>Create a new variable, <em>atrisk</em>, that combines women who are pregnant and women who have an infant at home. (You may use this line of code: data$atrisk = 1 – (1-data$pregnant)*(1-data$infant) )</li>

</ol>

Run one more probit model that uses <em>age</em>, <em>altitude</em>, <em>rural</em>, and <em>atrisk</em> to predict whether women use insecticide treated mosquito nets and show your results.

<ol start="6">

 <li>Using this last model, calculate the probabilities of using a mosquito net for a woman who (a) is not pregnant and has no infant, or (b) either is pregnant or has an infant at home. Fix the values of <em>age </em>and <em>altitude </em>at their means, set <em>rural </em>at its mode, and vary <em>atrisk</em> between = 0 and = 1. How does being at risk change the probability of using a mosquito net?</li>

</ol>

Download the dataset <strong><em>FERTIL2.DTA</em></strong> which describes the behavior of more than 4,000 adult (ages 15-49) women in Botswana (data were collected by a Michigan State University undergraduate student, David Heakins, from a 1988 Demographic and Health Survey). Here is a codebook for key variables:

<ul>

 <li><em>children</em>: number of children</li>

 <li><em>educ</em>: years of education</li>

 <li><em>urban</em>: whether the respondent lives in an urban ( = 1) or rural ( = 0) community</li>

 <li><em>electric</em>: whether the home has electricity</li>

 <li><em>catholic</em>: whether the respondent belongs to the Roman Catholic church</li>

 <li><em>protest</em>: whether the respondent belongs to a Protestant church</li>

 <li><em>spirit</em>: whether the respondent identifies as a Christian but has assimilated indigenous medical practices (<em>bongaka</em>) and religious practices (<em>badimo</em>), such as ancestral veneration [especially patriarchal ancestors], into their Christian beliefs</li>

</ul>

<ol start="7">

 <li>For the third and fourth variables shown above, calculate the average numbers of children in:

  <ol>

   <li>Residents of rural areas versus residents of urban areas; also answer what percent of homes are in rural areas and urban areas</li>

   <li>Homes with without electricity versus homes with electricity; also answer what percent of homes do and do not have electricity</li>

  </ol></li>

</ol>

According to <em>Wikipedia</em>, Botswana is a Christian majority nation (over 70% currently) however according to one article, “ancestral spirits form a very important part of the religious thought of most Africans…. The present tenacity and resilience of the African traditional ritual and spirituality posed a challenge.”

<ol start="8">

 <li>Estimate a linear regression model that uses the one continuous explanatory variables (<em>educ</em>) and five binary explanatory variables (<em>urban</em>,<em> electric</em>, <em>catholic</em>, <em>protest</em>, and <em>spirit</em>) to predict the number of children a woman has. Show the results of your analysis. Identify which variables are statistically significant and explain their effects on <em>children</em>.</li>

 <li>Assuming a linear relationship, plot the predicted number of children that a woman has across the range of values of <em>education</em> for two different types of areas: rural (<em>urban </em>= 0) and urban ( = 1).</li>

</ol>

Set the other binary explanatory variables (<em>electric</em>, <em>catholic</em>, <em>protest</em>, and <em>sprirt</em>) equal to zero. Beyond what value for <em>education</em> is a woman predicted to have zero <u>or</u> <u>fewer</u> children?

<ol start="10">

 <li>Re-estimate the regression model in 8. as a Poisson regression, keeping the same variables. Identify which variables are statistically significant and explain their effects on the number of <em>children</em>. Use techniques described in lecture to explain how a unit increase in an explanatory variable increases the mean number of children in <em>percentage</em></li>

 <li>Plot the nonlinear relationship between education and the number of children that a woman has for two different types of areas: rural (<em>urban </em>= 0) and urban ( = 1). Set the other binary explanatory variables (<em>electric</em>, <em>catholic</em>, <em>protest</em>, and <em>sprirt</em>) equal to zero. How does the effect shown here differ from the linear relationship assumed in 8. and displayed in 9.?</li>

 <li>Calculate predicted probabilities of the numbers of children for a woman with the median education level (<em>educ</em> = 7). Set three binary explanatory variables (<em>catholic</em>, <em>protest</em>, and <em>sprirt</em>) equal to 0, set the <em>urban </em>variable equal to 0.5, and vary the <em>electric</em> variable between 0 and 1.</li>

</ol>

In other words, perform the calculations of <em>mu</em> and <em>pr</em>(<em>y</em> = <em>k</em> | <em>mu</em>) <u>twice</u> to see the impact of electricity on fertility. Let <em>k</em> = 0, 1, 2, 3, 4, 5.
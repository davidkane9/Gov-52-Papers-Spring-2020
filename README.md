# Final Papers for Gov 1006 in Spring 2020

This repository contains the final papers for [Gov 1006: Models](https://www.davidkane.info/files/gov_1006_spring_2020.html) at Harvard University in the Spring of 2020.


[Miroslav Bergam](https://github.com/mirobergam) --- ([repo](https://github.com/mirobergam/Bergam-Zelizer-Replication-Paper) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Bergam_Replication.pdf)) --- Zelizer (2019) finds that the cues that legislators take from their peers, in addition to other credible sources of information like briefings, influence their policymaking decisions. I succesfully replicated Zelizer’s results. Zelizer took a Bayesian approach to his findings, running 10,000 simulations for each table and figure using for-loops to produce estimates and standard deviations; however, this made his code inefficient and extremely slow Using the rstanarm package, I was able to simplify his code while maintaining the Bayesian integrity of the study. This extension served as both a robustness test of his results and a simplification that makes the study more easily reproducable.

[Maria Burzillo](https://github.com/mburzillo/) ---([repo](https://github.com/mburzillo/Segregation-and-Public-Goods-Final) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Burzillo_Trounstine_Replication.pdf)) --- Trounstine (2016) suggests that high levels of residential segregation are associated with increased political polarization and decreased public goods spending. In this analysis, I was able to successfully replicate Trounstine (2016)’s main results. I then attempted to better deal with the large amounts of missing data in the datasets used in the original analysis by multiply imputing missing values and re-running the original models using the resulting multiply imputed datasets. My results suggest that segregation is associated with increased racial political polarization, although maybe not as strongly as Trounstine (2016) originally suggested. Furthermore, I find that Trounstine (2016)'s conclusion that increases in segregation are associated with decreases in public spending holds for large cities, but that diversity is a better explanatory factor for small cities. 

[Evelyn Cai](https://github.com/caievelyn) --- ([repo](https://github.com/caievelyn/voter_preferences_replication/) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Cai_voter_preferences.pdf)) --- Horiuchi, Smith, and Yamamoto (2020) found through differences between observational data and their conjoint survey results that Japanese voters' voting preferences are dependent on external factors. The conjoint survey results yielded consistent voter preferences across priming on different electoral systems; however, observational data and theoretical explanations show that voters' preferences do vary across electoral systems. I was able to successfuly replicate these results and findings. My extension focuses on examining the difference in marginal means instead of the difference of average marginal component effects, which avoid setting an arbitrary baseline when calculating treatment effects.  

[Molly Chiang](https://github.com/mollyechiang) --- ([repo](https://github.com/mollyechiang/gender_edu_voting) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/chiang_edu_and_voting.pdf)) --- Marshall (2015) shows the causal effect of additional years of schooling on voting conservative in his analysis of voting records before and after the British 1947 school-leaving age reform. I successfully replicated Marshall's code, except an update in the rdrobust package led to slightly different coefficients. In an extension of Marshall's work I investigated treatment effect heterogeneity between genders. Running rdrobust and creating regression discontinuity figures on male and female subsets of the data revealed Marshall's effect of more years of education increasing the likelihood of voting conservative was stronger in women than men. This finding could complicate Marshall's argument that more education leads to higher income then to more conservative political opinions and perhaps reveals something about the differing effect of education on men and women.

[Ali Crump](https://github.com/alicrump) --- ([repo](https://github.com/alicrump/Fentanyl_Replication_Project) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Crump_fentanyl.pdf)) --- Zoorob (2019) shows that geography and fentanyl exposure explain much of the variation in increased overdose mortality rates between 2011 and 2017. I successfully replicated much of Zoorob's results, but I found discrepancies in the fentanyl exposure coefficients and the total death estimates for each model. My replication finds that the total death estimates are approximately 13% and 16% larger for each model and that the regression coefficients on fentanyl are slightly larger than those published. In addition to replicating Zoorob’s work, this paper provides a Rubin causal model table to better understand the model framework, focusing on explaining the ordinary least-squares model. Next, the bulk of the extension investigates alternative definitions of fentanyl exposure while keeping all of Zoorob’s other modeling choices the same. The original paper's definition of fentanyl exposure explains more variation in age-adjusted mortality rates than those proposed in the extension. This finding is important because many different methods of defining fentanyl exposure exist, however, the proposed alternative definitions in this extension do not appear to improve Zoorob's model.

[Drake Deuel](https://github.com/ddeuel) --- ([repo](https://github.com/ddeuel/Bikeshare-Replication) [pdf](https://github.com/davidkane9/gov_1006_spring_2020_papers/papers/bikeshare_deuel.pdf)) --- Fuller et al. (2019) claimed that the disruption in public transit services caused by Philadelphia's transit workers strike from November 1-7th led to a short term increase in bikeshare use in Philadelphia when controlling for temperature, precipitation, and bikeshare use is similar cities during the same time. I successfully replicated Fuller's results. I recreated the interrupted time-series model that the authors used to model this natural experiment, and the Bayesian time-series model using the CausalImpact R package. I used the same raw data to with these structures to model bikeshare use per 100k population in Philadelphia. The models indicate that while the disruption to normal transit availability caused short term increase in bikehsare usage, usage returned to baseline within a short period. This may inform policy makers that short term interventions to promote cycling in cities may not have long term impacts.

[Angela Fu](https://github.com/angelafu7) ---
([repo](https://github.com/angelafu7/CrossingTheLineReplication) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/fufinalpaper.pdf)) --- In their paper "Crossing the Line: Local Ethnic Geography and Voting in Ghana," Nahomi Ichino and Noah Nathan found that the local ethnic demographics of the area in which Ghanian voters live affected who they chose to support in the 2008 Ghana presidential election. I successfully replicated Ichino's and Nathan's results. I have also reexamined their models and added an additional variable to explore the effect of a voter's trust in members of their own ethnicity. I found that the inclusion of this variable does not significantly alter the model. As a result, trust in one's co-ethnics or in others of a different ethnicity do not impact one's voting decisions as much as the demographics of one's location do.  

[Michelle Gao](https://github.com/michgao87) --- ([repo](https://github.com/michgao87/tech-politics-replication) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/gao_tech_politics.pdf)) --- Broockman, Ferenstein, and Malhotra (2019) show that technology entrepreneurs have a unique set of political beliefs: they are liberal on social issues, globalism, and redistribution, but very conservative on government regulation. The replication succeeded with the exception of some discrepancies in scaling variables. An extension that used linear regression to formally test whether certain values or predispositions, such as cosmopolitanism and authoritarianism, could predict policy preferences in particular domains, such as support for globalism and social issues, added support to the authors' ultimate claim that tech entrepreneurs' unique political beliefs stem from unique underlying philosophical values. Analyzing technology elites' political beliefs is an increasingly timely task as the tech industry becomes more influential in politics.

[Debora Gonzalez](https://github.com/deboragonzalez) --- ([repo](https://github.com/deboragonzalez/gop_voters_hisp_changes) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/GonzalezDebora_gop_voters_hisp_changes.pdf)) --- Hill, Hopkins, and Huber (2019) argue that demographic changes are not associated with increased Republican vote share at the precinct level between 2012 and 2016. I succesfully replicated Hill, Hopkins and Huber’s results. A robustness test using a subset analysis focusing on the state of FL indicates, despite minor state-specific deviance and poor statistical significance due to reduced sample size, that the authors' overall findings are valid. Another test focusing on the effect of any individual state on the overall outcome was also found to support the original paper's robustness. In addition, I constructed a fixed effects model by state, which further confirmed original findings even under fixed effects assumptions. In a twist of analysis, I constructed a new model analyzing the association between Republican vote share and economic indicators while controlling for change in percent Hispanic. The latter models indicate a stronger relationship between unemployment proportion change and GOP vote share, which suggests an opportunity for further research with alternative theoretical pathways involving economic indicators. 

[Carine Hajjar](https://github.com/carine-h)---
([repo](https://github.com/carine-h/replication-project)
[pdf](https://github.com/carine-h/replication-project/blob/master/final_project_carine_hajjar.pdf))--- Barber and Pope (2018) show that most Republicans operate according to party loyalty over policy (ideological) loyalty. I successfully replicated Barber and Pope's results. The results of the paper and the replication indicate that Republican party loyalists vote in line with President Trump, regardless of the political content of Trumps's cues. More specifically, Republicans with low political knowledge, high self-ranked ideology, high partisanship, and high approval of Trump are more likely to support their leader's cues, regardless of the true ideological implications, even if they are not in line with the party's traditional views. I looked at Barber and Pope's regressions testing the causal effect of conservative and liberal cues from President Trump on Republican, Democrats, and Independents with varying levels of political knowledge, partisanship, approval of Trump, and political ideology. I took the regression on partisanship and knowledge as well as the overall regression of average cue response among all political identities and ran a more robust binomial regression as well as corrected for a mistake in the first figure of the paper. I reiterate the fact that Republican party loyalists are not necessarily ideological loyalists and, more specifically, that many Republican Trump supporters respond positively to liberal or conservative cues from Trump but not necessarily from other Republicans. This finding forces Americans to rethink the importance of parties and the ideological strength of their positions. 

[Benjamin Hoffner-Brodsky](https://github.com/ben-hb) --- ([repo](https://github.com/ben-hb/development_without_representation_replication) [pdf](https://github.com/ben-hb/development_without_representation_replication/blob/master/milestone_4.pdf)) --- I'm replicating Jensenius (2015) *Development from Representation*, which appeared in the *American Economic Journal: Applied Economics*. Since 1950, the Indian Parliament and India's state assemblies have guaranteed a minimum number of seats to Scheduled Castes (SCs). Ensuring ascriptive representation for the 16% of Indian citizens who belong to SCs was intended, in part, as a mechanism to equitably allocate resources along caste lines. To implement SC quotas, the federal government non-randomly selected constituencies in which only SC members can run for office, though all members of the constituency are allowed to vote. The paper uses a dataset of constituency-level data of 3,134 state assembly constituencies from the 15 largest Indian states to compare development levels across reserved and non-reserved constituencies in 1971 and 2001. As reserved constituencies were non-randomly determined, Jensenius forms pairs of reserved and non-reserved constituencies, matching based on pre-selection characteristics to mitigate the effect of selection bias. She finds a null constituency-level effect on overall development, redistribution to SCs, literacy rates, SC employment patterns, and village amenities.

[Suriya Kandaswamy](https://github.com/sardination/) --- ([repo](https://github.com/sardination/policy-responsiveness) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Kandaswamy_Policy_responsiveness.pdf)) --- Caughey and Warshaw (2018) show that in American states, dynamic responsiveness of policy liberalism to mass liberalism has increased over the years and, further, that partisan control in any given year has a minimal effect on the liberalism of that year’s policy. Replication of results was successful, except for some discrepancies in the magnitude of coefficients, which do not affect their main conclusions, but do affect some marginal conclusions drawn. While this paper focuses on the impact that different features of public opinion, geography, and legislative partisanship have on policy, this extension sought to determine whether partisan control of a state’s legislature impacts the responsiveness of its policy to public opinion. In other words, while the party in control may not have a large impact on the liberalism of implemented policy by itself, this extension shows that the party in control has a noticeable short-term effect - through variable interaction - on how responsive policy liberalism is to mass liberalism for economic issues but has a negligible long-term effect for all types of issues. Regardless of what party is in power in any state, or the country for that matter, it is important that the policy of an administration reflects the wants and needs of its populace and it should be clear that policies evolve with the needs of the people rather than the wants of the party.

[Alexander Klueber](https://github.com/Alex1005-stack) --- ([repo](https://github.com/Alex1005-stack/Website_replication) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Klueber_website.pdf)) --- 
Pan (2017) shows that the emphasis on Chinese local government websites on either the competence or benevolence of county executives depends on where they are in the political tenure cycle. I was largely able to replicate these results. My extension confirms that this is the most likely explanation for the observed effect by comparing the statistical explanatory power of alternative models (e.g. cultural differences among regions, gender differences, etc.) through the leave one out method. In addition I validate the geographical randomness of the sample through simulations of repeated sampling and the construction of confidence intervals. They corraborate the findings of the paper by confirming the geographic randomness of the sample.

[Samuel Lowry](https://github.com/SamuelLowry) --- ([repo](https://github.com/SamuelLowry/why_friends_and_neighbors_replication_paper) [pdf](https://github.com/SamuelLowry/why_friends_and_neighbors_replication_paper/blob/master/milestone-8.pdf)) --- Campbell et al. (2019) details two separate experiments which suggest that individuals think of politicians with local roots and that exibit behavioral localism more highly. I was able to replicate the entire article with the exceptions of table 1 and figure 2 because they visuals relating to methodology and not the results themselves. I will be conducting an extension which includes the use of stan_glm instead of lm as well as look at certain subgroups based upon location and party identification. I hope to find cool things:)

[Chelsea Marlborough](https://github.com/chelseamarlborough) ---([repo](https://github.com/chelseamarlborough/marlborough_final) [pdf](https://github.com/chelseamarlborough/marlborough_final/blob/master/marlborough_final.pdf)) --- Stokes (2015) finds that voters do pay attention to climate policy and afterwards penalize the incumbent governments for facilities viewed as harmful to the communities.

[Diego Martinez](https://github.com/diegomartinez1221) --- ([repo](https://github.com/diegomartinez1221/local_roots_replication)  [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Martinez_local_roots.pdf)) Campbell et al. (2019) find evidence that local roots serve as a cue for behavioral information; however, they still find local roots to possess a positive impact on candidate selection. I was successfully able to replicate all the results presented in the original article "Why Friends and Neighbors? Explaining the Electoral Appeal of Local Roots." by Rosie Campbell, Philip Cowley, Nick Vivyan, Markus Wagner. To further their analysis, I modeled how local roots influence different sub-populations, including male vs. female voters, as well as between different age groups. I found the average treatment effect of local roots are not constant across subsets of the population. Furthermore, I found the average marginal effect of local roots to have substantial differences between males and females. Local roots affect groups of voters differently and any further research regarding local roots should account for demographic differences.  

[Liz Masten](https://github.com/LizMas) ---
([repo](https://github.com/LizMas/terrorism_rivalries_replication)
[pdf](https://github.com/LizMas/terrorism_rivalries_replication/blob/master/masten_fpy_replication.pdf)) ---
Findley, Piazza, and Young (2012) show that interstate rivalries are a positive predictor of transnational terrorist activity. The authors argue that terrorism is often a component of broader hostilities that can be emperically analyzed using a series of politicaly relevant directed dyads. In this paper, I successfully replicated all of their results and executed an extension which used dyadic quasipossion models. These models are equally statistically significant with respect to rivalry, the main concern of the original paper, and thereby confirm that the original findings are robust. However, concerns exist regarding the use of dyadic analysis and the conclusions we can draw from such analysis in general.    

[Beau Meche](https://github.com/BeauMeche) --- 
([repo](https://github.com/BeauMeche/enforcement_distribution_electorate)
[pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Meche_politics_dist_rep.pdf)) --- "The Distributive Politics of Enforcement" by Alisha Holland (2014) analyzes electoral behavior's relationship with police action in opposition to low-income unlicensed street vendors in three cities in Latin America. I was successful in replicating the results, with minute variance due to apparent differences between regression output between R and Stata. In my extenstion I re-regressed the models from the original paper under Bayesian modeling methods in the interest of discovering any differences likely to arise. The regression outputs themselves were quite similar and model comparisons favored similar models to the author; however upon cross-validation model analysis I found that a majority of the models did contain 'problematic' values. This implies that the models showing statistically significant support for the author's claim do not effectively model a subset of specific cases should any one case be removed. Should this prove to be a problem, it is only a problem of outliers which are not surprising in a small dataset. Otherwise, I find that Bayesian analysis supports Holland's claims both in conclusion and in process.

[Robert McKenzie](https://github.com/rmckenzie11) --- ([repo](https://github.com/rmckenzie11/https://github.com/rmckenzie11/Calvo_Rodden_-2015-_replication_and_extension) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/McKenzie_Geography_Represenatation.pdf)) --- "The Achilles Heel of Multiparty Democracies", by Ernesto Calvo and Jonathan Rodden (2014) shows that majoritarianbiases increase with the number of parties, and majoritarian systems harm small parties when their vote is more dispersed than average, and large parties when their vote is more concentrated than average. They built a mathematical model of the relationship between geographic distribution and electoral representation, using MC methods, and then analyzed UK elections over the past 60 years to determine which parties benefit from majoritarian bias. I've extended their paper by updating data, and adjusting specifications to look at the impact of regional parties. 

[Prachi Naik](https://github.com/prachiknaik) ---
([repo](https://github.com/prachiknaik/violent_protest_and_policy_change)
[pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/naik_eks_replication.pdf)) ---
Enos, Kaufman, and Sands (2019) show that the 1992 Los Angeles Riot— one of the most well-known and documented instances of political violence in recent American history— caused a significant liberal shift in policy support at the polls due to the increased mobilization of Black and White voters, a mobilization that has endured over a decade later. The replication attempted in this project successfully found that White voters demonstrated a 0.028 increase in support for public school funding relative to university funding (CI: [0.018, 0.039]) and Black voters demonstrated a 0.073 increase (CI: [0.066, 0.081]). To extend the work of this paper, this project sought to examine the effects the Riot had on Asian American voters. The findings were inconsistent with what the authors found for White and Black voters-- the riot appears to have caused a decrease in liberal policy support for Asians. This matters because heterogenous treatment effects are worth further scrutiny and complication, especially given climates of racial polarization.  


[Alexandra Norris](https://github.com/asnorris) --- ([repo](https://github.com/asnorris/Norris_EKR2017_Replication)
[pdf](https://github.com/asnorris/Norris_EKR2017_Replication/blob/master/Norris_Replication_Paper.pdf)) --- Ejdemyr, Kramon, and Robinson (2017), show that ethnic segregation is a key determinant in whether ethnic favoritism plays a role in the provision of public goods.  I was able to successfully replicate the authors' results. For my extension, I used the same models as for the replication except instead of using boreholes (wells) as my proxy for public goods provision as the authors did, I used health clinics and schools. When using these other dependent variables, I found that the effects of segregation were different from those presented in the paper. 

[Cris Patvakanian](https://github.com/cpatvakanian) --- ([repo](https://github.com/cpatvakanian/Vote_Brokers_Replication) [pdf](https://github.com/cpatvakanian/Vote_Brokers_Replication/blob/master/Replication.pdf)) --- Frye, Reuter and Szakony (2019) examine voter behavior in Russia and Venezuela and find different types of brokers, appeals, and targets have different effects on voter turnout. I successfully replicated all of their results. As a robustness test, I impute missing values in the dataset and find results in line with that of the original study, but of a slightly different magnitude. These results confirm the authors' original findings and suggest that the missing values in their sampled population do not bias the results. All analysis for this paper be found in the [original paper](https://www.cambridge.org/core/journals/world-politics/article/vote-brokers-clientelist-appeals-andvoter-turnout-evidence-from-russia-and-venezuela/45FE0BE1216FCD8744B02A82919B328A) and [data verse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YSVMS2).

[Pieter Quinton](https://github.com/PGQuinton) ---  ([repo](https://github.com/PGQuinton/gov1006-finalproject-2.0) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/quinton_unemployment.pdf)) --- Bauer (2018) finds that there is no consistent relationship between unemployment and one's trust in government or their satisfaction with democracy. I succesfully replicated Bauer's results except for a minor disprepency in a summary table which does not affect his conclusion. My extension evaluates how consistent or long-term unemployment may impact one's views. Rather than examining the effects of just a single year of unemployment, as Bauer did, I track unemployement trends over longer periods of time to see if extended periods of unemployment have a stronger impact on one's feelings towards the government and its institutions than shorter periods of unemployment do.

[Timothy Ravis](https://github.com/soetimno) --- ([repo](https://github.com/soetimno/ravis_1006_final_project.git) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Tim_Ravis_Deforestation_and_Titling.pdf)) --- Buntaine, et al (2015) find that donor-financed, government-implemented land tenure legalization efforts in forested areas have a negligible effect on the rate of deforestation versus that found in areas not subject to such an intervention. After matching treated plots with untreated ones, they find no significant treatment affect on deforestation rates. The major results of their analysis were successfully replicated in this study. In the present paper, I explore how spatial autocorrelation in both the treatment and the outcome affects the treatment effect found by the original authors. This illustrates the importance of including spatial relationships into models attempting to explain causality within explicitly spatial datasets.

[Niel Schrage](https://github.com/nschrage) --- ([repo](https://github.com/nschrage/schrage_replication) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/schrage_replication.pdf)) --- Enos (2016) measures the shift in voter turnout for white voters living in Chicago near demolished public housing, occupied predominantly by African Americans, as compared to white voters living farther away; observing that white voters living in close proximity to demolished public housing had a 10 percentage point drop in voter turnout between 2000 and 2004, Enos concludes that this change in behavior was the result of the decline in race threat from the change in size and proximity of the outgroup population. The results of my replication effort were largely successful, although there were some challenges. For my extension, I expanded the parallel trends robustness check that Enos presents in his appendix; my results were consistent with his findings. These results are significant in two important ways: first, they illustrate the strength of the robustness checks that Enos conducted and, second, they suggest that his conclusions about the effect of racial threat on voting are even more robust than his paper suggests.

[Daniel Shapiro](https://github.com/dfshapir) --- ([repo](https://github.com/dfshapir/Replication) [pdf](https://github.com/dfshapir/Replication/blob/master/Shapiro_Chechnya.pdf)) --- Lazarev (2019) uses data describing individuals’ choice between Russian state law, sharia law and customary law (adat) in Chechnya to show that gender can play a large role in societal splits in post-conﬂict societies. I was able to replicate all of the author’s results. In my extension to Lazarev’s paper, used the rstanarm package in R to check Lazarev’s analysis with Bayesian regression, and the results conﬁrmed the author’s ﬁndings. I also pointed out certain areas where I disagreed somewhat with Lazarev’s analysis and where I felt that the paper could improve. This paper’s successful replication of Lazarev’s ﬁndings helps strengthen Lazarev’s argument about the role of gender in choice of legal organ, and my additional comments on Lazarev’s anaylsis help to further discussion about postwar Chechnya and post-conﬂict society as a whole.

[Mike Silva ](https://github.com/mikesilva23) --- ([repo](https://github.com/mikesilva23/replication_1006) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/SilvaPaper.pdf)) --- Tingley et al (2014) find that olfactory senses could explain assortative mating by ideology. My replication of this paper succeeded in most cases. It failed in a few ways including clustering standard errors around certain variables and recreating graphs that used 21 specific observations from the data set. Through my extension, I evaluate one of the three models Tingley et al uses by using a bayesian fit instead of a regular linear model. I further create a posterior distribution of predictions on the outcome variable using the model and graph those predictions with the actual outcome values. Through this model, I confirm that Tingley's model significantly explains the data.  

[Cian Stryker](https://github.com/CianStryker) --- ([repo](https://github.com/CianStryker/Prosocial_Behavior) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Stryker_Prosocial_Behavior.pdf)) --- Hager, Krakowsi, and Schaub (2019) find that exposure to ethnic violence negatively affects prosocial behavior within and across ethnic groups in Osh, Kyrgyzstan. I was largely successful in replicating their main results and use their survey data of Kyrgyz and Uzbeks—the majority and minority ethnic groups of Osh—to expand upon their work. I find that the prosocial behavior of Kyrgyz towards Uzbeks is partially positively affected by exposure to violence. These results contradict the authors’ original findings that exposure to ethnic violence has a homogenous treatment effect. My models demonstrate that on the contrary, ethnic violence can have a heterogenous treatment effect, which warrants further analysis of ethnic violence’s influence on interethnic relations.

[Amanda Su](https://github.com/amanda-y-su) --- ([repo](https://github.com/amanda-y-su/race-writing-computation) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Su_RaceComputation.pdf)) --- So, Long, and Zhu (2019) determine that novelists marked as "white" versus "black' produce different narratological effects with respect to the interaction of race and religious authority, finding that black writers who cite the Bible are more likely to cite it in a social context compared to white writers who cite the Bible in their novels. I was able to successfully replicate the results of the authors' paper. For my extension, I decided to reconstruct the paper's primary model using a Bayesian approach. I found that the results of the model were largely the same as that of the original. This corroborates and strengthens the paper's conclusions about how race and writing intersect across more than a century of U.S. fiction.

[Abrar Trabulsi](https://github.com/abrartrabulsi) --- ([repo](https://github.com/abrartrabulsi/finalproject1006) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Trabulsi_Abrar_FinalDraft.pdf)) --- In his paper 'The Desire for Social Status and Economic Conservatism among Affluent Americans', Thal (2020) shows that affluent American's desire for social status drives conservative attitudes amongst them, and the will to advance economically conservative politics. Overall, I was successful in my replication efforts in this paper. Moreover, I extend Thal's results by running logistic regression and appropriate analysis, such a distribution of the posterior and predictive probabilities on his primary data. I find that Thal was indeed correct. Social status does in fact drive conservative attitudes amongst affluent Americans, and especially men.

[Hannah Valencia](https://github.com/h-valencia) --- ([repo](https://github.com/h-valencia/Firearms-Replication) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Valencia_Firearms.pdf)) --- Levine and McKnight (2017) show that in the 5-month period following the Sandy Hook school shooting in December 2012, a large spike in gun sales contributed to an increase in accidental firearm deaths. Their findings conclude that there was a spike in accidental firearm deaths resulting from the increase in exposure, which is confirmed in this replication. I was able to successfully replicate most of Levine and McKnight's results. As an extension to this paper, the original linear regression used to determine the increase in firearm sales per 100,000 popoulation in the post-Sandy Hook period was changed to a Bayesian generalized linear model. Even after this change, the results showing increases in certain states hold, backing the authors' claims.  Even though the Sandy Hook shooting showed the need for stricter gun laws, the immediate aftermath of this realization led to the opposite effect as desired: more accidental firearm deaths.

[Kevin Wang](https://github.com/kevpwang) --- ([repo](https://github.com/kevpwang/replication_project) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/wang_draft.pdf)) --- Hopkins (2015) finds that exposing a nationally representative sample of Americans to video of an immigrant speaking accented English causes the respondents to adopt more inclusionary attitudes. I successfully replicated Hopkins’s results, except for a minor manipulation check and the composite immigration index. As an extension, I modified the original regression by adding respondents’ self-reported familiarity with Spanish in real life. I found that respondents who reported more frequent encounters with Spanish tended to hold more restrictionist views. This result suggests the difficulty of changing exclusionary attitudes developed through long-term contact with culturally distinctive traits in daily life.


[Feven Yohannes](https://github.com/fyohannes) --- ([repo](https://github.com/fyohannes/Milestone_8) [pdf](https://github.com/fyohannes/Milestone_8/blob/master/Rough-Draft-.pdf)) ---   Kuipers (2019) explores the effect that the election of female candidates in the Indonesian legislature have on intimate partner violence attitudes. I replicated Nicholas Kuipers' paper “The Effect of Electing Female Candidates on Attitudes Towards Intimate Partner Violence” and I found my results to be consistent with the results found in the paper. After running the code from the main models, I concurred that the results showed that the election of female candidates did, in fact, have an effect that’s statistically significant on the IPV attitudes on female constituents. These results are particularly important because it shows the possible effect that female candidates can have on decreasing IPV, by at least contributing to more condemnation of IPV. Thus, the election of female candidates can result in tangible responses to IPV, leading to safer and healthier communities for women.


[Yao Yu](https://github.com/itsyaoyu) --- ([repo](https://github.com/itsyaoyu/mass-shooting-intervals) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/yu_mass_shooting_intervals.pdf)) --- Lin et al. (2018) found that the time interval between mass shootings has been drastically decreasing in the past three decades, suggesting that the rate of shootings is increasing. I was able to replicate all of the results from Lin et al. (2018), but while I was able to replicate the inconclusive results in table 1, I was not able to replicate the exact zero-inflated Poisson model. My extension broke down the interval trends between different venues of shootings showing in figure 2 of Lin et al. (2018). I found that the interval trend of mass school shootings remained relatively steady while the interval between mass workplace shootings and other mass shootings drastically decreased since 2015. This suggests that more research should be done looking at why workplace mass shootings have specifically increased drastically since 2015.

[Ruth Zheng](https://github.com/zhengruth) --- ([repo](https://github.com/zhengruth/replication_renters_paper_1006) [pdf](https://github.com/GOV-1006-Spring-2020/papers/blob/master/papers/Zheng-Ruth-Renters-Paper.pdf)) --- Hankinson (2018) shows that renters exhibit “Not in My Back Yard” (NIMBY) behavior on par with homeowners in high-rent cities despite overall support for a housing supply increase. I successfully replicated Hankinson’s results and confirmed they are consistent with results using a logistic regression model. The increased likelihood for these renters to reject policy proposals that create new housing helps explain the affordable housing crisis in major American cities



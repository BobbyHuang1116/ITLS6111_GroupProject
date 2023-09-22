# ITLS6111_GroupProject

## Project requirement
Project Brief
COVID-19 has created long-lasting impacts on the retailing sector. During the lockdown period 2019-2020, the pandemic had created a great opportunity for eCommerce when shoppers avoided malls and shopping centres in favour of online shopping. Emerging evidence suggests that while 15% of retail dollars were spent online in 2019, eCommerce is now expected to make up 22% of global retail sales, according to the Australia Post eCommerce Industry Report (Australia Post, 2020) and Ecommerce Research (Big Commerce, 2022). Thus, while the COVID-19 lock-downs in 2020 and 2021 had seen a few retailers considered closing their stores (Elmas, 2021), the ‘new normal’ has seen more foot traffic in major shopping centres. This new trend brings back brick-and-mortar stores. 
A retail chain in NSW is planning for this new trend. It plans to adjust their footprint (i.e., closing low-performing stores and setting up new stores in good locations), while ramping up online sales by investing in online as well as fulfilment and delivery services. The company has hired your group as consultants to analyse its sales data and come up with a plan to adjust physical shops, while increasing internet presence to capture new trend in online shopping. The retailer aims to close two low-performing stores, setting up one new store in NSW/ACT and invest more in fulfilment and delivery services. The retailer also wants to reduce logistic costs as much as possible. To accomplish these objectives, you will need to do the following:

Sales
•	Use the historical sales data across all shops, and the socio-economic and business indicators for the areas in which these shops are located to determine the performance of each shop relative to other shops. This process is known as benchmarking, a practice that typically uses modelling, such as a regression model. Benchmarking is, in essence, comparing the performance of each shop against the “average shop” or ranking the shops according to their sales, considering the demographic and economic settings in which the shop operates so that a like-for-like comparison can be made. Failing to account for differences in demographic and economic settings, any companion would not be very meaningful because without doing any analysis, we can say, with fair confidence, that a shop located in a busy area such as the CBD would perform better than a shop in regional area, simply because there are more potential customers in the former area. 
•	Based on your benchmarking above, identify 2 low-performing shops in NSW/ACT (Australian Capital Territory) for closure and one good location in NSW/ACT for setting up a new store. That is, the total number of brick-and-mortar stores will reduce by one. 

Logistics and distribution
•	Following the adjustment of brick-and-mortar stores, the company considers moving its distribution centres to serve the remaining shops better and to reduce logistic costs, of which transportation and inventory cost are the major components. You must identify the optimal number and location of new distribution centre(s) in NSW/ACT, assuming that (1) online sale quantities will increase by 40%, according to ABS Retail Trade report (2022), and (2) sale quantities of each of the remaining/new shops will increase by 15%, compared to the quantities recorded in the sales dataset. 
•	To help you locate new distribution centre(s) in the metropolitan area of NSW/ACT, the company provides your team with the list of candidates for Distribution Centres (DCs) in NSW as follows:

Table 1. Candidate locations for DC in NSW and unit renting cost (per month)
Address	Rent cost/m2
Grevillea Street Eastern Creek NSW 2766	$150
Blackbird Close NSW 2171	$200
Moorebank Logistics Park NSW 2170	$190
Clunies Ross Street Greystanes NSW 2145	$165
Wonderland Drive Eastern Creek NSW 2766	$140
Monaro Industrial Park in Hume, ACT 2620	$130

If a DC is required outside the metropolitan area of NSW/ACT such as in Albury – the border town of NSW and Victoria states, you are free to select any suitable location as DC and assume a unit rent cost of $100 / m2 per month.
•	Develop a routing plan which includes (i) identifying the number of vehicles, (ii) type of vehicle, and (iii) delivery schedule for servicing the brick-and-mortar shops in New South Wales/ ACT. You should justify why your routing plan is optimal, with consideration for how the company best fulfill the increasing online sales. 

Core datasets
To help you with your analysis and recommendations, the company provides the following datasets. Keep in mind that the datasets were provided by different consultants. They may contain errors and inconsistencies.

a)	One year of weekly sales data for all locations for over 1,000 products including toys, health and beauty, and home decoration (sales dataset NSWsales.csv)
b)	A Network Dataset for main roads in NSW (stored inside the MainRoads_NSW.gdb)
c)	Location of current retail shops of the company (NSW_shops_location)
d)	Geographic layers representing Central Business District (CBD) areas (AustralianCBD)
e)	Selected Person Characteristics (SPCA) at the SA2 level for all of Australia (SA2_Australia_SPCA_2021). See the Metadata_2021_GCP_DataPack_R1.xlsx for the meaning of shortened field/variable names.
f)	Selected medians and means at the SA2 level for all of Australia, including the number of Motor Vehicle (MV) per dwelling (SA2_Australia_selected_medians_means_2021)

Data items c – f can be found inside the GroupProject_SpatialData.gdb. ABS data from 2016 Census are included in this database too, but you should use data from the 2021 Census. 

Apart from the core datasets above, you can use any other data, including the data provided to you in this unit and those you find on the Internet (you don’t need to). You must include a section in your report detailing the sources of each dataset you use. You can download ABS 2021 DataPacks by clicking on the hyperlink, some of which I have processed and included in the GroupProject_SpatialData.gdb.

Assumptions
The company has several constraints that you must allow for in your analysis and routing plans. These cannot be changed.

•	Distribution centres are open from 05:00 to 17:00
•	Retail shops accept deliveries between 07:00 and 17:00 unless they are in the CBD where deliveries can only be made between 05:00 and 07:00 and from 13:00 to 15:00
•	Fuel cost 235 cents/Litre for Diesel
•	Fixed time: 12 minutes (fixed amount of time required by the truck driver each time he serves a shop)
•	Unit time: 0.3 minutes per unit (e.g., a delivery of 100 units will take 0.3 * 100 = 30 minutes)
•	To reduce maintenance and training costs, only three types of vehicles are used by the company to make deliveries, with the following characteristics: 
Table 2. Truck characteristics
Type	Capacity (units)*	Purchase Cost	Fuel efficiency (L/100km)
Articulated	250	$250,000	55
Large Rigid	60	$90,000	32
Small Rigid	40	$70,000	22
Note: * Capacity is defined by the maximum number of units of the products included in the sales dataset that each vehicle can carry at a time.


Project Deliverables

Presentation: 10%
A group presentation of 10 minutes max. Each team members must present/speak to gain marks. You should use the rubric for Presentation below to guide the structure of your presentation. 

What should you cover in your presentation?
You should assume you are presenting your findings and recommendations to the management of the retail company that has contracted your group to provide the consulting service. You should provide an overview of the problem, how you approached the problem and the justification for it, your major findings, and recommendations. There are no hard and fast rules on how to do this – that is the challenge for you to solve. The main thing you need to think about is what message do you want your client to take away? Remember that you only have 10 minutes to get your message across – choose your most important findings to present instead of trying to present everything you have done in 10 minutes. When marking your presentation, the following rubric will be used: 
Structure: 4
•	Coherent and logical structure to the presentation? Introduction, Methods, Results/Analysis, Conclusions/Recommendations Kept within time limits?
•	Evidence of teamwork rather than a series of individual presentations?
•	Quality and use of slides to support presentation		
Content: 4
•	Methodologies used are logical and applied correctly?
•	Recommendations are logical and well founded on analysis results?		
Communication: 2
•	Clear and coherent English expression?
•	Monotone vs. expressive?
•	Engaging talk vs. reading from the slides?
•	Handling Q&A

Report: 20%
A group report, in a format and style suitable to provide to management executives in a national retailer, consist of:
•	A title page (one-page)
•	A maximum 4-page executive summary; and
•	A maximum 10-page technical report, including any references and appendices.

The executive summary is a non-technical summary of (1) the project, (2) the analysis that was conducted, (3) the major findings, and (4) the recommendations. In industry most people will NOT read the technical report, so it is crucial that the executive summary succinctly communicates your work and the main results/takeaway.

The technical report details the technical aspects of your analysis. You should NOT repeat information included in the executive summary unless it is required for context/understanding. Despite being a technical report, this section may be read by those that are not well versed in spatial analytics (think about what you knew about spatial analytics and spatial terminologies three months ago) and you should write this report with that in mind. It is also NOT necessary to describe the exact buttons you pressed or R functions or R codes in this section. Do not include screenshots from R or ArcGIS – ensure all figures and tables are presented in a manner consistent with a formal report.

Your entire report must be no longer than 15 pages including the title page and any maps, tables, references, and appendices (meeting minutes does not count toward the page limit). It must contain at least the following somewhere in your report but how you organise the report is up to you:

•	At least five visuals (maps and graphs) that effectively communicate the analysis and plans. These can be produced by any software/tool. You may include additional maps if you wish.
•	The financial implications of the recommendations should be discussed but a full financial analysis is not required.
•	A section explaining assumptions you have made about the data and/or the analysis you have done. In the same section, listing all datasets that were NOT provided to you as part of this unit (and where possible, include a URL link to these datasets). 
•	Anything that is not your own work must be properly referenced. The last thing I want is to refer (a group of) students to the School’s Academic Integrity for investigation.
•	A copy of meeting summaries (template included at the end of this file, and meeting summaries do not count towards your 15-page limit).

You should use the following rubric to guide your group report.  
  
Exec Summary: 5
1 - General introduction (Don't just jump into what you did. Why are you doing it?)
1 - Analysis - Clear, non-technical description.
1 - Findings and Recommendations - Clear, non-technical description.
1 - Assumptions - Clear, non-technical description.
0.5 - Referenced datasets - Listing
0.5 - Meeting summaries - Appendix
 
Analysis of Sales data: 8 (clarity of description, appropriateness of methodology, graphics)
3 - Analysis of historical sales performance 
3 – Benchmarking, including an analysis of socio-economic data
2 - Selection of stores to close
 
Logistics and Distribution: 5 (clarity of description, appropriateness of methodology, graphics)
2.5 - Placement of DC
2.5 - Routing plan
 
Readability: 2
1 - Grammar and spelling
1 - Report structure and page limit

Independent Peer Evaluation: Due by 27/10/2023 at 23:59
While this is a group project, group members will receive individual marks according to their relative contributions to the group work. Therefore, you must submit your independent peer evaluation of your group members’ contributions, relative to your contribution. For example, if all group members contribute equally, you should give each and all group members, including yourself, an average mark of 3 (on a scale from 1 to 5).  If member X in your group contributes a bit more than member Y, you should X a higher mark than the mark you give to Y.  
It is very important that (1) you use word processing software (such as MS Word) to complete the Independent Peer Evaluation form (available on Canvas on the submission page) and that (2) the submitted file be in word format (i.e., .docx). DON’T use handwriting or converting your completed form to another format such as PDF. Doing so will result in your peer evaluation being excluded from consideration in the process of assigning individual mark to each group member.

References
ABS (2022): “Retail Trade, Australia”. Available at https://www.abs.gov.au/statistics/industry/retail-and-wholesale-trade/retail-trade-australia/latest-release#online-retailing 
Australia Post (2020) “2020 ecommerce industry report”. Available at https://auspost.com.au/content/dam/auspost_corp/media/documents/2020-ecommerce-industry-report.pdf 
Big Commerce (2022) “16 Online Shopping Statistics: How Many People Shop Online?”. Available online at https://www.bigcommerce.com.au/blog/online-shopping-statistics/#5-essential-online-shopping-statistics 
Elmas, M. (2021) The 50 billion reasons why Myer is closing yet another store. The New Daily. Available at https://thenewdaily.com.au/finance/consumer/2021/03/31/myer-closes-store/. 

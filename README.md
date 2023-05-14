# garimas_WHOcovid19_analysis_powerbi
scope = Data analysis of corona virus by scrapping data from the WHO website, cleaning and tranforming it then creating dashboard ; all using power bi
Step1) scrapping - Take out important data from website 
 https://covid19.who.int/table
https://app.powerbi.com/view?r=eyJrIjoiYWRiZWVkNWUtNmM0Ni00MDAwLTljYWMtN2EwNTM3YjQzYmRmIiwidCI6ImY2MTBjMGI3LWJkMjQtNGIzOS04MTBiLTNkYzI4MGFmYjU5MCIsImMiOjh9
https://worldhealthorg.shinyapps.io/covid/

Step2) Transform data in power bi – data cleaning.
Changed the type of column to appropriate datatype
Iso_start_date to date
Replaced values – nulls to 0
Added custom columns – population , persons not vaccinated, …
Filtered rows – where sex was all
Replaced values – age group to consistent with only 6 bins, any values like null,N/A,or empty value in numeric columns to 0
Removed columns – removed unwanted columns like number

Step3) Create desired dashboard visualization.
1)	type of vaccinations and their success rate
2)	total cases, total death, New cases
3)	Deaths w.r.t. age categories
4)	the number of people infected based on location
5)	Confirmed cases, deaths and vaccination according to countries. percentage decrease/ increase on the basis of months
6)	trends of deaths & people receiving vacinations.
7)	How many infected and how many die
8)	Geographical analysis – num of death ,recovery 


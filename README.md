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


DATASET FIELD NAME, DATATYPE AND DESCRIPTION
![image](https://github.com/gbcltr/garimas_WHOcovid19_analysis_powerbi/assets/85185163/b505d22a-d128-46e5-9d16-b0045c086477)

Field name	- Type	 - Description
Date_reported -	Date	 -Date of reporting to WHO
Country_code -	String -	ISO Alpha-2 country code
Country	- String - 	Country, territory, area
WHO_region	-String-	WHO regional offices: WHO Member States are grouped into six WHO regions  Regional Office for Africa (AFRO), Regional Office for the Americas (AMRO), Regional Office for South-East Asia (SEARO), Regional Office for Europe (EURO), Regional Office for the Eastern Mediterranean (EMRO), and Regional Office for the Western Pacific (WPRO).
New_cases-	Integer -	New confirmed cases. Calculated by subtracting previous cumulative case -count- from current cumulative cases count.*
Cumulative_cases	-Integer-	Cumulative confirmed cases reported to WHO to date.
New_deaths	-Integer-	New confirmed deaths. Calculated by subtracting previous cumulative deaths from current cumulative deaths.*
Cumulative_deaths	-Integer	-Cumulative confirmed deaths reported to WHO to date.


DATE_UPDATED -	Date	-Date of last update
TOTAL_VACCINATIONS -	Integer	- Cumulative total vaccine doses administered
PERSONS_VACCINATED_1PLUS_DOSE -	Decimal	- Cumulative number of persons vaccinated with at least one dose
TOTAL_VACCINATIONS_PER100	- Integer	- Cumulative total vaccine doses administered per 100 population
PERSONS_VACCINATED_1PLUS_DOSE_PER100 -	Decimal	- Cumulative persons vaccinated with at least one dose per 100 population
PERSONS_FULLY_VACCINATED -	Integer -	Cumulative number of persons fully vaccinated
PERSONS_FULLY_VACCINATED_PER100	- Decimal	- Cumulative number of persons fully vaccinated per 100 population
VACCINES_USED -	String	- Combined short name of vaccine: “Company - Product name” (see below)
FIRST_VACCINE_DATE	- Date -	Date of first vaccinations. Equivalent to start/launch date of the first vaccine administered in a country.
NUMBER_VACCINES_TYPES_USED	- Integer	- Number of vaccine types used per country, territory, area
PERSONS_BOOSTER_ADD_DOSE	- Integer -	Persons received booster or additional dose
PERSONS_BOOSTER_ADD_DOSE_PER100	- Decimal	- Persons received booster or additional dose per 100 population



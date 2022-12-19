
data acquisitie
		: https://coronadashboard.rijksoverheid.nl/verantwoording#ziekenhuizen
		: source-age-statistics.png
		
source age 	: https://opendata.cbs.nl/#/CBS/nl/dataset/03759ned/table?dl=39E0B 
		: accessed at 18-05-2022 10:06
		: population-age.png
		: population-age.csv
		
		: summed age categories and divided by 0.1% of total population size to translate to categories of max 200 and leading to a test population size of 1000
		: Note these statistics describe the situation on 1-1-2020

source severe cases
		: https://data.rivm.nl/covid-19/COVID-19_ziekenhuis_ic_opnames_per_leeftijdsgroep.csv
		: accessed at 18-05-2022 10:25
		: COVID-19_ziekenhuis_ic_opnames_per_leeftijdsgroep.csv
		: description: https://data.rivm.nl/meta/srv/dut/catalog.search#/metadata/759f40ae-33b4-4fc1-89d3-c4fa6393622e

source fatalities
		: file: https://data.rivm.nl/covid-19/COVID-19_casus_landelijk.csv
		: accessed ad 18-05-2022 13:13
		: Note we took the first approx 50k rows to select the first half of 2020, lowering the file size: COVID-19_casus_landelijk_Q1Q2_2020.csv
		: of these rows we only observed row 12062 to 47426 to select the smart lockdown period of 23-3-2020 to 31-05-2020
		: description: https://data.rivm.nl/meta/srv/dut/catalog.search#/metadata/2c4357c8-76e4-4662-9574-1deb8a73f724 laboratorium bevestigde COVID-19 patiënten 

populatieopbouw genomen uit kolom F van population-age.csv
percentages SR en IFR genomen uit kolom V en Q uit COVID-19_casus_landelijk_Q1Q2_2020.csv (welke aantallen (IC) opnames uit COVID-19_ziekenhuis_ic_opnames_per_leeftijdsgroep.csv overgenomen heeft (kolom L en V))

Testing:

run several tests with and without lockdown, with and without masks etc.

masks do matter in this model, but not as much just to prevent death

Note that official NL statistics for a population size 1000 would mean no deaths at all!

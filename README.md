# OpenDatasus Covid-19 Vaccine Base
This script generates a basis for analysis of Covid-19 vaccination data. The base format is already perfect for BI tools. It is possible to identify people with a delayed vaccination schedule.

Second doses of Astrazeneca that are not administered 99 days after the 1st dose are considered overdue. The interval is reduced to 45 days for Pfizer and CoronaVac.

## Authors:
- Isadora Rodrigues
- Heitor Mesquita (https://github.com/heitorcmesquita)

## In this sense, the Dictionary of the column "vacina_descricao_dose_2" follows:

0 : Subjects with delayed second dose

1 : Individuals with a second dose already applied

2 : Subjects who received a single-dose vaccine

8 : Individuals with a second dose already applied, but without a corresponding first dose at the base

9 : Subjects in the interval between doses

It is worth mentioning that the OpenDatasus microdata present a certain delay in relation to what is published on LocalizaSUS. Also, in another important consideration, cell #7 contains the names of vaccines that are entered into the system. This list was made on 6/17, and new names may have been added since then. That's why we have a script in this repository that is used to extract the names of vaccines in the system, and it can be verified by each user.

In the following link are the files with the microdata: https://opendatasus.saude.gov.br/dataset/covid-19-vacinacao

Other considerations are within the script.

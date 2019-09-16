# Project Notes

This document will contain all questions with answers related to the project as well as various notes.

### How was the project started?
The city of San Francisco releases data to the public through its [open data portal][1]. They have an enormous trove of data available.

Kaggle ("Your home for data science") has a [datasets][2] section of their site where any user can submit a dataset. The city of SF has an account and submitted this current dataset on [library usage][3]. The [original data][4] can be found on SF's data portal.

### Description (from the city)

> The Integrated Library System (ILS) is composed of bibliographic records including inventoried items, and patron records including circulation data. The data is used in the daily operation of the library, including circulation, online public catalog, cataloging, acquisitions, collection development, processing, and serials control. This dataset represents the usage of inventoried items by patrons

> The dataset includes approximately 420,000 records, with each record representing an anonymized library patron. Individual columns include statistics on the type code and age of the patron, the year the patron registered (only since 2003), and how heavily the patron has been utilizing the library system (in terms of number of checkouts) since first registering.


### Essential metadata
423K Rows and 15 Columns - Each row is a patron record

### When was the data created
Dec 1, 2016

### How far back does the data go?
According to the *Year Patron Registered* column, there are no dates prior to 2003 due to system migration.

### How often is it updated?
* Data changes multiple times per hour.  
* It is published twice every year

### What database contains the data?
No details

### Who are the admins of the database?
No details

### How to contact owner?
Link on data portal site allows you to contact owner

### What is the process that the raw data has gone through before it reached your hands? 
No details

### Is there a data dictionary describing every column
Yes, the original data dictionary is an excel file found on the data portal. I have also converted it to a csv file so I can view it in the Jupyterlab.

### What previous work has been done with this dataset?
The [kernels section][5] on kaggle has several notebooks that you can use to explore other ideas, comment on, and get feedback.

### How has data changed over time?
Unknown without looking at data?

## Subject Matter Research

Wikipedia article on [trends of library usage][6]

> While usage of some library services, such as reference assistance, has declined, there has been a well-documented increase in the usage of public libraries in the U.S. and Canada over the last decade. Most libraries have added services such as public computers, free wifi, and digital materials such as web sites and e-books, leading to higher overall usage of the library. 

> Public libraries remain very popular among all users, and as of 2014, younger patrons read and use the library at the same rate as older ones. Over 94% of Americans say that “having a public library improves the quality of life in a community.”

> At the same time, public funding of libraries has declined precipitously.

From the [pew research center][8] (2016)

![pew research][7]

# Exploratory Data Analysis questions

* Why is the Supervisor district a float?

* Examine low count patron types. Can they be combined into another category?

[1]: https://data.sfgov.org
[2]: https://www.kaggle.com/datasets
[3]: https://www.kaggle.com/datasf/sf-library-usage-data
[4]: https://data.sfgov.org/Culture-and-Recreation/Library-Usage/qzz6-2jup
[5]: https://www.kaggle.com/datasf/sf-library-usage-data/kernels
[6]: https://en.wikipedia.org/wiki/Trends_in_library_usage
[7]: http://assets.pewresearch.org/wp-content/uploads/sites/14/2016/09/PI_2016.09.09_Libraries-2016_2-01.png
[8]: http://www.pewinternet.org/2016/09/09/library-usage-and-engagement/
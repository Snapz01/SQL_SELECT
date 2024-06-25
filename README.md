USE world;
# SQL select query exercise
#
# World database layout:
# To use this database from a default MySQL install, type: use world;
#
# Table: City
# Columns: Id,Name,CountryCode,District,Population
#
# Table: Country
# Columns: Code, Name, Continent, Region, SurfaceArea, IndepYear, Population, LifeExpectancy, GNP, Capital
#
# Table: CountryLanguage
# Columns: CountryCode, Language, IsOfficial,Percentage
#
#
# 1: Get a query to return "Hello World", 123
# (Hint: 1 row, 2 columns)
#SELECT "hello world" as message , 123 as id;
#
# 2: Get everything from the city table
# (Hint: Many many rows)
#SELECT * FROM world.city;
#
# 3: Get everything on the cities whose district is "aceh"
# (Hint: 2 rows)
#SELECT * FROM world.city WHERE District IN ('aceh');
#
# 4: Get only the name of the cities where the countrycode is "bfa"
#SELECT Name FROM world.city where CountryCode IN ('bfa');
#
# 5: Get both the name and district of the cities where the countrycode is "tto"
#SELECT Name, District FROM world.city where Countrycode IN ('tto');
#
# 6: Get the name and district named as nm,dist from the cities where the countrycode is "arm"
#SELECT Name as nm, District as dist FROM world.city WHERE CountryCode IN ('arm');
#
# 7: Get the cities with a name that starts with "bor"
#SELECT Name FROM world.city where Name LIKE 'bor%';
#
# 8: Get the cities with a name that contains the string "orto"
#SELECT Name FROM world.city where Name LIKE '%orto%';
#
# 9: Get the cities that has a population below 1000
#SELECT Name, Population FROM world.city WHERE Population < 1000;
#
# 10: Get the unique countrycodes from the cities that has a population below 1000
#SELECT CountryCode, Population FROM world.city WHERE Population < 1000;
#
# 11: Get the cities with the countrycode UKR that has more than 1000000 (one million) in population
#SELECT Name, CountryCode, Population FROM world.city WHERE Population > 1000000;
#
# 12: Get the cities with a population of below 200 or above 9500000 (9.5 million)
#SELECT Name, Population FROM world.city WHERE Population < 200 OR Population > 9500000;
#
# 13: Get the cities with the countrycodes TJK, MRT, AND, PNG, SJM
#SELECT Name, CountryCode FROM world.city WHERE CountryCode IN ('TJK', 'MRT', 'AND', 'PNG', 'SJM');
#
# 14: Get the cities with a population between 200 and 700 inclusive
#SELECT Name, Population FROM world.city WHERE Population BETWEEN 200 AND 700;
#
# 15: Get the countries with a population between 8000 and 20000 inclusive
#SELECT NAME, Population FROM world.country WHERE Population BETWEEN 8000 AND 20000;
#
# 16: Get the name of the countries with a independence year (indepyear) before year 0
#SELECT Name FROM world.country WHERE IndepYear < 0;
#
# 17: Get the countries that has no recorded independence year and a population above 1000000
#SELECT Name, IndepYear, Population FROM world.country WHERE IndepYear IS NULL AND Population > 1000000;
#
# 18: Get countries with a SurfaceArea below 10 and a defined(can i define it? or i'm i not understanding the asignment) LifeExpectancy
#SELECT Name, SurfaceArea, LifeExpectancy FROM world.country WHERE SurfaceArea <10 AND LifeExpectancy > 40;

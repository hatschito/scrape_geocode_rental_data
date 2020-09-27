## scrape_geocode_rental_data
Script to scrape rental data from the German portal Immobilienscout24.

### Scrape rental data (source statisquo.de; modified by hatschito)
The first part of the script scrapes rental data with the  „beautiful soup“ Python library. Based on code from statisquo.de, that had to be updated, as Immobilienscout24 changed the structure, how they put their data on the website. The code was partly re-written, and now serves as nice efficient way, to scrape through the rental portals webpages and download data as csv.
### Geocode
In the second part of the script, is a geocoding part. Geopy is used to geocode the csv and export a geopackage. 

The code daily scrapes and geocodes data and writes it to a PostgreSQL database with PostGIS extension.  



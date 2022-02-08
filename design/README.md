# Schema Design

The format of the World Bank Data CSVs is as below.

![Markdown Logo](https://github.com/Kwesi-Peterson/Enlightenment-Now/blob/main/design/CSVSchema.png)

Having ingested these CSVs, I use Pyspark to transform the data into the Star Schema below.

![Markdown Logo](https://github.com/Kwesi-Peterson/Enlightenment-Now/blob/main/design/StarSchema.png)

Design considerations:
1) Minimize size of fact table
2) Optimize for reads
3) Optimize for fast aggregations
4) Plan to load data via batch processing

Having created the Star Schema, I then prep the data for ingestion into PowerBI for further analysis. The PowerBI Model is as below.

![Markdown Logo](https://github.com/Kwesi-Peterson/Enlightenment-Now/blob/main/design/PowerBiModel.png)

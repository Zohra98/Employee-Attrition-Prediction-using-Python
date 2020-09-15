You can load the data using read_excel(), pointing the path to your local file.

# Read excel data
hr_data_raw <- read_excel(path = "data/WA_Fn-UseC_-HR-Employee-Attrition.xlsx")

Let’s check out the raw data. It’s 1470 rows (observations) by 35 columns (features). The “Attrition” column is our target. We’ll use all other columns as features to our model.
# View first 10 rows
hr_data_raw[1:10,] %>%
    knitr::kable(caption = "First 10 rows")

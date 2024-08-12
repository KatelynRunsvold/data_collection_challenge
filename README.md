# data_collection_challenge
i used chat gpt to help me with
mars_data = []

# Loop through each row in the table
for row in rows:
    # Find all columns (cells) in the current row
    cols = row.find_all('td')
    
    # Extract the text from each column, stripping any surrounding whitespace
    cols = [col.text.strip() for col in cols]
    
    # Only add non-empty rows to the list (to skip headers or empty rows)
    if len(cols) > 0:
        mars_data.append(cols)

i had trouble importing the data into the list

# Quiz Solutions

### Q1: How do you create a new Series with the default index and the data `[2.5, 4.0, 5.5, 6.75]`?

**Answer: A** - `pd.Series([2.5, 4.0, 5.5, 6.75])`

Explanation: This is the simplest way to create a Series with default index (0, 1, 2, 3) and the given data values.

### Q2: How do you drop the columns 'two' and 'four' from a DataFrame named 'data'?

**Answer: B** - `data.drop(['two', 'four'], axis=1)`

Explanation: To drop columns, we use axis=1 (columns). axis=0 would drop rows instead.

### Q3: What is the difference between `loc` and `iloc` indexing in Pandas?

**Answer: A** - `loc` indexing refers to the index label, while `iloc` refers to the position

Explanation: `loc` uses labels/index to select data, while `iloc` uses integer positions.

### Q4: How do you apply a function to each column of a DataFrame named 'frame'?

**Answer: A** - `frame.apply(func)`

Explanation: By default, `apply()` operates on columns. If you need to apply to rows, you would specify axis=1.

### Q5: How do you rank a DataFrame named 'frame' over the columns?

**Answer: D** - Both B and C are correct

Explanation: Both `axis='columns'` and `axis=1` are valid ways to specify ranking over columns.

### Q6: What is the purpose of the `combine_first` method in Pandas?

**Answer: A** - To combine two DataFrames by taking values from the first DataFrame when overlapping

Explanation: `combine_first` combines two DataFrames, using values from the caller DataFrame where available.

### Q7: How do you return unique values of the index `pd.Index(['a', 'b', 'c', 'a'])`?

**Answer: A** - `pd.Index(['a', 'b', 'c', 'a']).unique()`

Explanation: The `unique()` method returns an array of unique values in the Index.

### Q8: How do you create a new column 'age' in a DataFrame named 'df' with a scalar value of 25?

**Answer: A** - `df['age'] = 25`

Explanation: This is the simplest way to add a new column with a scalar value that will be broadcast to all rows.

### Q9: What is the purpose of the `isna` and `notna` functions in Pandas?

**Answer: A** - To detect missing or null values

Explanation: These functions return boolean masks indicating which values are missing/null (`isna`) or not missing/null (`notna`).

### Q10: What is the purpose of the `na_position` parameter in the `sort_values` method?

**Answer: A** - To specify the position of missing values in the sorted data

Explanation: `na_position` can be set to 'first' or 'last' to control where NULL values appear in the sorted result.

# pandas cheatsheet
---

## DataFrames

### removing columns/rows

```
df.drop('col_to_delete', axis=1) # columns; axis = 1
df.drop('row_to_delete', axis=1) # rows; axis = 0
```

### selecting rows & columns
*selecting columns*
```python
df['col_name'] # based off label

df[2] # based off position
```

*selecting loc rows*

```python
df.loc['row_label'] # based off label

df.iloc[2] # based off position
```

*selecting subset of rows & columns*

```python
df.loc['row_label', 'col_name']

df.loc[['row1_label', 'row2_label'], ['col1_name', 'col2_name']]
```

### conditional selections
similar to numpy, you can perform conditional selections with bracket notations

```python
df>0 

df[df>0] 

df[df['col1']>0]['col2', 'col3'] 

df[(df['col1']>0) & (df['col2'] > 1)] 

df[(df['col1']>0) | (df['col2'] > 1)] 
```








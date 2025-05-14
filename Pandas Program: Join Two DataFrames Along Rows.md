# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

# Create the first DataFrame
data1 = {
    'ID': [1, 2],
    'Name': ['Alice', 'Bob']
}
df1 = pd.DataFrame(data1)
data2 = {
    'ID': [3, 4],
    'Name': ['Charlie', 'David']
}
df2 = pd.DataFrame(data2)
df_combined = pd.concat([df1, df2], ignore_index=True)
print("Combined DataFrame:\n")
print(df_combined)
```
## Output:
````
    Input                                 Result
  id=[1 2]                                      Combined DataFrame:
 name=[alice, bob]                                            ID     Name
  id=[3 4]                                               0    1      Alice
name=[carlie,david]                                      1    2      Bob
                                                         2    3      Charlie
                                                         3    4      David
````
## Result:
The program was successful

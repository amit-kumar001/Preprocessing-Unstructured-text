# Preprocessing-Unstructured-text
## Some key points of this code  
 <ul>
    <li>Pandas is used to structure the data</li>
    <li>Numeric digits, special characters words are removed using anonymous and regular expression</li>
    <li>Use of loc and iloc to convert integer into text</li>
  </ul>
  
## Use of lambda function in the code  
To optimize code,lambda or anonymous function is used. It helps in structuring the text in better way. Please review the below code
```
new_df.loc[:, 'fetch_response'] = new_df.fetch_response.apply(
    lambda x: integer_2_text(df, x))
```

 ## Use of split function to remove @ character
 Split function is used to remove the word with @. Please see the below code to understand it.
 ```
 data = ' '.join(word for word in data.split(' ') if not word.startswith('@'))
 ```
 ## How to run this code
 Since the code for this repository is in form of .ipynb file, you may use the jupyter notebook. Code is running hence you can see the output of steps without running also. You can install jupyter using the below command
 ```
 pip install jupyter
 ```
 You can now run the file by opening the terminal and typing jupyter notebook. Please open the terminal in the folder where the jupyter file from this repository is downloaded.

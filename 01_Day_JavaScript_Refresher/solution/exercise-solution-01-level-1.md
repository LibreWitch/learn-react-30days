1. Declare an *empty* array;
   
   ```java
   const array1 = Array();
   const array2 = [];
   console.log(array1); // Output : []
   console.log(array2); // Output : []
   ```

2. Declare an array with more than 5 number of elements
   
   ```javascript
   const array = Array(6);
   const array1 = ["hello", "hallo", "awo", "uwu", "hey", "hoho"];
   
   console.log(array); 
   // Output : [null, null, null, null, null, null]
   
   console.log(array.fill("hello"));
   // Output: ["hello","hello","hello","hello","hello","hello"]
   
   console.log(array1);
   // Output : ["hello", "hallo", "awo", "uwu", "hey", "hoho"];
   ```

3. Find the length of your array
   
   ```javascript
   const array1 = ["hello", "hallo", "awo", "uwu", "hey", "hoho"];
   const arrayL = array.length;
   
   console.log(arrayL); // Output : 6
   ```

4. Get the first item, the middle item and the last item of the array
   
   ```javascript
   const array1 = ["hello", "hallo", "awo", "uwu", "hey", "hoho"];
   
   // Get the first item
   console.log(array1[0]); // Output : hello
   
   // Get the middle item
   console.log(array1[Math.floor(array1.length / 2 - 1)]); 
   // Output : awo
   console.log(2);
   // Output : awo
   
   //Get the last item
   console.log(array1[Array1.length -1]); // Output : hoho
   ```

5. Declare an array called *mixedDataTypes*, put different data types in the array and find the length of the array. The array size should be greater than 5
   
   ```javascript
   const mixedDataTypes = ["hello", "hallo", "awo", "uwu", "hey", "hoho"];
   
   console.log(array1.length); // Output : 6
   ```

6. Declare an array variable name itCompanies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon
   
   ```javascript
   const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
   ```

7. Print the array using *console.log()*
   
   ```javascript
   console.log(itCompanies); 
   // Output : ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon']
   ```

8. Print the number of companies in the array
   
   ```javascript
   console.log(itCompanies.length); // Output :  7
   ```

9. Print the first company, middle and last company
   
   ```javascript
   // Get the first company
   console.log(array1[0]); // Output : Facebook
   
   // Get the middle company
   console.log(array1[Math.floor(array1.length / 2 - 1)]); 
   // Output : Apple
   console.log(3);
   // Output : Apple
   
   //Get the last company
   console.log(array1[Array1.length -1]); // Output : Amazon
   ```

10. Print out each company
    
    ```javascript
    console.log(itCompanies.join(", "));
    // Output : Facebook, Google, Microsoft, Apple, Oracle, Amazon
    ```

11. Change each company name to uppercase one by one and print them out
    
    ```javascript
    console.log(itCompanies.toString().toUpperCase().split(','));
    // Output : ["FACEBOOK","GOOGLE","MICROSOFT","APPLE","ORACLE","AMAZON"]
    
    console.log(itCompanies.toString().toUpperCase());
    // Output : FACEBOOK,GOOGLE,MICROSOFT,APPLE,ORACLE,AMAZON
    ```

12. Print the array like as a sentence: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.
    
    ```javascript
    const bigCompanies = "Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon";
    
    console.log(bigCompanies.split(','));
    // Output : ["Facebook"," Google"," Microsoft"," Apple"," IBM","Oracle and Amazon"]
    ```

13. Check if a certain company exists in the itCompanies array. If it exist return the company else return a company is *not found*
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    const company = "IBM";
    const checkArray = itCompanies.includes(company) ? itCompanies[itCompanies.indexOf(company)] : "not found";
    
    console.log(checkArray);
    
    // or
    
    if (itCompanies.includes(company)) {
        console.log(itCompanies[itCompanies.indexOf(company)]);
    } else {
        console.log("not found");
    }
    ```

14. Filter out companies which have more than one 'o' without the filter method
    
    ```javascript
    const itCompanies = ['Facebook', 'Microsoft', 'Google',  'Apple', 'Oracle', 'Amazon'];
    let arr = [];
    
    const res = itCompanies.forEach(company => { if (company.match(/oo/g)) return arr.push(company); 
    });
    
    console.log(arr);
    ```

15. Sort the array using *sort()* method
    
    ```javascript
    console.log(itCompanies.sort());
    ```

16. Reverse the array using *reverse()* method
    
    ```javascript
    console.log(itCompanies.reverse());
    ```

17. Slice out the first 3 companies from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    console.log(itCompanies.splice(0, 3));
    ```

18. Slice out the last 3 companies from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    console.log(itCompanies.splice(3));
    ```

19. Slice out the middle IT company or companies from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    const middleArray = Math.floor(itCompanies.length / 2 - 1);
    
    console.log(itCompanies[middleArray]); // Output : Microsoft
    ```

20. Remove the first IT company from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    console.log(itCompanies.slice(1));
    // Output : ["Google","Microsoft","Apple","Oracle","Amazon"]
    ```

21. Remove the middle IT company or companies from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    const middleArray = Math.floor(itCompanies.length / 2 - 1);
    itCompanies[middleArray] = itCompanies[itCompanies.length - 1];
    itCompanies.pop();
    
    console.log(itCompanies);
    ```

22. Remove the last IT company from the array
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    console.log(itCompanies.slice(0, -1));
    ```

23. Remove all IT companies
    
    ```javascript
    const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'Oracle', 'Amazon'];
    
    console.log(itCompanies.slice(0, 0);
    ```

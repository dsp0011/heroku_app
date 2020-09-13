## Techincal Problems and summary

- The installation of the database went relatively smooth and not many problems were encountered.
- Running the cheksum test wasn't problemmatic, just had to remember that the script was in powershell and had to be saved as .ps1
- Some errors were encountered when running mongod command, however they were resolved quickly after googling the error codes
- Experiment 1 went fine and all the database statements were executed properly 
- Everything else is pretty self-explanatory given the pictures provided

---


## Custom function for experiment 2

The function tells the amount of times a customer has visited the store.
In theory, it can be useful to tell whether the customers are returning to the store often and see how it changes over time. 

    var mapFunctionTest = function() {
        emit(this.ord_date, this.cust_id);
    };

    var reduceFunctionTest = function(keyOrdDate, custId) {
        return custId.length;
    };

    db.orders.mapReduce(
        mapFunctionTest,
        reduceFunctionTest,
        { out: "map_reduce_test" }
    )


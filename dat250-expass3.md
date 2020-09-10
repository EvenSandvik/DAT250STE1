# Expass 3

## Technical problems

Screenshot for validation:

## Screenshots
### Validation

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/validation.png?raw=true "Optional Title")

### Screenshots experiment 1:

1. Insert and query

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/ex3ex1.1.png?raw=true "Optional Title")

2. Update

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/ex3ex1.3.png?raw=true "Optional Title")

3. Delete

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/ex3ex1.4.png?raw=true "Optional Title")

### Screenshots experiment 2:

#### Tutorial

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/ex3ex2.1.png?raw=true "Optional Title")

![Alt text](https://github.com/EvenSandvik/DAT250STE1/blob/master/ex3/ex3ex2.2.png?raw=true "Optional Title")

//My mapfuntion

// lets you see how many items a customer has. 

var mapFunction3 = function() 

{

   emit(this.cust_id, this.items.length);
   
}; 


//My ReduceFunction

var reduceFunction3 = function(keyCustId, items) {

   return Array.sum(items.length);
   
};


//My Mapreduce

db.orders.mapReduce(

   mapFunction3,
   
   reduceFunction3,
   
   { out: "map_reduce_example" }
   
);

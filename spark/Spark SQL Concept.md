## Spark SQL Concept

- Spark SQL in-memory caching
	Spark SQL **comular cache** (.cache()) reduce memory footprint by an order of magnitude. It applies column compression schemas such as **dictionary encoding** and run-length encoding.
- Spark SQL UDF
	Example: 
	```scala
	val model:LogisticRegressionModel = ...
	sparkSession.udf.register("predict",predict(x:Float,y:Float)=>model.predict(Vector(x,y)))
	sparkSession.sql("SELECT predict(age,weight) FROM uses")

	```
- **Catalyst** is a SQL query optimizer which contains a general library for representing **trees** and applying **rules** to manipulate it. It contains libraries and set of rules below:
	- expressions (1+(2+3))
	- logic query plans
	- analysis
	- logical optimization
	- physical planning
	- code generation

![SQL query planning](https://raw.githubusercontent.com/zhaomingli007/techinical_documents/master/resources/images/SQL\ query\ planning.png | width=100)

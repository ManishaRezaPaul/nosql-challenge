# nosql-challenge

##Challenge Objective
Using MongoDB, evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

##Analysing the dataset
1. Created database and collection using pymongo library for analysing the data
2. Added record using insert_one
3. Updated data fields using $set
4. Updated fields using update_many, delete_many and found queries using 'find' or 'find_one'
5. Created queries using $regex, $match, $gte and $lt to produce a list of establishements based on the given criterias
6. Created pipeline and used aggregation method to produce the list of establishment names based on the given criterias 
7. Used pandas dataframe to show the list of the establishments 

###Attention!
1. Ensure the field names match while querying, updating and adding new data
2. When updating fields using update_many ensure its in a list. 
For example: 
            "collection.update_many({},
            [{ '$set': {
                'fieldname': {'$toDouble': '$fieldname'},
                'fieldname': {'$toInt': '$fieldname'},
                }} ]
                )"

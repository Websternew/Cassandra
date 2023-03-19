# Cassandra

Trip Collaborator is an application which will help solve the biggest problem of booking a trip among friends,family and relatives.The suggestions we either get it from various platforms but managing them is sometimes difficult.So, Trip Collaborator is used to make that easier,two users should easily be able to share preferred location of their own.There are various features that can be implemented with these.

To convert the Redis data into a Cassandra column-family database, we would need to perform the following steps:

1.Create a keyspace in Cassandra to store the data.

2.Create column families to store the data.

3.Insert the data into the column families.


The following are the Column-families and their corresponding attributes


 
 mykeyspace.person (
    name text,
    age int,
    id int,
    PRIMARY KEY (id)
);


 mykeyspace.social (
    name text,
    relation text,
    placevisit text,
    name1 text,
    name2 text,
    relation1 text,
    relation2 text,
    placevisit1 text,
    placevisit2 text,
    PRIMARY KEY (name)
);


 mykeyspace.place (
    pname text,
    review text,
    cost int,
    days int,
    PRIMARY KEY (pname)
);


 mykeyspace.invitedfriends (
    num int,
    name text,
    nam1 text,
    name2 text,
    PRIMARY KEY (num)
);

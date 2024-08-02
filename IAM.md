Identity and access management ---> authentication(user) and authorization services (policies)

---> polices and services can be accesses with attaching a role / group /user

AWS root user (dont use root user ) ------> create a user

users --> authentication ---> attach policies (which and what they can do )

create and user and add it in groups ( so we dont have attach polices everytime )

groups ---> add group of people with same policies (devs , qa , systemadmins )

policies

roles

1.Roles for applications and system to authencticate to aws services
2.Attach the role to the application
3.applications connecting to each other

Policies JSON :

1.version
2.statement
3.Effect
4.Action
5.resource

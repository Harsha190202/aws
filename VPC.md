VPC : virtual private cloud ---> it is a public cloud where we can maintain access through ip addresses

Virtual private clouds can be configured to tighten down security at the highest level. For instance, an organization can create virtualized replicas of access control features usually employed by traditional data centers. Like data center security, a VPC can control access to resources by IP address

VPC ---> subnets (spliting the VPC)

subnets ---> public and private

VPC ---> needs to gateway to access from outside of the vpc

public subnet ---> can be connected using internet gateway
|
v
load balancer
|
v
route table
|
v
private subnet ----> sg (application / ec2 )

NACL(subnet level rules) and Nat gateway

private subnet ----> internet (it should not go through internet gateway because ip will be exposed) ---> so we mask ip using nat gateway

nacl ---> subnet layer traffic access , what traffic can be denied

will be applied to every application in subnet (allow / denied rule 1 > rule 100 > rule 200 > rule \*)

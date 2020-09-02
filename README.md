# Creating dynamic proxy using WCF ChannelFactory

This article helps you to generate a dynamic WCF service proxy using ChannelFactory. This will also describe what is ChannelFactory, the difference between ChannelFactory and Proxy, and when to use proxy or ChannelFactory.

## What is WCF ChannelFactory
ChannelFactory enables you to dynamically create a proxy object based on the Service Contract alone. You do not require to explicitly generate a proxy class or manually define it. This is helpful in a scenario where your service address changes frequently or DataContract changes to a newer version and as a client, you have lot of references to those services. So after changes happen at the service side, the client must update proxy.

## Applications

1. **[Northwind WCF Services](https://github.com/geeksarray/creating-dynamic-proxy-using-wcf-channelfactory/tree/master/NorthwindDynamicProxy/NorthwindServices)** - WCF Services 
   that implements and exposed Product and Category Service Contracts.
1. **[Shared Data Contracts](https://github.com/geeksarray/creating-dynamic-proxy-using-wcf-channelfactory/tree/master/NorthwindDynamicProxy/NorthwindContracts)** - that will be shared between Service and Clients
1. **[Client application](https://github.com/geeksarray/creating-dynamic-proxy-using-wcf-channelfactory/tree/master/NorthwindDynamicProxy/NorthwindClient)** - it is a console application that consumes uses Channel Factory and uses Shared data contract.

For more details visit - https://geeksarray.com/blog/creating-dynamic-proxy-using-wcf-channelfactory

# AzureServiceBusDemo
Demo for [azure service bus](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-messaging-overview) & [masstransit](https://masstransit-project.com/)
> Sending/Receiving messages From/To
>> - Queues
>> - Topics
>> - Subscriptions

Solution structure :
- `App` : console application net core 3.1
- `Lib` : class library net std 2.0

Demo will start 2 hosted services :
- `BusHostedService` : responsible of starting/stopping bus
- `FakeSenderHostedService` : responsible of publishing messages to bus

Bus is created & configured with `MassTransitBootstrapper` helper class

**`Tools`** : vs19, net core 3.1, masstransit 6, nlog 4.6

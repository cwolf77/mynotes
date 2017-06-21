# Camel

## Components

### Direct-vm

The **direct-vm:**component provides direct, synchronous invocation of any consumers in the JVM when a producer sends a message exchange.  
This endpoint can be used to connect existing routes in the same camel context, as well from other camel contexts in the **same**JVM.

This component differs from the [Direct](http://camel.apache.org/direct.html) component in that [Direct-VM](http://camel.apache.org/direct-vm.html) supports communication across CamelContext instances - so you can use this mechanism to communicate across web applications \(provided that camel-core.jar is on the system/boot classpath\).

At runtime you can swap in new consumers, by stopping the existing consumer\(s\) and start new consumers.  
But at any given time there can be at most only one active consumer for a given endpoint.

This component allows also to connect routes deployed in different OSGI Bundles as you can see here after. Even if they are running in different bundles, the camel routes will use the same thread. That autorises to develop applications using Transactions - Tx.






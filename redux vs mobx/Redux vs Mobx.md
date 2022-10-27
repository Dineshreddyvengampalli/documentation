## Redux vs Mobx
Both redux and mobx are used for state management.Redux uses single store for managing state were as mobx uses multiple stores to manage stores.Redux uses pure functions that does not allow the change of existance state.In Mobx we can use impure functions ,so that the existance state can be updated to new state with some changes.Mobx is simple and easy to learn for beginners.State is immutable in redux whereas state is immutable in mobx.

## When to use Redux
-->complex applications
-->To maintain single store (single source of truth)
-->To develop reducers as pure functions
-->Perticularly using functional based component development

## When to use Mobx
-->simple applications
-->To maintain multiple store for state management
-->do not need to use pure functions
-->Perticularly using class based component development

## Debugging
-->Redux provides debugging tools that makes it easier to debug apps
-->Since mobx has lot of abstraction, it is quite difficult to debug compared to redux

## Scalability
-->Since redux uses pure functions , it is easy to scale the application than mobx

## Data structure
-->Redux uses single object to store all the state ,updates must be tracked manually.
-->mobx uses absorveable data,that helps in automatically track the updates.
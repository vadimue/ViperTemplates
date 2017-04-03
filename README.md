# Swift templates
This are templates for [`Generamba`](https://github.com/rambler-digital-solutions/Generamba) 

- [Installation](#installation)
- [Reactive Viper](#reactive-swift)

## Installation
1) Setup [`Generamba`](https://github.com/rambler-ios/Generamba) and run `generamba setup` and fill out `Rambafile`

2) Updates templates section in your `Rambafile` as follow:
```
### Templates
catalogs:
- 'https://github.com/vadimue/ViperTemplates'
templates:
- {name: reactive_viper}
```

3) Run `generamba template install`

## Reactive Viper

Based on [Swifty Viper](https://github.com/rambler-digital-solutions/generamba-catalog)

Template was created for using with RxSwift and some other frameworks. Why? It turned out, that we don't need two protocols of [Rambler Version](https://github.com/strongself/The-Book-of-VIPER) of Viper. It is ViewInput and InteractorOutput. The rejection of these protocols ensures that we get rid of the bidirectional communication between the layers of the module. In this case, communication is provided by binding data through the Observable's.

Also, those libraries should be installed into project:
- [RxSwift](https://github.com/ReactiveX/RxSwift)
- [ViperMcFlurry](https://github.com/rambler-digital-solutions/ViperMcFlurry) for transferring data between VIPER modules
- [Cuckoo](https://github.com/SwiftKit/Cuckoo) for simplify writing stubs of protocols in Unit tests

# jdeserialize

jdeserialize is a library that interprets Java serialized objects -- the data generated by an ObjectOutputStream.  It also comes with a command-line tool that can generate compilable class declarations, extract block data, and print textual representations of instance values.

It is a full implementation of the Object Serialization Stream Protocol, as described in the Java Object Serialization Specification, chapter 6.  It does not instantiate any classes described in the stream; instead, it builds up an intermediate representation of the types, instances, and values.  Because of this, it can analyze streams without access to the class code that generated them.

It is aimed at reverse engineers working with serialized streams of unknown provenance, as well as developers working with code that uses Java serialization to store data. 

All public classes have workable javadoc documentation.


## Getting Started

Download the latest release jar and run
```
java -jar jdeserialize.jar -help
```

To analyse a serialized java object stored in a file run
```
java -jar jdeserialize.jar <theFileToAnalyse>
```

### Prerequisites

What things you need to install the software and how to install them

```
Java Runtime Environment
```

## Built With

* [Maven](https://maven.apache.org/) - Dependency Management

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Brandon Creighton** - *Initial work* - (<cstone@pobox.com>)
* **Chris Frohoff** - *Migration to github* - [frohoff](https://github.com/frohoff)
* **Frank Huxol** - *Mavenized project* - [FrankHuxol](https://github.com/FrankHuxol)

See also the list of [contributors](https://github.com/FrankHuxol/jdeserialize/contributors) who participated in this project.

## License

This code is in the public domain.

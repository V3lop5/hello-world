# Hello World!
**... in many computer languages.**

This Repository contains programs written in many different computer languages producing `Hello World!` as output.
It is similar to [leachim6/hello-world](https://github.com/leachim6/hello-world) except that this repository includes fully working and runnable sample projects. These projects are tested with docker whenever possible. 

This project also includes a README.md for each computer language with usefull information and links to get started. 

Feel free to contribute!


## Structure of Repository
```
language/
|--- HelloWorld-<language>
|--- README.md
|--- example-project/
```
Every computer language has its own folder named after it. The folder contains a file named `HelloWorld-<language name>` with an example printing `Hello World!` to console.
The `README.md` file contains information about the language and useful links.
In any case it should contain the release date, what the language is designed for, supported operating systems, a introduction how to build and run the code and a short guide (or link to a guide) for getting in touch with this language for the first time.


## Contributing
Feel free to contribute. Thats all for now. Just open a PR and add a new language and create the `README.md`. 

If you want to add or update a example project feel free to do so! When possible add a Dockerfile to build the program from source and creating a image to execute the program. 
You might checkout example projects of popular computer languages like [Java](./Java/java-maven) or [Kotlin](./Kotlin/kotlin-gradle-kts) to see how its done.
You might also update the configuration of Dependabot if its supports your build system.

## Modular samples for Visual Studio Code

JavaFX 17 samples to run from Visual Studio Code with different options and build tools.

Version Visual Studio Code: 1.63.0 or higher.

Download [JDK 11 or later](http://jdk.java.net/) for your operating system. Make sure `JAVA_HOME` is properly set to the JDK installation directory.

### Gradle

For the first time only:

- Make sure you have installed following extensions in your Visual Studio Code:
  - [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  - [Gradle for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-gradle)

- Clone the sample, open the folder `hellofx` in Visual Studio Code.

To run the JavaFX application, you can open the `Gadle Projects` explorer, expand `hellofx` > `Tasks` > `application` and run the Gradle task: `run`

![Run](./run.png)

#### Custom Runtime

To create and run a custom JRE, from terminal:

On Linux or Mac run:

    cd IDE/VSCode/Modular/Gradle/hellofx
    ./gradlew jlink
    build/image/bin/hellofx

On Windows run:

    cd IDE\VSCode\Modular\Gradle\hellofx
    .\gradlew.bat jlink
    build\image\bin\hellofx.bat
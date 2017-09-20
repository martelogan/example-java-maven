Apache Commons Collections - Ecse 429 Testing Project
===================
[![Build Status](https://travis-ci.org/martelogan/example-java-maven.svg?branch=trunk)](https://travis-ci.org/martelogan/example-java-maven)
[![Coverage Status](https://coveralls.io/repos/martelogan/example-java-maven/badge.svg?branch=trunk)](https://coveralls.io/r/martelogan/example-java-maven)

Description
-------------

This repo - forked from [here](https://github.com/codecov/example-java-maven)
will serve as a base for Project Group P 17's ECSE 429 - Software Validation Project. 

In particular, we will replace the original test cases with our own - but follow the paradigm set out by the original repository.

Instructions
-------------

1. Make sure you have all the dependencies needed to build this project. In particular, 
immediately after git clone, you should be able to successfully build and execute tests 
from the working directory via:
 <br>
 <br>
 `mvn clean install -U`
 <br>
 
2. We should all plan on using [IntelliJ](https://www.jetbrains.com/idea/) to keep consistent. 
Additionally, it would be very useful for everyone to [install the checkstyle plugin](https://medium.com/@jayanga/how-to-configure-checkstyle-and-findbugs-plugins-to-intellij-idea-for-wso2-products-c5f4bbe9673a),
download the [Google Code Style XML](https://raw.githubusercontent.com/google/styleguide/gh-pages/intellij-java-google-style.xml),
and [configure this as the default for IntelliJ](https://stackoverflow.com/a/35273850).
<br>
<br>
Ideally, if we are all using this plugin, we can ensure consistent formatting by running the plugin in IntelliJ 
to make sure our code conforms. It should actually also format our code to this by default.

3. **Most importantly**, before making a pull request, we should make sure the build
is passing by running:
 <br>
 <br>
 `mvn clean install -U test surefire-report:report`
 <br>
 <br>
 In addition to compiling and executing our test cases, this will also generate an HTML
 test report under _target/site/surefire-report.html_ . The test report will likely be a useful
 reference for compiling official documentation on the tests we've executed.
 <br>
 <br>




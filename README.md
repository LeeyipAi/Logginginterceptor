# Logginginterceptor
[![](https://jitpack.io/v/LeeyipAi/Logginginterceptor.svg)](https://jitpack.io/#LeeyipAi/Logginginterceptor)
How to
To get a Git project into your build:

Step 1. Add the JitPack repository to your build file

gradle
maven
sbt
leiningen
Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.LeeyipAi:Logginginterceptor:1.0.0'
	}
Step 3. Add LoggingInterceptor 	:
	 
	new LoggingInterceptor.Builder()
                .loggable(BuildConfig.DEBUG)
                .request()
                .requestTag("Request")
                .response()
                .responseTag("Response")
                .addHeader("version", BuildConfig.VERSION_NAME)
                .build();
	

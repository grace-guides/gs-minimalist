[![Main branch build status](https://github.com/grace-guides/gs-minimalist/workflows/Grace%20CI/badge.svg?style=flat)](https://github.com/grace-guides/gs-minimalist/actions?query=workflow%3A%Grace+CI%22)
[![Apache 2.0 license](https://img.shields.io/badge/License-APACHE%202.0-green.svg?logo=APACHE&style=flat)](https://opensource.org/licenses/Apache-2.0)
[![Grace on X](https://img.shields.io/twitter/follow/graceframework?style=social)](https://twitter.com/graceframework)

[![Groovy Version](https://img.shields.io/badge/Groovy-4.0.24-blue?style=flat&color=4298b8)](https://groovy-lang.org/releasenotes/groovy-4.0.html)
[![Grace Version](https://img.shields.io/badge/Grace-2023.2.0-blue?style=flat&color=f49b06)](https://github.com/graceframework/grace-framework/releases/tag/v2023.2.0-M3)
[![Spring Boot Version](https://img.shields.io/badge/Spring_Boot-3.2.12-blue?style=flat&color=6db33f)](https://github.com/spring-projects/spring-boot/releases/tag/v3.2.12)

# Minimalist App

### Grace Version

* Grace 2023.2.0-M3

### Creating a minimal app

```bash
$ grace -v

------------------------------------------------------------
Grace 2023.2.0-M3
------------------------------------------------------------

Build time:   2024-12-25 16:56:41 UTC
Revision:     d9fe039fabe3382aa74e660c6e31b1c260df1481

Spring Boot:  3.2.12
Gradle:       8.11.1
Groovy:       4.0.24
JVM:          17.0.12 (Azul Systems, Inc. 17.0.12+7-LTS)
OS:           Mac OS X 12.7.6 aarch64
```

Creating an app by using Grace CLI,

```bash
$ grace create-app grace.apps.minimalist --minimal
```

Now you get,

```bash
.
├── app
│   ├── conf
│   └── init
├── buildSrc
│   └── build.gradle
├── gradle
│   └── wrapper
├── src
│   ├── main
│   └── test
├── HELP.md
├── README.md
├── build.gradle
├── gradle.properties
├── gradlew
├── gradlew.bat
└── settings.gradle

9 directories, 8 files
```

Execute `grace run-app` or `./gradlew bootRun`,

```bash
> Task :bootRun

               ______
              / _____)
 o  o   o  o | /  ___   ____   ____   ____   ____
  \/ \^/ \/  | | (___) / ___) / _  | / ___) / _  )
   \_____/   | \____/|| |    ( ( | |( (___ ( (/ /
    =====     \_____/ |_|     \_||_| \____) \____)
  ================================================
  :: Grace ::                       (v2023.2.0-M3)

2024-12-26 17:13:18.078  INFO --- [  restartedMain] grace.guides.Application                 : Starting Application using Java 17.0.12 with PID 5867 (/Users/rain/Development/github/grace/grace-guides/gs-minimalist/build/classes/groovy/main started by rain in /Users/rain/Development/github/grace/grace-guides/gs-minimalist)
2024-12-26 17:13:18.079 DEBUG --- [  restartedMain] grace.guides.Application                 : Running with Spring Boot v3.2.12, Spring v6.1.16
2024-12-26 17:13:18.079  INFO --- [  restartedMain] grace.guides.Application                 : The following 1 profile is active: "development"
2024-12-26 17:13:18.097  INFO --- [  restartedMain] .e.DevToolsPropertyDefaultsPostProcessor : Devtools property defaults active! Set 'spring.devtools.add-properties' to 'false' to disable
2024-12-26 17:13:18.098  INFO --- [  restartedMain] .e.DevToolsPropertyDefaultsPostProcessor : For additional web related logging consider setting the 'logging.level.web' property to 'DEBUG'
2024-12-26 17:13:18.337  INFO --- [  restartedMain] g.plugins.DefaultGrailsPluginManager     : Total 1 plugins loaded successfully, take in 19 ms
2024-12-26 17:13:18.530  INFO --- [  restartedMain] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port 8080 (http)
2024-12-26 17:13:18.535  INFO --- [  restartedMain] o.a.coyote.http11.Http11NioProtocol      : Initializing ProtocolHandler ["http-nio-8080"]
2024-12-26 17:13:18.536  INFO --- [  restartedMain] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2024-12-26 17:13:18.536  INFO --- [  restartedMain] o.apache.catalina.core.StandardEngine    : Starting Servlet engine: [Apache Tomcat/10.1.34]
2024-12-26 17:13:18.555  INFO --- [  restartedMain] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2024-12-26 17:13:18.555  INFO --- [  restartedMain] w.s.c.ServletWebServerApplicationContext : Root WebApplicationContext: initialization completed in 457 ms
2024-12-26 17:13:18.675  WARN --- [  restartedMain] .b.a.g.t.GroovyTemplateAutoConfiguration : Cannot find template location: classpath:/templates/ (please add some templates, check your Groovy configuration, or set spring.groovy.template.check-template-location=false)
2024-12-26 17:13:18.743  INFO --- [  restartedMain] o.s.b.d.a.OptionalLiveReloadServer       : LiveReload server is running on port 35729
2024-12-26 17:13:18.754  INFO --- [  restartedMain] o.a.coyote.http11.Http11NioProtocol      : Starting ProtocolHandler ["http-nio-8080"]
2024-12-26 17:13:18.760  INFO --- [  restartedMain] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port 8080 (http) with context path ''
2024-12-26 17:13:18.766  INFO --- [  restartedMain] grace.guides.Application                 : Started Application in 0.829 seconds (process running for 1.193)
2024-12-26 17:13:18.789 DEBUG --- [  restartedMain] grace.guides.Application                 :
----------------------------------------------------------------------------------------------
        Application:   gs-minimalist
        Version:       0.0.1-SNAPSHOT
        Environment:   development
        Local:         http://localhost:8080
        External:      http://192.168.5.9:8080
----------------------------------------------------------------------------------------------
```

### Links

- [Grace Framework](https://github.com/graceframework/grace-framework)
- [Grace Guides](https://github.com/grace-guides)


## MCast

Cast from one to another type. A central collection will hold a list of default cast methods. You can extend or replace the methods if you want.

All methods will return a default value if casting is not possible. It will never throw an exception.

For basic types there are fast implementations to improve speed.

## MString

Functions to work with strings.

...

## M

This is a shortcut class to allow using of every day doings in a short way. This will clean the code without confusion (hopefully).

## MActivator

The activator loads object instances using singletons or load balancer. You can load instances by lookup the interface. It will return a default implementation or an existing for the current environment.

## MApi

A global singleton to manage all central services like configuration or logging.

## MArgs

Parse command line arguments.

## MBigMath

Tools to work with BigInteger and BigDecimal.

## MCollection

Tools for collections, lists and arrays.

## MConstant

Library constants.

## MCount

A counter that can be accesses from JMX.

## MCountWithDelay

A counter that can be configured by JMX to delay in moment of increasing the counter.

## MDate

Tools for Date and Calendar. Parsing and formatting.

## MEventHandler

Collect listeners in solid and weak lists and fire events to the listeners.

## MFile

Tools to work with files. Read, Write, Copy and Delete files. Normalize file names.

## MHousekeeper

Do house keeper tasks in the background.

## MJson

Tools to work with json.

## MLdap

Tools to work and simplify with LDAP.

## MLog

Extend MLog to support the log() tool. This replaces the definition of log in every class definition.

## MMath

Tools for numbers.

## MNet

Tools for networking.

## MPassword

Tools to encode, decode and generate passwords.

## MPeriod

Tool to work with time periods. Parse and format time periods and a lot of constants.

## MProperties

A better implementation if properties with casting of the primary types.

## MSoftTimerTask

A timer task encapsulated in a soft reference.

## MSql

Tools to work with sql.

## MStopWatch

A stop watch you can start pause and stop. You can print the time with formatted output.

## MSwing

Tools for the graphical framework swing.

## MSystem

System tools to get user, hostname, host system type and more.

## MThread

In the beginning a thread pool but now native thread enhancement. The method sleep() can't be interrupted. Also async execution methods.

## MThreadDaemon

Like MThread but for daemon threads.

## MThreadPool and MThreadDaemonPool

The original MThread implementation using thread pools (not recommended any more).

## MTimerTask

A timer task that can't be interrupted by exceptions.

## MValidator

Tools to validate data types like UUID email ect.

## MWeakTimerTask

A timer task encapsulated in a weak reference.

## MXml

Tools to work with xml.


## ILog

A logger meta framework. It enhanced the established log systems with new features. The framework contains appenders to common log systems like java logger, log4j and direct console output.

It fasten the log output by reducing overhead of serialising messages if the log level is not active.

It also introduce the concept of log trails. This means you can follow up what happens in because of an action in every module by increasing the log level for the thread.

## IRegistry

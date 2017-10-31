## Specification for a simple REST based communication

This specification is about a simpler way then the RESTful communication. This specification modifies 
the RESTful in a way the most http servers can handle out of the box.

### Overview of differences between RESTless and RESTful

The main difference is that in RESTless there will be no payload as JSON in the HTTP header. All parameters 
will be send as http form parameters. In case of a GET as GET parameters for other methods as form-data.

### Special parameters

Special parameters starts with an underline character but will not proceed with an underline. Parameters with multiple 
underlines will be shorten by one. e.g. '__parameter' will be '_parameter' in the underlying method. but '_parameter' 
will not be passed to the underlying method.

### Action extension

The HTTP method POST is used in two ways. In the first case as CREATE command and the other case a ACTION command. To
separate the cases the parameter '_action' will name the action to execute. If the the parameter is not given then 
the call is used as a CREATE command.

### Method simulation

The parameter '_method' is used to switch the called HTTP method. The value is not case sensitive and values 
are get, post, put, delete.

### Authentication by parameter

Authentication can be done by simple http authentiction or using the parameter '_ticket'. The value is some kind of
authentication string e.g. '_ticket=user:password'. It depends on the underlying engine.


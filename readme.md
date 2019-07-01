#### Dynamic subprocesses example

A RHPAM project illustrating how subprocesses can be included dynamically based on the value of a process instance variable.

* The project contains 3 processes: `main-process`, `sub-process-1`, `sub-process-2`.
* The `main-process` process definition has a _reusable sub-process node_.
* The _Called Element_ property of the subprocess node is set to the expression `#{subprocess}`.
* At runtime, when a process instance of `main-process` is created, the sub process invoked corresponds to the subprocess whose name is equal to the value of the `subprocess` process variable.
 
# Objective-C dealloc Error: Double Release Crash

This repository demonstrates a common but subtle error in Objective-C memory management: prematurely releasing objects within the `dealloc` method.  Incorrectly releasing an object that's also retained elsewhere will result in a double release, leading to a crash.

The `bug.m` file shows the erroneous code. The `bugSolution.m` demonstrates the correct approach, ensuring proper memory management.
# Ruby Bug: Unexpected Instance Variable Behavior

This repository demonstrates a subtle bug in Ruby related to modifying instance variables indirectly through accessor methods.

The `bug.rb` file shows that assigning a new value to the `value` method (which only returns the instance variable) does not change the instance variable itself.  This behavior can be unexpected and lead to hard-to-debug issues.

The `bugSolution.rb` file provides the correct way to modify instance variables, using `instance_variable_set` or creating a setter method.
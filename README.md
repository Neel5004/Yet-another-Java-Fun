# Yet-another-Java-Fun
Fun with auto boxing and the integer cache in Java
Integer foo = 1000;
Integer bar = 1000;
 
foo <= bar; // true
foo >= bar; // true
foo == bar; // false
//However, if the values of foo and bar are between 127 and -128 (inclusive)
//the behaviour changes:
 
Integer foo = 42;
Integer bar = 42;
 
foo <= bar; // true
foo >= bar; // true
foo == bar; // true

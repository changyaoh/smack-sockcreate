smack-sockcreate
================
This is a patch to add two new nodes : /proc/self/attr/sockincreate /proc/self/sockoutcreate ,
sockincreate is for smk_in label , sockoutcreate is for smk_out label .
A process may write label into given interface and all subsequent sockets created will be 
labeled with that label .
The idea comes from SELinux's  /proc/self/attr/sockcreate node.

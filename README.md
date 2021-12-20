Role Name
=========

This role is designed to reach into Satellite and create a new VM from a template in VMware.

Requirements
------------


Role Variables
--------------

The following variables are used in this role and MUST be passed in from command line or group/host vars:
  - new_hostname: This will be the short hostname of the new VM.
  - host_group: This is the host group within Satellite to put the VM inside.  The host group ties it to content view and activation key.
  - vm_image:  This is the image to clone from.  
  - vm_lifecycle: 
  - vm_cpu: Number of CPUs required for VM.
  - vm_mem: How much RAM is required for VM.


The following variables are configured with default values that you may choose to change:
  
  - vm_location:
  - vm_compute_resource: 
  - vm_subnet: 

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------


Author Information
------------------

Originally created by Charles Randall RHCE, Red Hat Senior Consultant.

# Smartriqs fork
This fork is a modified version of Smartriqs.
## Original documentation
Visit https://smartriqs.com for more information.
## Modifications
### Added match output fields: registeredRoles and registeredRolesCount
If embedded data registeredRoles is added to the match configuration, after the (either failed or successful) match it will contain the roles that were registered during matching for non-bot participants. For example, if two people are matched with roles A and B, registeredRoles will be "A,B". In addition, if you add embedded data item registeredRolesCount, it will contain the number of roles that were thus registered. In the example, its value would be 2.
### Fixed bug with timed chat
If a timed chat is used, and the chat is exited using the exit button, the timer is still active in the Qualtrics background. As a result of this bug fix, the timer will no longer cause the Qualtrics next page button to be executed unexpectedly at a later moment.
### Fixed errors with PHP 8.4
Several errors and warnings produced on a server running PHP 8.4 were resolved in this fork.

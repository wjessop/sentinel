## v2.0.2
* Fix watch debug message formatting error.
* Allow watchers to be configured without templates.

## v2.0.1
* Handle 401 error codes from etcd.

## v2.0.0
+ More CLI options. Use -h to see them all.
* Connectivity related bug fixes:
* Bug fix: Watches would fail and skip changes on loss of connectivity.
* Bug fix: On start watchers would not be executed if no connection could be made.
* Bug fix: Gracefully handle "unexpected end of JSON input" error.
* Refactored and cleaner logging.
* Refectored configuration system.

## v1.1.1
* Execute command when no templates exist.

## v1.1.0 - Watcher Prefixes
+ Add watcher specific prefixes.
+ Allow watching on directories.

## v1.0.5 - Logger Bug Fix
* Fix logger output setup on start.

## v1.0.4 - Watcher Bug Fix
* Validate watcher configuration.

## v1.0.3 - Watcher Bugs
* Do not exit when a watcher fails.

## v1.0.2 - Template Bug Fixes
* Renderer templates in temporary files under the destination directory. Fixes
  cross-volume link error.
* Fail template rendering if destination hash generation fails.

## v1.0.1 - Bug Fixes
+ Execute all watchers on start when run as a service.
* Clean all key path elements replacing `-` with `_`.
* Fix bug which causes hang on stop forcing the use of a SIGKILL.

## v1.0.0 - Initial Release
+ Trigger template rendering and command execution.
+ Watch and retrieve context for multiple keys.
+ Only execute command when rendered templates change.
+ Support multple templates.

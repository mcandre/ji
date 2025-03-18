# ji: DevOps Reanimated

![jiangshi](ji.png)

# USAGE

```console
$ ji
```

# EXAMPLE

A UNIX-based implementation in [bin/](bin).

# ABOUT

**ji** (as in *"jeepers"*)

ji is a convention for streamlined DevOps maintenance. The two characters *j, i* trigger your custom server automation. Interaction promotes a single `Enter` button, with an optional `Ctrl+C` hotkey to quit.

This dramatically simplifies workflows. For example, you can quickly update many homegrown servers by typing out `ji` on a smartphone terminal.

# PRECEPT 0: Maintainability

ji scripts should be reliable and implemented with simple code. If the script is not reliable, then it should not be run. If the code is not easy to modify, then it should not be written.

Commands in ji scripts should be easy to reproduce manually as a fallback. For example, by copy & paste into an SSH session.

ji scripts should not depend on external machine triggers such as CI/CD servers or cron jobs. It is okay to *wrap* a ji script this way. However, the script should be able to fulfill its duties when run from a local machine, triggered by manually running the command `ji`.

ji scripts should be linted regularly, in order to catch any glitches sooner.

ji does not say what is reliable or what is simple, that is for your team to decide.

# PRECEPT 1: Automation

ji scripts should automate laborious tasks, without runtime parameters. A repeated task with fixed parameters is a good candidate for a ji script.

ji follows the zeroconf semantic: The script should provide practical default behavior when no command line flags are specified, no environment variables are configured, and no configuration files are present.

The runtime environment should have the ji script in the `PATH` environment variable.

The ji entrypoint is triggered by executing the command *`ji`*, without arguments.

# PRECEPT 2: User Friendliness

Generally safe commands, such as updating package caches, should not prompt for user confirmation.

Potentially risky commands, such as upgrading software components, may prompt for user confirmation.

Potentially hazardous commands, such as deleting user data or rebooting servers, should have an explicit prompt to confirm the operation.

ji scripts should present simple binary user options, such as pressing `Enter` to continue; or pressing `Ctrl+C` to cancel the script.

ji scripts should not prompt for console input values. ji scripts may prompt once for sudo authentication.

ji prompts should not require explicit console values to be typed out, such as "Yes", "No", "y", "n", etc.

For example, configure low level commands to force acceptance by default without prompting. If needed, a simple `Enter` / `Ctrl+C` prompt can be introduce to replace the original prompt.

ji scripts should terminate on the first error or `Ctrl+C` interrupt, not continue processing.

ji scripts should report accurate exit codes.

For example, the common UNIX convention is to emit a non-zero code in the event of a failure, otherwise, zero. Termination due to user interruption by `Ctrl+C` is not considered a failure.

ji error traces should contain actionable, specific information for troubleshooting.

ji logs should present minimal, relevant, actionable information. Log noise should be kept to a minimum.

ji scripts should complete fairly quickly, with incrementing progress feedback during long delays.

ji scripts should behave idempotently: The script should succeed regardless of whether it is the first time run, or the nth time run.

# LICENSE

FreeBSD

# RUNTIME REQUIREMENTS

(User-specified)

## Recommended

* Run `ji` commands within a persistent terminal session such as [screen](https://en.wikipedia.org/wiki/GNU_Screen), especially for update scripts that may be sensitive to network disconnects.

# CONTRIBUTING

For more information on developing ji itself, see [DEVELOPMENT.md](DEVELOPMENT.md).

# CREDITS

* [Daniel Yu](https://www.thedanielyu.com/) artwork

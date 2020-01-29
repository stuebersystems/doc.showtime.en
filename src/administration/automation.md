# Automation

Automation means running certain recurring computer tasks without any required action from a user. Below we describe some ways you can fully automate certain operations of a public display computer using CONFIRE SHOWTIME.

## Start Up Computer

You have the following options to automatically start a computer without having to explicitly press the power button.

### Wake on Power

Starting up the computer as soon as power is restored for example after a power outage or a power cable is reconnected (Wake on Power). It's a setting which must be supported by your BIOS. This setting is preconfigured on our [CONFIRE E-BOARDS]. You'll find further details about our CONFIRE E-BOARDS in the [CONFIRE E-BOARD Documentation] under the "BIOS Configuration" of the respective computer.

The advantage of Wake on Power is that it requires absolutely no power to have been running prior to power being restored. The setting is stored in the BIOS and is not lost during a power outage.

### Wake on LAN

Starting up a computer can also be done by a dedicated network command via another computer (Wake on LAN). An active computer in the network sends a small data packet to the network card of turned off computer(s). The computer will then start up by itself. Wake on LAN is an industry standard and must be supported by the computer's network card.

With Wake on LAN the computer is never 100% turned off. The network card still receives a minimal supply of power and therefore must remained plugged into the mains. See our [Wake on LAN] guide for more info.

### Wake on Standby

CONFIRE SHOWTIME supports [Wake on Standby]. You can define a task in the schedule of a project that configures the system to shutdown at a given time. Optionally you can configure the Startup/WakeUp for this task via Wake On Standby.

## Start Player

Once the computer has started up CONFIRE SHOWTIME PLAYER must be started and the appropriate project launched too. Even this can be automated too. You'll find the AutoStart Settings under `ENVIRONMENT > AutoStart Settings` in CONFIRE SHOWTIME PLAYER. Select your project from the bottom option `Start project automatically`. Once you've done that then next time the computer starts CONFIRE SHOWTIME PLAYER will behave as follows:

1. Straight after Windows starts up the Player starts.

2. The selected project is loaded.

3. The Showcase or Schedule assigned to this project is launched.

Further details can be found in [Start Player].

## Update Content

If a project is launched on a public display and the content of the project changes CONFIRE SHOWTIME PLAYER can react to this automatically:

1. In the Player subscribe to the project that you want to launch.

2. Under properties of the project configure regular intervals to set how often the Player should check for an update to the published project.

When CONFIRE SHOWTIME PLAYER detects that the problem has changed it will automatically download and updated the project in the background. It will then restart the project with the new content. 

See more details about subscribing to projects in chapter [Subscribe to Projects], Details about publishing projects in chapter [Publish Projects].

## Shutdown Computers

In order to automatically shutdown a computer you have mostly three options:

* You turn off the power for all computers centrally.

* You set up a task in the Task Management of Windows that shuts down the computer at a given point in time.

* You set up a schedule in CONFIRE SHOWTIME for the project running on the public display that defines a task of shutting down the computer 

The advantage of the last option is you can configure the shutdown of the system from the comfort of your desk. By publishing the project the settings of the schedule are distributed to all public displays. In addition you could configure Wake on Standby. 

Details for settings up schedules can be found in chapter [Manage Schedules].

[CONFIRE E-BOARDS]: http://eboard.stueber.co.uk
[CONFIRE E-BOARD Documentation]: http://doc.eboard.stueber.de
[Wake on Standby]: ../simple-glossary.md#wakeonstandby
[Start Player]: ../howto/play-projects/start-player.md
[Subscribe to Projects]: ../howto/play-projects/subscribed-projects.md
[Publish Projects]: ../howto/publish-projects/README.md
[Manage Schedules]: ../howto/create-projects/manage-schedules/README.md
[Wake on LAN]: https://doc.eboard.stueber.de/tips/wake-on-lan/index.html
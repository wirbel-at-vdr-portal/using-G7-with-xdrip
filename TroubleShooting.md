# Trouble shooting the G7 - an yet incomplete list

## There is written G6 sensor, I'm using a G7? Is there something misconfigured?
This normal, as both sensors use largely same parts of code.

## I always read *System Status page* or *Classic Status page*? Where do i find them?
Open the menu on top, left hand side. Those three lines, click on it.
Choose system status.

The page that just now opened is the System Status page. Now, tap on the middle of the screen and shift right. This is the Classic Status page.

## No connection?
Check if the following

1. in system status, on the Classic Status Page, there should be a line **Last Connected: xx minutes ago**, the number of minutes should be less or equal five minutes.
2. there should be none of this messages
- Hunting Transmitter
- Scanning Error
- Waiting Connect Errors
- Checking Auth Errors
- Deep Sleeping Errors

If this is not true, this needs to be solved *before doing anything else*.
- Is any other software contacting the sensor, ie Dexcom app? If so, disconnect it.
- Clear the command queue, if in system status there's one or more **Queue Items: ..** written:

1. Tap on the dropper symbol on the main screen (right hand side).
2. In the newly opened window, click on the microphone symbol.
3. A new edit window with catipn 'Type treatments' opens.
4. Enter (exactly) **clear transmitter queue**.

- *Last Connected is always less that 5 minutes* and *Checking Auth Errors* or *Deep Sleeping Errors*
Tap on **Forget device** on **classic status page**. Stay on system status page and observe a pair request.

- Try triggering a pair request
1. Find your current Dexcom sensor transmitter ID in the data source menu. Be shure to remember it, write it either down or do a screenshot.
2. Now, change it to an invalid number.
3. wait a few seconds and change it to the correct transmitter ID again.
4. Observe status in the system status page


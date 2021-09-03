# Multiprotocol TX Module OpenTX LUA scripts
<img align="right" width=300 src="../docs/images/multi.png" />

If you like this project and want to support further development please consider making a [donation](../docs/Donations.md).  

<table cellspacing=0>
  <tr>
    <td align=center width=200><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=VF2K9T23DRY56&lc=US&item_name=DIY%20Multiprotocol&currency_code=EUR&amount=5&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted"><img src="../docs/images/donate_button.png" border="0" name="submit" title="PayPal - Donate €5" alt="Donate €5"/></a><br><b>€5</b></td>
    <td align=center width=200><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=VF2K9T23DRY56&lc=US&item_name=DIY%20Multiprotocol&currency_code=EUR&amount=10&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted"><img src="../docs/images/donate_button.png" border="0" name="submit" title="PayPal - Donate €10" alt="Donate €10"/></a><br><b>€10</b></td>
    <td align=center width=200><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=VF2K9T23DRY56&lc=US&item_name=DIY%20Multiprotocol&currency_code=EUR&amount=15&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted"><img src="../docs/images/donate_button.png" border="0" name="submit" title="PayPal - Donate €15" alt="Donate €10"/></a><br><b>€15</b></td>
    <td align=center width=200><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=VF2K9T23DRY56&lc=US&item_name=DIY%20Multiprotocol&currency_code=EUR&amount=25&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted"><img src="../docs/images/donate_button.png" border="0" name="submit" title="PayPal - Donate €25" alt="Donate €25"/></a><br><b>€25</b></td>
    <td align=center width=200><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=VF2K9T23DRY56&lc=US&item_name=DIY%20Multiprotocol&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted"><img src="../docs/images/donate_button.png" border="0" name="submit" title="PayPal - Donate" alt="Donate"/></a><br><b>Other</b></td>
  </tr>
</table>

## MultiChannelsUpdater.lua

Automatically name the channels based on the loaded Multi protocol and sub protocol including the module channel order convention.

Need OpenTX 2.3.9 or above. Located on the radio SD card under \SCRIPTS\TOOLS. This script needs MultiChan.txt to be present in the same folder.

[![MultiChannelsUpdater](https://img.youtube.com/vi/L58ayXuewyA/0.jpg)](https://www.youtube.com/watch?v=L58ayXuewyA)

## DSM Forward Programming

This is a work in progress. It's only available for color screens (Horus, TX16S, T16, T18...).

If some text appears as Unknown_xxx, please report xxx and what the exact text display should be.

Need OpenTX 2.3.10 nightly or above. Located on the radio SD card under \SCRIPTS\TOOLS.

[![DSM Forward Programming](https://img.youtube.com/vi/sjIaDw5j9nE/0.jpg)](https://www.youtube.com/watch?v=sjIaDw5j9nE)

## DSM PID Flight log gain parameters for Blade micros

Lua telemetry script from [feathering on RCGroups](https://www.rcgroups.com/forums/showpost.php?p=46033341&postcount=20728) to facilitate setting the Gain Parameters on the Blade 150S FBL. It doesn't use Forward Programming but instead it just reads telemetry data from the Multi-module and displays it on a telemetry display.

It is very similar to the Telemetry Based Text Generator functionality on Spektrum transmitters where one doesn't need to rely on the angle of the swashplate to determine selection/value.

## Graupner HoTT.ua

Enable text configuration of the HoTT RX and sensors: Vario, GPS, ESC, GAM and EAM.

Need OpenTX 2.3.9 or above. Located on the radio SD card under \SCRIPTS\TOOLS.

Notes:
- Menu/MDL/Model is used to cycle through the detected sensors.
- It's normal to lose the telemetry feed while using the text mode configuration. Telemetry will resume properly if the script is exited by doing a short press on the exit button.

[![Text mode video](https://img.youtube.com/vi/81wd8NlF3Qw/0.jpg)](https://www.youtube.com/watch?v=81wd8NlF3Qw)

# Acer H101 cable repair
Acer H101 WMR DIY cable repair. The goal is to remove the original broken cable, and put some connectors on the headset for easy replacement of the cable in the future.

![proof](https://github.com/Levente96/AcerH101cablerepair/blob/main/IMG_20210410_191918.jpg "Working")

## Cable properties
Observing the cable and other headsets, it turns out the cable is a simple HDMI 2.0 and USB 3.0 SuperSpeed cable weaved together.

## HDMI 2.0
According to the ifixit guide, the hdmi part is ended woth a Spectra7 HT8181 HDMI 2.0 Cable Equalizer. This means it is a simple HDMI cable so we only need to look for the HDMI rules for these pins.
* This means that signals within a TMDS pair shall have matching lengths of ± 3mm.
* HDMI channel shall have matching lengths of ± 3mm
* TMDS pair shall have differential impedance of 100 Ω ± 5%

Not having proper equipment I was not able to measure the impedance properly, but approximating the impedance to length, with a 5 meter cable, I should have around 20cm to operate on.
On closer inspection the cables are the following for the HDMI:
* 4 wider shielded cables for TMDS pairs
* thin black
* thin yellow
* thin white
* thin green
* thin orange(the lighter one)
* thin brown(the darker one)

If you look into a male connector and number the pins as following:

| 19 | 17 | 15 | 13 | 11 | 9 | 7 | 5 | 3 | 1 |
|----|----|----|----|----|---|---|---|---|---|
| 18 | 16 | 14 | 12 | 10 | 8 | 6 | 4 | 2 | / |

The connections are the following(single color is the thin wire, double color is line and the major color in the pair (within the blue pairs)):
1. black
2. orange
3. yellow
4. brown
5. green
6. not connected!
7. white
8. white(yellow)
9. shield
10. yellow(yellow)
11. white(blue)
12. shield
13. blue(blue)
14. white(brown)
15. shield
16. brown(brown)
17: white(orange)
18: shield
19: orange(orange)

![soldered](https://github.com/Levente96/AcerH101cablerepair/blob/main/IMG_20210410_192151.jpg "Soldered")

## USB 3.0 SuperSpeed
The POC is done, still using the original cable, will replace next.

## Repair live
[https://www.twitch.tv/sloom96](https://www.twitch.tv/sloom96)

## Sources
* [iFixit Guide](https://www.ifixit.com/Teardown/Acer+Windows+Mixed+Reality+Headset+Developer+Edition+Teardown/96581)
* [HDMI2.0 Guide](https://ez.analog.com/video/w/documents/687/hdmi-layout-guideline)

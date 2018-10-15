---
layout: post
title:  "Ordering the kit and the first steps"
date:   2018-10-07 14:59:06 +0200
categories: Amp
---

**Wednesday 03-10-2018**: Just before 16:00 I ordered my JTM45 kit from ToneFactory for 555,- euro. Within minutes I received the build manual (which I've stored in Dropbox). A layout and schematic was not present. ToneFactory also did not have one, but provided me with with close matches. I found that the build-your-own-clone versions were even closer.
- [BYOC Schematic](http://byocelectronics.com/brit45schematic.pdf)
- [BYOC Layout](http://byocelectronics.com/jtm45-240v.pdf)
- [BYOC Build Instructions](http://byocelectronics.com/brit45instructions.pdf)
- [MableAudio Layout](http://www.mableaudio.com/uploadFile/Picture_small/201710251152564297.jpg)

Might check if ToneFactory can get a hi-res version, as they might get the kit there.

**Thursday 04-10-2018**: Around 12:00 the kit arrived. After some inspection it became clear some parts weren't delivered. A quick response on a mail to ToneFactory stated that they would sent the missing parts. See [PartList](/assets/PartList.xslx). The screw, nuts, etc. where nowhere close and the manual was also not clear. 

**Friday 05-10-2018**: I fixed to mechanical parts to the chassis (excluding front and back) to see if I could figure out which screws and nuts I was missing.

**Saturday 06-10-2018**: Eventually I went to a hardware store and got myself a variety of screws and nuts. I started with an amp cradle to facilitate the build.

**Sunday 07-10-2018**: I finished the amp cradle. ![cradle](/assets/cradle.jpg) Generated an [additional parts list](/assets/AdditionalParts.xlsx). [Das MusikDing](https://www.musikding.de/) has the 2W metal film resistors, 5W 750V Metal Oxide resistors and some handy stuff.

**Monday 08-10-2018**: Mailed ToneFactory about the missing parts. Created the empty and populated turret board in DIYLC as a preparation for the alterations I'm planning to do. Some of these changes will be: Use the preferred input network as in 'Designing Tube Preamps for Guitar and Bass'; Move the grid stoppers to the tube sockets; Change the bias supply to the one discussed at [the site](http://www.valvewizard.co.uk/bias.html) of Merlin Blencowe.

**Tuesday 08-10-2018**: DIYLC files are available:
- [Empty turretboard](/assets/TurretBoardOnly.diy)
- [Original turretboard](/assets/TurretBoardWithComponents.diy)
- [New turretboard](/assets/TurretBoardWithComponentsNew.diy)

New turretboard is currently rough, but the plan is it will be updated in the future. Also updated layout, links and images of this blog. Also posted it to http://tomkamphuys.github.io .

**Wednesday 10-10-2018**: Started a [thread](http://www.tdpri.com/threads/jtm45-build.881258/) at TDPRI. Started a schematic.

**Thursday 11-10-2018**: Band practice.

**Friday 12-10-2018**: Finished first iteration of schematic.

**Saturday 13-10-2018**: Received the parts from ToneFactory and installed them. Bias circuit etc. added to schematic.

**Sunday 14-10-2018**: As I will be using a multiple star grounding scheme (as described in Blencowe's book), which is different from the manual, I was looking around where I should put the safety-earth. I found no hole for a dedicated screw close to the mains inlet, so I will have to drill that.

I found that the input tube sockets were loose in their chassis mount. They were the shielded version, which I choose for (possible) lower noise. Three chassis clamps without a shield were also supplied and these did clamp the sockets tightly to the chassis.
![pre-amp tube socket](/assets/Photos/pre-ampTubeSocket.jpg)

Also the output tube sockets were loose. These have small metal parts that clamp the ceramic socket to the metal chassis mount, which I tightened with a long nose plier.
![output tube socket tightening](/assets/Photos/TubeSocketTightening.jpg)

Looking for resistors.

- Metal film
    - Vishay CPF1 1W, 250V, 1%
    - Vishay CPF2 2W, 350V, 1%
    - Vishay CPF3 3W, 500V, 1%
    - Vishay CCF60 1W, 500V, 1%
    - Vishay PR03 3W, 750V, 5% (probably). I think these are suitable for the plate load resistors and cathode follower cathode resistor. They need high power and voltage spec (see e.g. [Aiken](http://aikenamps.com/index.php/technical-q-a)), tolerance is not that important.
    - Yageo FMP200 2W, 500V, 1%

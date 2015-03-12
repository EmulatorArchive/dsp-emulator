# Introduction #

DSP Emulator v0.14 - Leniad 2001-2011


# Details #

Well, this is just another emulator... but, what's the difference? This is a pascal open source emulator using Delphi/Lazarus enviroment. There are not so many emulators in pascal...<br>
Yes, its open source, you can compile it yourself. But you cannot use it for commercial purposes.<br>
Why pascal, and not C, C++, Java or any other languaje? Well, pascal it is powerful enough to handle my emulator (120fps in spectrum driver with a Pentium CPU) and it is as good as many any other languages.<br>
You can not distribute this emulator with ROMS, except those that include the original ZIP file.<br>
Since version 0.9ß3 portability has begun to Lazarus/Free Pascal, so there is a Linux 32/64bits version available.<br><br>
<b>1-. Emulation</b>
<br>
<br>
<hr><br>
<br>
<br>
+ INFO: Emulator can handle ZIP format. You can load roms, tapes, snapshots or disks from a ZIP file.<br>
+ FILES NEEDED: In Windows the emulator needs the library 'SDL.DLL' that must be in the same folder that the executable, you can download it from the emulator site or you can download the last version from 'www.libsdl.org'.<br>
In Linux this library comes with your OS.<br><br>
The emulator includes (not in WIP versions) inside the ZIP the ROMS for Spectrum 48K/128K/+3 (and variants), Amstrad CPC 464/664/6128 and Coleco. You can download more tapes, disks and coleco ROMS from the 'Spectrum is Alive!!!' and 'Coleco is Alive!!!' pages, from the original emulator web.<br><br>
IS NOT ALLOWED DISTRIBUTE THIS EMULATOR WITH A COPYRIGHTED ROMS.<br><br>
<b>1.1-. Keys during emulation</b><br>
<br>
<br>
<hr><br>
<br>
<br>
General Keys:<br>
<blockquote>'F2' --> Full speed/Normal Speed<br>
'F3' --> Reset machine<br>
'F11' --> Changes emulation speed from 25%, 50%, 75% and 100%<br><br>
Arcade drivers basic keys are redefinable, by default are:<br>
'1' --> Start player one<br>
'2' --> Start player two<br>
'5' --> Insert coin<br>
'6' --> Inser Coin<br>
Keys for both players are redefinable, and you can select any joystick for any player and up to 6 buttons per player, by default keys are:<br>
Player 1 Up       --> Key 'Cursor UP'<br>
Player 1 Down     --> Key 'Cursor DOWN'<br>
Player 1 Left     --> Key 'Cursor LEFT'<br>
Player 1 Right    --> Key 'Cursor RIGHT'<br>
Player 1 Button 1 --> Key 'LEFT CONTROL'<br>
Player 1 Button 2 --> Key 'LEFT ALT'<br>
Any other control, by default, is not defined. You can redefine it in the main configuration menu.<br><br>
Spectrum/Amstrad basic keys:<br>
'F1' --> Play/Stop tape<br>
'F4' --> Save snapshot<br>
'F5' --> Remove Disk<br>
The joystick uses keys redefinable or external joystick.<br>
In Amstrad CPC for use 'F1' to 'F10' keys you must press right Shift.<br><br>
<b>1.2-. Language Files</b><br>
<br>
<br>
<hr><br>
<br>
<br>
DSP is by default in English, if you want to change it using 'File -> Language' or click the Settings button. You can select Castellano, Catalan, English, German, French, Brazilian or Italian.<br>
If you want to add another language, edit any file whith the extension '.lng' in the 'LNG' directory, rename it with the name of the languaje and send it to me to add it to the next version.<br>
If the language files are not present, the emulation can not start.<br><br>
<b>1.3-. Configure DSP</b><br>
<br>
<br>
<hr><br>
<br>
<br>
Clicking the Settings button you can configure the options in the emulator can select the language, quality of audio, video settings, default directories, redefine keys/use joystick and redefine main keys.<br>
In addition there are systems that can configure the options separately from the driver (Spectrum) and in arcade drivers, since version 0.12ß4 dipswitches can be modified through this button, to set game options.<br><br>
<b>1.4-. Audio</b><br>
<br>
<br>
<hr><br>
<br>
<br>
You can select the sound quality: 11025Khz, 22050Khz and 44100Khz. The more quality you choose more cristal crear will sound the emulation.<br>
If you do not have sound card the sound is turned off. Anyway you can select the option 'Mute' to save a few frames.<br><br>
<b>1.5-. Save Pictures</b><br>
<br>
<br>
<hr><br>
<br>
<br>
Since DSP 0.2wipb5 you can save GIF files from Spectrum emulation.<br>
Since 0.7ß2 version you can also save JPG and PNG formats from all drivers.<br><br>
<b>1.6-. Initial Game List</b><br>
<br>
<br>
<hr><br>
<br>
<br>
Since version 0.9 there is the possibility of booting DSP with the list of games, which shows the games, computers and consoles available. Further information on the availability of ROMS for each system, distribution year, conpany, etc.<br>
In general configuration you can choose this way of booting (show a game list), or the old way (load the last driver).<br><br>
<b>2-. Drivers</b><br>
<br>
<br>
<hr><br>
<br>
<br>
<b>2.1 Computers</b><br>
<br>
<br>
<hr><br>
<br>
<br>
<b>Spectrum</b><br>
<br>
<br>
<hr><br>
<br>
<br>
This driver have it's own configuration system. You can choose:<br>
- ROMS: You can change Spectrum's ROM. Configure you favorite ROM in 'ZIP' format (the name of the ROM inside the ZIP must be the same of ZIP name, for example 'SPECTRUM.ZIP' and the ROM inside the ZIP 'SPECTRUM.ROM') or in ROM format.<br>
By default the ROM files are:<br>
<blockquote>-Spectrum 16k/48k: 'SPECTRUM.ZIP' --> 'spectrum.rom' CRC: 0xDDEE531F<br>
-Spectrum 128k: 'SPEC128.ZIP' --> '128-0.rom' CRC: 0xE76799D2 and '128-1.rom' CRC: 0xB96A36BE<br>
-Spectrum +2: 'PLUS2.ZIP' --> 'plus2-0.rom' CRC: 0x5D2E8C66 and 'plus2-1.rom' CRC: 0x98B1320B<br>
-Spectrum +2A/+3: 'PLUS3.ZIP' --> 'plus3-0.rom' CRC: 0x30C9F490 , 'plus3-1.rom' CRC: 0xA7916B3F , 'plus3-2.rom' CRC: 0xC9A0B748 and 'plus3-3.rom' CRC: 0xB88FD6E3<br>
- Border: You can choose line by line emulation, pixel by pixel emulation (slowly but more exact) or disable border emulation (festest).<br>
- Lens Lock: Enable/disable the LensLock protection simulation<br>
- Spectrum 48K issue: Choose spectrum <a href='https://code.google.com/p/dsp-emulator/issues/detail?id=2'>issue 2</a> or 3<br>
- Joystick: You can choose from four joysticks; Kempston, Cursor, Sinclair 1 and Sinclair 2. Joystick is emulated with the redefinable keys or external joystick.<br>
- Gunstick/Lightgun: The mouse is used as Gunstick, and left button is used as fire.<br>
- AMX Mouse/Kempston Mouse: Use the mouse and the buttons.<br>
- ULA+: Enable/disable ULA+ extended colors. Supported since 0.9ß3 version.<br>
- AY8912 sound: Set the type of sound channels. Supports mono, stereo ABC channels and stereo ACB channels.<br>
- Tape loading sound: Enable/disable the sound of the tape when loading.<br>
- Speaker filter: Enable/disable filter to reduce the noise in speaker emulation.<br>
- Speaker oversample: Quality of speaker emulation.<br><br>
- Keyboard: Fully working keyboard emulation, and LShift and LControl working as Capshift and SimbolShift.<br>
- Virtual Tapes: Can load ZIP, TAP, TZX, PZX, WAV and CSW. Fully working spectrum load schemes (bleepload, alkatraz, original rom...). With the mouse you can move inside virtual tape and select the star possition. Tape begin to play when detects - LOAD "" - and stop when reaches the final.<br>
If inside the ZIP file there is a ROM file, emulator load fisrt ROM file and then loads then virtual tape.<br>
Also, if inside the ZIP is a .SCR image, it's used as a preview.<br>
- Snapshots: you can load Z80, DSP, SNA, SZX, ZX and SP. And you can save in SZX, Z80, DSP and SNA format.<br>
- Audio: Spectrum beeper, and in version wich have it there is a AY-8912 emulation. You can choose the speaker rate, as high you choose the better sound quality.<br>
- Floppy disk: Emulated all NEC-765 functions but write operations. Supports DSK format and 'extended' DSK.<br>
- To do: Contented memory is not working correctly at 100%.<br><br>
<b>Amstrad CPC 464,664 y 6128</b><br>
<br>
<br>
<hr><br>
<br>
<br>
- ROMS: By default the files are:<br>
-CPC-464: 'CPC464.ZIP' --> 'cpc464.rom' CRC: 0x40852F25<br>
-CPC-664: 'CPC664.ZIP' --> 'cpc664.rom' CRC: 0x9AB5A036 and 'amsdos.rom' CRC: 0x37F1BB31<br>
-CPC-6128: 'CPC6128.ZIP' --> 'cpc6128.rom' CRC: 0x9E827FE1 and 'amsdos.rom' CRC: 0x37F1BB31<br>
- Keyboard: Mapped the keys for each of the CPC. To press the '|' press left shift key and '><' next to the Z.<br>
- Joystick: emulated with the redefinable keys or external joystick.<br>
- Virtual Tape: you can load ZIP, CDT, WAV and CSW. It's working the classical loading squemes (bleepload, alkatraz, SpeedLock ...). Use the mouse to move inside the virtual tape and select the starting position.<br>
- Sound: Polyphonic sound from AY-8912 chip<br>
- Floppy disk: Emulated the functions of the NEC-765, just missing writing functions. Supports the format 'DSK' and the 'extended' DSK formats.<br>
-To do:<br>
-Snapshots are not implemented.<br>
-Some disk protections are not working (a few).<br>
-Some video effect are missing (M6845 video)<br><br>
<b>2.2 Consoles</b><br>
<br>
<br>
<hr><br>
<br>
<br>
<b>NES</b><br>
<br>
<br>
<hr><br>
<br>
<br>
-Cartridge: Supports '.nes' ROM format, compressed in ZIP format or not.<br>
-Keys: Use the redefined keys and 'SELECT' uses coin 1 (by default is mapped as key '5' and 'START' uses start player 1 (by default is mapped as the '1' key).<br>
-Sound: Support sound, only remains DPCM<br>
-Mappers: Supports 0,1,2,3,4,7,66 y 87<br>
-To Do<br>
- Snapshots<br>
- Add more mappers<br>
- Video Timmings<br><br>
<b>GameBoy/Gameboy Color</b><br>
<br>
<br>
<hr><br>
<br>
<br>
-ROM: Not required, but if present are loaded and run as the original console.<br>
The default ROMs names are<br>
-GameBoy: 'GAMEBOY.ZIP' --> 'dmg_boot.bin' CRC: 0x59C8598E<br>
-GameBoy Color: 'GBCOLOR.ZIP' --> 'gbc_boot.1' CRC: 0x779EA374 and 'gbc_boot.2' CRC: 0xF741807D<br>
-Keys: Use the redefined keys and 'SELECT' uses coin 1 (by default is mapped as key '5' and 'START' uses start player 1 (by default is mapped as the '1' key).<br>
-Cartridges: Supports cartridges '.gb' and '.gbc', compressed or not.<br>
Mappers are supported are MBC0, MBC1 and MBC5.<br>
-To Do<br>
- Snapshots<br>
- Audio problems, do not work  with high frequencies<br>
- Video Timmings<br>
- Add more mappers<br><br>
<b>ColecoVision</b><br>
<br>
<br>
<hr><br>
<br>
<br>
-ROM: The ROM is needed for emulation<br>
ROM file name is<br>
-Coleco: 'COLECO.ZIP' --> 'coleco.rom' CRC: 0x3AA93EF3<br>
-Joystick: The numbers on the keyboard from '1'to '0' emulate the keys on the two joysticks. Keys 'Q' and 'W' emulate the Keys '<code>*</code>' and '#' of the two joysticks also, main joystick is emulated with the redefinable keys or external joystick (the secondary joystick does not have keys assigned). Does not support (still) the special joysticks.<br>
-Cartridges: It supports the standard game cartridges (not expansion cartridges) with 'ROM' and 'COL' file extension. Support ZIP files, of course.<br>
-Sound: Support the sound with AY-8912<br><br>
<b>Chip 8/Super Chip8</b><br>
<br>
<br>
<hr><br>
<br>
<br>
-ROM: Does not have. It's a simulation of a pseudo CPU.<br>
-Keyboard: Mapped the system keys<br>
</blockquote><code>1 2 3 A --&gt; 1 2 3 4</code><br>
<code>4 5 6 B --&gt; Q W E R</code><br>
<code>7 8 9 C --&gt; A S D F</code><br>
<code>D 0 E F --&gt; Z X C V</code><br>
-Sound: basic sound<br>
-Video: Supports 64x32 format from Chip8, 64x64 from Chip8 Hires and 128x64 from SuperChip8<br>
-Files: Supports '.CH8' y '.BIN' formats<br>
-To do<br>	- Snapshots<br><br>
<b>2.3 Arcade</b><br>
<br>
<br>
<hr><br>
<br>
<br>
<b>2.3.1 Samples</b>

<hr>

<br>
Some games, given the difficulty of emulating old sound systems, uses 'samples'. Such files are portions of digitized sound, played instead of emulating the sound system.br><br>
Currently only some drivers use wholly or partly this system.<br>
If you want the emulator to use the samples, put the files with the same name as the ROM in a folder named 'samples'.<br>
<br>
<b>2.3.2 Emulated Systems</b>

<hr>

<br>
<table><thead><th> <b>Name</b></th><th> <b>ROM</b>          </th><th> <b>Completed</b>  </th><th> <b>Notes</b></th></thead><tbody>
<tr><td>Phoenix                    </td><td> PHOENIX.ZIP  </td><td>      99,1  </td><td> Preliminary analog sound, music (TMS36XX) and digital sound are OK</td></tr>
<tr><td>Bombjack                   </td><td> BOMBJACK.ZIP </td><td>     100    </td></tr>
<tr><td>Pac-man                    </td><td> PACMAN.ZIP   </td><td>     100    </td><td> Pac-man Hardware</td></tr>
<tr><td>Ms. Pac-man                </td><td> MSPACMAN.ZIP </td><td>     100    </td><td> Pac-man Hardware</td></tr>
<tr><td>Mysterious Stones          </td><td> MYSTSTON.ZIP </td><td>     100    </td></tr>
<tr><td>Frogger                    </td><td> FROGGER.ZIP  </td><td>     100    </td><td> Galaxian Hardware</td></tr>
<tr><td>Galaxian                   </td><td> GALAXIAN.ZIP </td><td>      95    </td><td> Galaxian Hardware<br>Partial sound with samples</td></tr>
<tr><td>Jump Bug                   </td><td> JUMPBUG.ZIP  </td><td>     100    </td><td> Galaxian Hardware</td></tr>
<tr><td>Moon Cresta                </td><td> MOONCRST.ZIP </td><td>      90    </td><td> Galaxian Hardware<br>No sound</td></tr>
<tr><td>Scramble                   </td><td> SCRAMBLE.ZIP </td><td>     100    </td><td> Galaxian Hardware</td></tr>
<tr><td>Super Cobra                </td><td> SCOBRA.ZIP   </td><td>     100    </td><td> Galaxian Hardware</td></tr>
<tr><td>Amidar                     </td><td> AMIDAR.ZIP   </td><td>     100    </td><td> Galaxian Hardware</td></tr>
<tr><td>Donkey Kong                </td><td> DKONG.ZIP    </td><td>     100    </td><td> Donkey Kong Hardware<br>Samples sound</td></tr>
<tr><td>Donkey Kong Junior         </td><td> DKONGJR.ZIP  </td><td>     100    </td><td> Donkey Kong Hardware<br>Samples sound</td></tr>
<tr><td>Donkey Kong 3              </td><td> DKONG3.ZIP   </td><td>     100    </td><td> Donkey Kong Hardware</td></tr>
<tr><td>Black Tiger                </td><td> BLKTIGER.ZIP </td><td>     100    </td></tr>
<tr><td>Green Beret                </td><td> GBERET.ZIP   </td><td>     100    </td></tr>
<tr><td>Commando                   </td><td> COMMANDO.ZIP </td><td>     100    </td></tr>
<tr><td>Ghost'n'Goblins            </td><td> GNG.ZIP      </td><td>     100    </td></tr>
<tr><td>Mikie                      </td><td> MIKIE.ZIP    </td><td>     100    </td></tr>
<tr><td>Shaolin's Road             </td><td> SHAOLIN.ZIP  </td><td>     100    </td></tr>
<tr><td>Yie Ar Kung-Fu             </td><td> YIEAR.ZIP    </td><td>     100    </td></tr>
<tr><td>Son Son                    </td><td> SONSON.ZIP   </td><td>     100    </td></tr>
<tr><td>Asteroids                  </td><td> ASTEROID.ZIP </td><td>     100    </td><td> Analog sound and samples</td></tr>
<tr><td>Star Force                 </td><td> STARFORC.ZIP </td><td>     100    </td></tr>
<tr><td>Rygar                      </td><td> RYGAR.ZIP    </td><td>     100    </td><td> Tecmo Hardware</td></tr>
<tr><td>Silk Worm                  </td><td> SILKWORM.ZIP </td><td>     100    </td><td> Tecmo Hardware</td></tr>
<tr><td>Pitfall II                 </td><td> PITFALL2.ZIP </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Teddy Boy Blues            </td><td> TEDDYBB.ZIP  </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Wonder Boy                 </td><td> WBOY.ZIP     </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Wonder Boy in Monster Land </td><td> WBML.ZIP     </td><td>     100    </td><td> Sega System 2</td></tr>
<tr><td>Choplifter                 </td><td> CHOPLIFT.ZIP </td><td>     100    </td><td> Sega System 2</td></tr>
<tr><td>Mister Viking              </td><td> MRVIKING.ZIP </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Sega Ninja                 </td><td> SEGANINJ.ZIP </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Up'n Down                  </td><td> UPNDOWN.ZIP  </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Flicky                     </td><td> FLICKY.ZIP   </td><td>     100    </td><td> Sega System 1</td></tr>
<tr><td>Pooyan                     </td><td> POOYAN.ZIP   </td><td>     100    </td></tr>
<tr><td>Jungler                    </td><td> JUNGLER.ZIP  </td><td>     100    </td><td> Rally X Hardware</td></tr>
<tr><td>Rally X                    </td><td> RALLYX.ZIP   </td><td>     100    </td><td> Rally X Hardware<br>Explosion sound uses samples</td></tr>
<tr><td>New Rally X                </td><td> NRALLYX.ZIP  </td><td>     100    </td><td> Rally X Hardware<br>Explosion sound uses samples</td></tr>
<tr><td>City Connection            </td><td> CITYCON.ZIP  </td><td>     100    </td></tr>
<tr><td>Burger Time                </td><td> BTIME.ZIP    </td><td>     100    </td></tr>
<tr><td>Express Raider             </td><td> EXPRRAID.ZIP </td><td>     100    </td></tr>
<tr><td>Super Basketball           </td><td> SBASKETB.ZIP </td><td>     100    </td></tr>
<tr><td>Lady Bug                   </td><td> LADYBUG.ZIP  </td><td>     100    </td></tr>
<tr><td>Tehkan World Cup           </td><td> TEHKANWC.ZIP </td><td>      99    </td><td> Problem with CPUs syncronization</td></tr>
<tr><td>Popeye                     </td><td> POPEYE.ZIP   </td><td>     100    </td></tr>
<tr><td>Psychic 5                  </td><td> PSYCHIC5.ZIP </td><td>      96    </td><td> Missing Alpha render (background and sprites) and colour intensity</td></tr>
<tr><td>Kung-Fu Master             </td><td> KUNGFUM.ZIP  </td><td>     100    </td><td> Irem M62 Hardware</td></tr>
<tr><td>Spelunker                  </td><td> SPELUNKR.ZIP </td><td>     100    </td><td> Irem M62 Hardware</td></tr>
<tr><td>Spelunker II               </td><td> SPELUNK2.ZIP </td><td>     100    </td><td> Irem M62 Hardware</td></tr>
<tr><td>Lode Runner                </td><td> LODERUN.ZIP  </td><td>     100    </td><td> Irem M62 Hardware</td></tr>
<tr><td>Lode Runner II             </td><td> LODERUN2.ZIP </td><td>     100    </td><td> Irem M62 Hardware</td></tr>
<tr><td>Terra Cresta               </td><td> TERRACRE.ZIP </td><td>     100    </td></tr>
<tr><td>Shoot Out!                 </td><td> SHOOTOUT.ZIP </td><td>     100    </td></tr>
<tr><td>Vigilante                  </td><td> VIGILANT.ZIP </td><td>     100    </td></tr>
<tr><td>Jackal                     </td><td> JACKAL.ZIP   </td><td>     100    </td></tr>
<tr><td>Bubble Bobble              </td><td> BUBLBOBL.ZIP </td><td>     100    </td></tr>
<tr><td>Prehistoric Isle in 1930   </td><td> PREHISLE.ZIP </td><td>     100    </td></tr>
<tr><td>Tiger Road                 </td><td> TIGEROAD.ZIP </td><td>     100    </td><td> Tiger Road Hardware</td></tr>
<tr><td>F1 Dream                   </td><td> F1DREAM.ZIP  </td><td>     100    </td><td> Tiger Road Hardware</td></tr>
<tr><td>Snow Bros                  </td><td> SNOWBROS.ZIP </td><td>     100    </td></tr>
<tr><td>Toki                       </td><td> TOKI.ZIP     </td><td>      95    </td><td> Some problems with sound, M68000 core bugs?</td></tr>
<tr><td>Contra                     </td><td> CONTRA.ZIP   </td><td>      99    </td><td> Some graphics bugs</td></tr>
<tr><td>Mappy                      </td><td> MAPPY.ZIP    </td><td>     100    </td><td> Mappy Hardware</td></tr>
<tr><td>Dig-Dug II                 </td><td> DIGDUG2.ZIP  </td><td>     100    </td><td> Mappy Hardware</td></tr>
<tr><td>Super Pacman               </td><td> SUPERPAC.ZIP </td><td>     100    </td><td> Mappy Hardware</td></tr>
<tr><td>Rastan                     </td><td> RASTAN.ZIP   </td><td>     100    </td></tr>
<tr><td>Legendary Wings            </td><td> LWINGS.ZIP   </td><td>     100    </td><td> Legendary Wings Hardware</td></tr>
<tr><td>Section Z                  </td><td> SECTIONZ.ZIP </td><td>     100    </td><td> Legendary Wings Hardware</td></tr>
<tr><td>Trojan                     </td><td> TROJAN.ZIP   </td><td>     100    </td><td> Legendary Wings Hardware</td></tr>
<tr><td>Street Fighter             </td><td> SF.ZIP       </td><td>     100    </td></tr>
<tr><td>Galaga                     </td><td> GALAGA.ZIP   </td><td>     100    </td><td> Galaga Hardware</td></tr>
<tr><td>DigDug                     </td><td> DIGDUG.ZIP   </td><td>      95    </td><td> Galaga Hardware<br>Problems with IO 53XX (dipswitch)</td></tr>
<tr><td>Xain'd Sleena              </td><td> XSLEENA.ZIP  </td><td>     100    </td></tr>
<tr><td>Hard Head                  </td><td> HARDHEAD.ZIP </td><td>     100    </td><td> Suna Hardware</td></tr>
<tr><td>Hard Head 2                </td><td> HARDHED2.ZIP </td><td>      10    </td><td> Basic driver</td></tr>
<tr><td>Saboten Bombers            </td><td> SABOTENB.ZIP </td><td>     100    </td><td> NMK 16 Hardware</td></tr>
<tr><td>Bomb Jack Twin             </td><td> BJTWIN.ZIP   </td><td>     100    </td><td> NMK 16 Hardware</td></tr>
<tr><td>Knuckle Joe                </td><td> KNCLJOE.ZIP  </td><td>     100    </td></tr>
<tr><td>Wardner                    </td><td> WARDNER.ZIP  </td><td>     100    </td></tr>
<tr><td>Big Karnak                 </td><td> BIGKARNC.ZIP </td><td>     100    </td><td> Gaelco Hardware</td></tr>
<tr><td>Thunder Hoop               </td><td> THOOP.ZIP    </td><td>     100    </td><td> Gaelco Hardware</td></tr>
<tr><td>Squash                     </td><td> SQUASH.ZIP   </td><td>     100    </td><td> Gaelco Hardware</td></tr>
<tr><td>Biomechanical Toy          </td><td> BIOMTOY.ZIP  </td><td>     100    </td><td> Gaelco Hardware</td></tr>
<tr><td>Exed Exes                  </td><td> EXEDEXES.ZIP </td><td>     100    </td></tr>
<tr><td>Gun.Smoke                  </td><td> GUNSMOKE.ZIP </td><td>     100    </td><td> Gun.Smoke Hardware</td></tr>
<tr><td>1943: The Battle of Midway </td><td> 1943.ZIP     </td><td>     100    </td><td> Gun.Smoke Hardware</td></tr>
<tr><td>1943 Kai: Midway Kaisen    </td><td> 1943KAI.ZIP  </td><td>     100    </td><td> Gun.Smoke Hardware</td></tr>
<tr><td>1942                       </td><td> 1942.ZIP     </td><td>     100    </td></tr>
<tr><td>Jail Break                 </td><td> JAILBREK.ZIP </td><td>     100    </td></tr>
<tr><td>Circus Charlie             </td><td> CIRCUSC.ZIP  </td><td>     100    </td></tr>
<tr><td>Iron Horse                 </td><td> IRONHORS.ZIP </td><td>     100    </td></tr>
<tr><td>R-Type                     </td><td> RTYPE.ZIP    </td><td>      70    </td><td> Irem M72 Hardware<br>Missing sound and controls, some sprite problems and missing some NEC v30 opcodes</td></tr>
<tr><td>Break Thru                 </td><td> BRKTHRU.ZIP  </td><td>     100    </td><td> Break Thru Hardware</td></tr>
<tr><td>Darwin 4078                </td><td> DARWIN.ZIP   </td><td>     100    </td><td> Break Thru Hardware</td></tr>
<tr><td>Super Real Darwin          </td><td> SRDARWIN.ZIP </td><td>     100    </td></tr>
<tr><td>Double Dragon              </td><td> DDRAGON.ZIP  </td><td>     100    </td><td> Double Dragon Hardware</td></tr>
<tr><td>Double Dragon II - The Revenge</td><td> DDRAGON2.ZIP </td><td>     100    </td><td> Double Dragon Hardware</td></tr>
<tr><td>Mr. Do!                    </td><td> MRDO.ZIP     </td><td>     100    </td></tr>
<tr><td>The Glob                   </td><td> THEGLOB.ZIP  </td><td>     100    </td><td> Epos Hardware</td></tr>
<tr><td>Super Glob                 </td><td> SUPRGLOB.ZIP </td><td>    100    </td><td> Epos Hardware</td></tr>
<tr><td>Tiger Heli                 </td><td> TIGERH.ZIP   </td><td>     100    </td><td> Slap Fight Hardware</td></tr>
<tr><td>Slap Fight                 </td><td> SLAPFIGH.ZIP </td><td>     100    </td><td> Slap Fight Hardware</td></tr>
<tr><td>The Legend of Kage         </td><td> LKAGE.ZIP    </td><td>     100    </td></tr>
<tr><td>Cabal                      </td><td> CABAL.ZIP    </td><td>      95    </td><td> Bugs in M68000 core</td></tr>
<tr><td>Ghouls and Ghosts          </td><td> GHOULS.ZIP   </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Final Fight                </td><td> FFIGHT.ZIP   </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>The King of Dragons        </td><td> KOD.ZIP      </td><td>     100    </td><td> Capcom Play System 1 - CPS1<br>Missing third player controls</td></tr>
<tr><td>Street Fighter II The World Warrior</td><td> SF2.ZIP      </td><td>      95    </td><td> Capcom Play System 1 - CPS1<br>Missing some controls and scroll row</td></tr>
<tr><td>Strider                    </td><td> STRIDER.ZIP  </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Three Wonders              </td><td> 3WONDERS.ZIP </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Captain Commando           </td><td> CCOMANDO.ZIP </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Knights of the Round       </td><td> KNIGHTS.ZIP  </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Street Fighter II' Champion Edition </td><td> SF2CE.ZIP    </td><td>      95    </td><td> Capcom Play System 1 - CPS1<br>Missing some controls and scroll row</td></tr>
<tr><td>Cadillacs and Dinosaurs    </td><td> DINO.ZIP     </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>The Punisher               </td><td> PUNISHER.ZIP </td><td>     100    </td><td> Capcom Play System 1 - CPS1</td></tr>
<tr><td>Shinobi                    </td><td> SHINOBI.ZIP  </td><td>      95    </td><td> Sega System 16A<br>Missing PCM Sound</td></tr>
<tr><td>Alex Kidd                  </td><td> ALEXKIDD.ZIP </td><td>      95    </td><td> Sega System 16A<br>Missing PCM Sound</td></tr>
<tr><td>Fantasy Zone               </td><td> FANTZONE.ZIP </td><td>      95    </td><td> Sega System 16A<br>Missing PCM Sound</td></tr>
<tr><td>Time Pilot '84             </td><td> TP84.ZIP     </td><td>      99    </td><td> Missing RC filters</td></tr>
<tr><td>Tutankham                  </td><td> TUTANKHM.ZIP </td><td>     100    </td></tr>
<tr><td>Pang                       </td><td> PANG.ZIP     </td><td>      95    </td><td> Missing YM2413</td></tr>
<tr><td>Ninja Kid II               </td><td> NINJAKD2.ZIP </td><td>      95    </td><td> UPL Hardware<br>No PCM sound</td></tr>
<tr><td>Ark Area                   </td><td> ARKAREA.ZIP  </td><td>     100    </td><td> UPL Hardware</td></tr>
<tr><td>Mutant Night               </td><td> MNIGHT.ZIP   </td><td>     100    </td><td> UPL Hardware</td></tr>
<tr><td>Sky Kid                    </td><td> SKYKID.ZIP   </td><td>     100    </td></tr>
<tr><td>Rolling Thunder            </td><td> RTHUNDER.ZIP </td><td>      95    </td><td> Namco System 86<br>Missing ADPCM sound</td></tr>
<tr><td>Hopping Mappy              </td><td> HOPMAPPY.ZIP </td><td>     100    </td><td> Namco System 86</td></tr>
<tr><td>Sky Kid Deluxe             </td><td> SKYKIDDX.ZIP </td><td>     100    </td><td> Namco System 86</td></tr>
<tr><td>Roc'n Rope                 </td><td> ROCNROPE.ZIP </td><td>     100    </td></tr>
<tr><td>Repulse                    </td><td> REPULSE.ZIP  </td><td>     100    </td></tr>
<tr><td>The NewZealand Story       </td><td> TNZS.ZIP     </td><td>     100    </td><td> The NewZealand Story Hardware</td></tr>
<tr><td>Insector X                 </td><td> INSECTX.ZIP  </td><td>     100    </td><td> The NewZealand Story Hardware</td></tr>
<tr><td>Pacland                    </td><td> PACLAND.ZIP  </td><td>     100    </td></tr>
<tr><td>Mario Bros.                </td><td> MARIO.ZIP    </td><td>     100    </td><td> Full sound with samples</td></tr>
<tr><td>Solomon Key                </td><td> SOLOMON.ZIP  </td><td>     100    </td></tr>
<tr><td>Combat School              </td><td> COMBATSC.ZIP </td><td>      95    </td><td> Minimal graphics problems</td></tr>
<tr><td>Heavy Unit                 </td><td> HVYUNIT.ZIP  </td><td>     100    </td></tr>
<tr><td>P.O.W. - Prisoners of War  </td><td> POW.ZIP      </td><td>     100    </td><td> SNK 68K Hardware</td></tr>
<tr><td>Street Smart               </td><td> STREETSM.ZIP </td><td>     100    </td><td> SNK 68K Hardware</td></tr>
<tr><td>Ikari III - The Rescue     </td><td> IKARI3.ZIP   </td><td>     100    </td><td> SNK 68K Hardware</td></tr>
<tr><td>Search and Rescue          </td><td> SEARCHAR.ZIP </td><td>     100    </td><td> SNK 68K Hardware</td></tr>
<tr><td>P47 - Phantom Fighter      </td><td> P47.ZIP      </td><td>     100    </td><td> Jaleco Megasystem</td></tr>
<tr><td>Rodland                    </td><td> RODLAND.ZIP  </td><td>     100    </td><td> Jaleco Megasystem</td></tr>
<tr><td>Saint Dragon               </td><td> STDRAGON.ZIP </td><td>      95    </td><td> Jaleco Megasystem<br>Missing Protection</td></tr>
<tr><td>Time Pilot                 </td><td> TIMEPLT.ZIP  </td><td>     100    </td></tr>
<tr><td>Pengo                      </td><td> PENGO.ZIP    </td><td>     100    </td></tr>
<tr><td>Twin Cobra                 </td><td> TWINCOBR.ZIP </td><td>     100    </td><td> Twin Cobra Hardware</td></tr>
<tr><td>Flying Shark               </td><td> FSHARK.ZIP   </td><td>     100    </td><td> Twin Cobra Hardware</td></tr>
<tr><td>Jr. Pac-Man                </td><td> JRPACMAN.ZIP </td><td>     100    </td></tr>
<tr><td>Robocop                    </td><td> ROBOCOP.ZIP  </td><td>     100    </td><td> Deco0 Hardware</td></tr>
<tr><td>Baddudes vs. DragonNinja   </td><td> BADDUDES.ZIP </td><td>     100    </td><td> Deco0 Hardware</td></tr>
<tr><td>Hippodrome                 </td><td> HIPPODRM.ZIP </td><td>      95    </td><td> Deco0 Hardware<br>Some times the game resets, maybe Hu6280 bugs?</td></tr>
<tr><td>Tumble Pop                 </td><td> TUMBLEP.ZIP  </td><td>     100    </td></tr>
<tr><td>Funky Jet                  </td><td> FUNKYJET.ZIP </td><td>     100    </td></tr>
<tr><td>Super Burger Time          </td><td> SUPBTIME.ZIP </td><td>     100    </td></tr>
<tr><td>Caveman Ninja              </td><td> CNINJA.ZIP   </td><td>     100    </td><td> Caveman Ninja Hardware</td></tr>
<tr><td>Robocop 2                  </td><td> ROBOCOP2.ZIP </td><td>     100    </td><td> Caveman Ninja Hardware</td></tr>
<tr><td>Diet Go Go                 </td><td> DIETGO.ZIP   </td><td>     100    </td></tr>
<tr><td>Act-Fancer Cybernetick Hyper Weapon</td><td> ACTFANCR.ZIP </td><td>      95    </td><td> Bugs on Hu6280</td></tr>
<tr><td>Arabian                    </td><td> ARABIAN.ZIP  </td><td>     100    </td></tr>
<tr><td>Pirate Ship Higemaru       </td><td> HIGEMARU.ZIP </td><td>     100    </td></tr>
<tr><td>Bagman                     </td><td> BAGMAN.ZIP   </td><td>      95    </td><td> Bagman Hardware<br>Missing TSM 5110 sound</td></tr>
<tr><td>Super Bagman               </td><td> SBAGMAN.ZIP  </td><td>      95    </td><td> Bagman Hardware<br>Missing TSM 5110 sound</td></tr>
<tr><td>Congo                      </td><td> CONGO.ZIP    </td><td>      20    </td><td> Zaxxon Hardware<br>Missing controls, audio, background and palette</td></tr>
<tr><td> Total: 166</td></tr></blockquote></tbody></table>

<b>3-. Contribute/Code distribution</b><br>
<br>
<br>
<hr><br>
<br>
<br>
If you make any improvements to any driver, processor, main code, etc. or add drivers, please send the changes to me, so they can be added to the main code.<br>
If you use part of the code of the emulator for any non commercial purpose, you only need to add in the documentation/source something like 'Z80 core written by Leniad'. And please send me a email to see the written program. :-)<br><br>
<b>4-. Acknowledgments</b><br>
<br>
<br>
<hr><br>
<br>
<br>
- First, of course, the MAME team. Without them, this emulator never had existed, thanks to distribute the source code to help many people, people like me. (And of course the 'MAME guru' Nicola Salmoria).<br>
- Chris Cowley, author of VBSpec, from where I've pick a lot of information about Spectrum. In addition I've also got the part of the AY-3-8912 of its emulator, which is an excellent conversion that comes with MAME.<br>
- Raul Gomez Sanchez author of the <a href='https://code.google.com/p/dsp-emulator/source/detail?r=80'>R80</a>, one of the best Spectrum emulators for DOS, which use your debugger to trace errors in my emulator Z80.<br>
- World of Spectrum, they have many tapes, snapshots, in addition many technical information, including the format TZX, DSK, Z80, etc.<br>
- javi<code>[@]</code>fsmail.net that helped me in a moment of desperation, with directSound.<br>
- Thanks to Michael Franzen, who sent me drivers for Pooyan, Coleco, System1, Chip8 and many others to be included in DSP.<br>
- Thanks to Tom Walker, he sent me his driver CPS1 where I got and understood a lot of information.<br>
- Thanks to sremulador he made the drivers list, and constant source updates and for begin the rewriting of NES driver<br>
- And many pages of the Internet, many documents ... and people who I forget, thank you all.<br><br>
<b>5-. Copyright</b><br>
<br>
<br>
<hr><br>
<br>
<br>
The Coleco and Pooyan has been rewrited from the originals by Michael Franzen.<br>
The CPS1 has been rewrited from the original by Tomas Walker.<br>
The rest of the drivers the Z80 core, M6502 core, M6809 (HD6309) core, M68000 core, M680X core, TMS-32010 core, NEC v20/v30/v33 core, LR35902 core, M6805 core, MCS51 core,Hu6280 core and MB88XX core are writed by me, Leniad.<br>
AY-3-8912 emulator is a conversion from Chris Cowley, but the original emulator come from MAME team.<br>
SN76496, YM2203, TMS36XX, VLM-5030, YM3812/YM3526, YM2151, i8255, OKI6295, UPD7759, Z80PIO and Z80CTC emulators are a conversion writed by me from MAME original.<br>
TMS99XX emulator have been rewrited from the original by Michael Franzen and have parts from MAME.<br>
NEC765 emulator is a conversion writed and adapted by me, from MESS original.<br>
GameBoy/GameBoy Color sound emulator is a conversion writed by me from MESS original.<br>
NES sound emulator is a conversion writed by me from MAME original.<br>
All Spectrum, CPC464, CPC664 and CPC6128 roms are copyright of Amstrad.<br><br>
<b>6-. Contact & Links</b><br>
<br>
<br>
<hr><br>
<br>
<br>
If you want to contact me, send me feedback or anything just use leniad2<code>[@]</code>hotmail.com<br>
My DSP home page leniad.cjb.net<br>
You can also download the offical version and WIP versions from Google Code page<br><br>
<a href='http://code.google.com/p/dsp-emulator/'>http://code.google.com/p/dsp-emulator/</a><br><br>
If you want info...<br>
www.mamedev.org<br>
www.aarongiles.com<br>
www.emulatronia.com<br><br>
if you want spectrum tapes, snapshot, info...<br>
leniad.cjb.net/sp<br>
www.worldofspectrum.org<br>
tzxvault.retrogames.com<br>
zx.dyndns.org/trastero<br>
www.speccy.org/spa2<br><br>
If you want Coleco games<br>
leniad.cjb.net/coleco
# Deadline Pro changelog

Before launch, Deadline Pro's builds were numbered 1.0.0 to 1.0.3. Until launch they are numbered 0.x, and launch will be 1.0.

## 0.9.18 · 7 Nov 2026
- **A macro and its module light each other.** The glow is always on the other side. Choose a module in CONTROL and its macro glows once (its panel stroke and pointer LED), then keeps a light stroke. Grab a macro and it takes the light stroke at once, while its module glows once in the chain, the grid and the panel. Only a change of module glows, in the colour the skin draws its CONTROL strokes, and only while CONTROL is showing. LIMITER lights LEVEL and CEILING. The LED rings are never touched, so the value always reads. Settings > DISPLAY turns it off.
- **Command-click no longer resets a knob.** Command-click (Ctrl-click on Windows) on a main panel knob behaves as a normal click. Option-click (Alt-click on Windows) and double-click still reset, and the Field Guide now says so.

## 0.9.12 · 5 Nov 2026
- **Readouts let the display show through.** The dark surround behind the figures in every module's graph is now one value, 80%.
- **RESET clears the peak holds.** Reset Macros and Reset All in the header now clear the red peak holds on the meters as well. Clicking a readout still works as before.
- **HIGH reads as one spectrum.** PRESENCE, BITE and AIR blend into one another, with no divider lines through them, and the frequency marks are short ticks. ROOF dims the high end less, so it stays readable. The ROOF line now runs behind the headings, the frequency figures and the curve, so the words stay clear.
- **COMP's scope sits in the middle.** The waveform is centred in its display and slightly larger.
- **COMP shows what SIDECHAIN HPF does to the gain reduction.** Gain reduction hangs from the top of the scope and, on the same scale, what the filter changes in it rises from the bottom, with an HPF figure beside IN, GR and OUT. The gain reduction also shows in orange on the music's peaks. GR and HP are named in the left-hand corners on a part-opaque surround, readable with the metering running under them.
- **Shift is a real fine-tune.** Hold Shift while dragging any knob, on the main view, a tile or a panel, or anything you can drag on a graph, and it moves four times finer. Shift still lifts the snap at zero on bipolar knobs.
- **The smooth analyser fades out at the bottom** instead of stopping on the floor line.
- **The Field Guide is written from the build.** Its version, its list of every control and its What's new section come from the build itself, and the build stops if a control has no words. Search text and the help link are left-aligned, and body text and search text sit centred in their space.

## 0.9.10 · 3 Nov 2026
- **Option-click resets a control in CONTROL too, as in Pro Tools.** In the CONTROL view, Option-click (Alt-click on Windows) on any knob, in a module's panel or on its tile, now returns it to its default, as it already did on the main panel. Double-click in a module's panel still does the same. Option-click on a module's name or light on the main panel still bypasses everything except the limiter, and Option-Shift-click still bypasses everything.

## 0.9.9 · 3 Nov 2026
- **PHASE switches without a click.** Switching INPUT, PHASE between normal and inverted during playback no longer makes a plop. The polarity now turns over smoothly in 20 milliseconds instead of all at once. With PHASE left alone the sound is exactly as before.

## 0.9.8 · 2 Nov 2026
- **Evenly spaced analyser bars at every window size.** The spectrum's bars, fine and wide, keep the same width and the same gap between them however you size the window. Before, some gaps came out wider than others at some sizes.

## 0.9.7 · 1 Nov 2026
- **The COMP curve shows the knee.** KNEE now rounds the corner of the compressor curve, from a sharp corner at 0 dB to a long, gentle bend at 24 dB, and the shaded band is gone. The curve follows KNEE, RATIO and THRESHOLD as you turn them, even with playback stopped. The knee is easiest to see at higher ratios.

## 0.9.6 · 1 Nov 2026
- **KNEE turns.** COMP's KNEE knob was stuck at 12 dB in 0.9.4 and 0.9.5. It now moves through its full range, 0 dB (a hard knee) to 24 dB (very soft).

## 0.9.5 · 1 Nov 2026
- **The right icon everywhere.** The installer and the standalone app now show Deadline Pro's own icon, the one in Atomic Manager. Nothing else changes.

## 0.9.4 · 1 Nov 2026
- **CONTROL readouts that hold still.** In MID, LOW and HIGH every figure now sits in a fixed place, sized for its widest value, so nothing jumps, slides or covers the curve as you adjust it.
- **HIGH in three zones.** PRESENCE, BITE and AIR each have their own coloured zone, and each dot stays inside it. Each heading shows its band's amount and frequency. Drag a dot up or down for AMOUNT, sideways for frequency, and with Option for that band's Q. The master Q reads at the bottom left.
- **LOW, clearer.** SUB-CUT reads on one line with its frequency, and SUB-CUT and BASS-COMP are easier to read. HARMONICS is now a bar that fills and warms from blue to orange and red the harder it works, instead of flashing. Dragging the WEIGHT dot moves frequency sideways and amount up and down, steadily.
- **A new COMP display, and a KNEE control.** Three views side by side: the compressor curve with the knee shaded, a scrolling view of the music with gain reduction hanging from the top and a sidechain lane showing what the compressor hears after SIDECHAIN HPF, and a gain reduction meter. The new KNEE knob sets the soft knee from 0 to 24 dB. It starts at 12 dB, the knee Deadline Pro always had, so existing sessions sound the same.
- **HEAT's display scrolls smoothly.** It no longer stutters once the screen fills, and the waveform is scaled to fill the display.
- **FOCUS curves drawn smoothly.**

## 0.9.3 · 27 Oct 2026
- **Pro Tools' automation highlights, redrawn.** In Pro Tools, a control enabled for automation now gets one thin rounded box round the whole control: the knob with its name and value, or the whole TRUE PEAK or BYPASS row. It is teal green while the track reads automation and red when the track is armed to write (touch or latch), instead of a heavy ring round the knob. Nothing moves or resizes, and other DAWs are unchanged.

## 0.9.2 · 25 Oct 2026
- **The changelog now ships inside the plug-in.** Every format (AU, VST3, AAX and the standalone app) carries this changelog as CHANGELOG.md, so you, or any tool you point at it, can read what changed without going online.

## 0.9.1 · 25 Oct 2026
- **Fixes the 0.9.0 update not replacing 1.0.x on Mac.** On a Mac that already had a 1.0.x version, the 0.9.0 installer reported success but left the older plug-ins in place, so the update was offered again and again. This version always replaces what is installed.

## 0.9.0 · 25 Oct 2026
- **New version numbers, on purpose.** Deadline Pro moves from 1.0.3 to 0.9.0. We decided it stays below 1.0 until its public launch, which will be 1.0. Nothing is lost or rolled back: 0.9.0 contains everything in 1.0.3 and more, and updates count up from here (0.9.1, 0.9.2 …).
- **Automation highlights you can trust.** In Pro Tools, Deadline Pro now shows only Pro Tools' own highlights, so an outline goes away the moment Pro Tools takes it away. Before, an outline could stay on until the plug-in was switched off and on again.
- **Automation outlines in other DAWs are now a choice.** Settings, DISPLAY, Show automation highlights puts a green outline on any control automation is moving, or has moved, in the session. It is off unless you turn it on, and a DAW re-sending a value it already has no longer lights anything, so nothing is outlined when a session opens.
- **Settings in six tabs.** AUDIO, METERS, DISPLAY, DEFAULTS, LIBRARY and ABOUT, each a short page in one window that stays the same size, as in Deadline Go and Mini. AUDIO shows the sample rate, buffer size, latency and channels your DAW is running Deadline Pro at. Every word in Settings is now at least 12 points.
- **"Reset all settings".** The button that returns Settings to their defaults is now called Reset all settings, under ABOUT.
- **What's new, from inside the plug-in.** A WHAT'S NEW button in Settings, ABOUT opens this page.
- **The build number, small and out of the way.** It sits under the version in ABOUT; click it to start an email to support that already says which version and build you have.
- **A quieter Field Guide search box.** The search text is centred, the box has a thin outline with small rounded corners, and the large focus ring is gone.
- **Field Guide brought up to date.** Settings, automation highlights and the meters are described as they are now.
- **WIDTH values hold still.** The figures in the WIDTH display no longer shift sideways as they change while you adjust it.

## 1.0.3 · 25 Oct 2026
- **IN and OUT headings above the meters.** Each level meter pair is now headed IN or OUT, on the same line as REDUCTION beside it, so every meter on the screen starts at the same height. REDUCTION's VIEW buttons move to a second row of their own, clear of its title.
- **L R and M S back in the pills.** With the headings naming each pair, the pill under each heading goes back to switching between left and right and mid and side.
- **Red only at 0.** The peak hold line and the peak figures turn red only at 0 dBFS or above, or above 0 dBTP with TRUE PEAK on, never at -0.1. They use each skin's own over colour, so they read correctly on skins whose red is closer to orange.
- **Choose how long the peak hold stays.** A new METERS section in Settings sets PEAK HOLD to INFINITE, 10 s, 5 s or 3 s. INFINITE is the default, so you can never miss an over. Clear a hold by double-clicking the meter or clicking its figures.
- **The classic meter colours are back, with a choice.** The meter fade is exactly as it was before 1.0.2. Settings > METERS > COLOURS sets where the colours start: CLASSIC (the default: yellow from -15 dB, amber from -9, red from -3), LATE (-6, -3, -1) or TOP (-3, -1.5, red only at 0).
- **Analyser tilt named after the standard it copies.** Settings > METERS > ANALYSER TILT offers CLARITY (the default, drawn as the TC Electronic Clarity M draws it, and the same picture as Deadline Go), RTA (pink noise reads flat, as on a one-third-octave analyser) and PRO-Q (FabFilter Pro-Q's 4.5 dB per octave). This replaces the TILT button in the analyser header. It changes only the drawing, never the sound.
- **The same metering across the range.** Peak hold, colours and red-at-0 now behave the same in Deadline Pro, Meters and Meters Pro.
- **"Atomic" in your DAW's plug-in list.** Deadline Pro is now listed under the vendor Atomic rather than Atomic Audio in Logic, Ableton Live, Pro Tools, Cubase, Studio One and Reaper. Your sessions, presets and settings recall exactly as before. Some DAWs move the plug-in to the new vendor folder only after a plug-in rescan.
- **A cleaner Field Guide search box.** The search box at the top of the Field Guide has a softer surround and centred text.
- **Field Guide updated.** The meters and Settings sections describe the new headings, peak hold, colour and tilt choices.

## 1.0.2 · 24 Oct 2026
- **Reduction peak hold fixed for COMP and CLIP.** The CMP and CLP lanes of the REDUCTION meter showed no peak hold when gain reduction rose smoothly. Every new maximum now moves the peak line and restarts its hold. All three lanes hold for one and a half seconds from the peak, then fall at 1.5 dB per second.
- **Calmer IN and OUT colours.** The level bars and the TRUE PK figures now warm up only near the top of the scale, so a master peaking at -3 dBTP no longer looks hot.
- **IN and OUT named on the meters.** Each meter pair's readout caption now says which pair it is, IN TRUE PK or OUT TRUE PK, and the tooltips explain both clicks.
- **Automation frames in every DAW.** Any control whose parameter is being moved by automation now gets a green outline, in every format. The outline is bright while automation moves it and stays dimmer once it has been automated, so after a pass you can see at a glance what is automated. It is cleared when you load a session, a preset or a snapshot, or press RESET. In Pro Tools, Pro Tools' own highlight colours still take priority.
- **Analyser tilt.** A TILT button in the spectrum analyser's header sets the slope the analyser is drawn with, from 0 to 6 dB per octave, default 4.5. It is saved with the session and changes only the drawing, never the sound.
- **Help link fixed.** The manual link in the plug-in pointed to a page that no longer exists. It now reads "Need help? Email info@atomic.audio".
- **Field Guide updated.** New sections cover automation frames and the analyser tilt, and the meters section is rewritten to match what the meters show.
- **Sound unchanged.** Your masters sound exactly as they did in 1.0.1.

## 1.0.1 · 24 Oct 2026
- **Automation highlights in Pro Tools.** Pro Tools' write, touch, latch and control-surface selection highlights now outline every control of the parameter: the knobs and switches on the main panel, the HQ chip, and the tiles and open panel in the CONTROL view. Nothing moves or resizes.
- **Gain reduction meter in Pro Tools.** Deadline Pro now sends its gain reduction, the compressor and limiter together, to Pro Tools' gain reduction meter in the mixer and on control surfaces.
- **EQ and dynamics curves in Pro Tools.** Pro Tools can now show Deadline Pro's EQ curve (LOW, MID and HIGH together), its dynamics curve and its gain reduction curve, in the insert and on control surfaces. The curve Pro Tools draws is the same curve Deadline Pro draws.
- **LOW and WIDTH tiles fixed.** In the CONTROL view, dragging the knobs on the LOW and WIDTH tiles moved different controls from the ones drawn. Each tile knob now moves the control it shows.
- **Panel RESET fixed on FOCUS and LIMITER.** RESET in the FOCUS and LIMITER panels did nothing visible. Every panel's RESET now puts its controls back, main knob included: FOCUS switches off, CLIP returns to zero and relinks its ceiling to the limiter, and LIMITER returns LEVEL, CEILING and RELEASE to their defaults, leaving TRUE PEAK and HQ as they are.
- **More of your edits can be undone.** Dragging a tile knob and double-clicking a panel knob to reset it are now each one undo step.
- **PEAK / RMS saved for each meter pair.** Choosing PEAK or RMS on one IN or OUT meter pair is now saved with the session, not just a change to both. Older sessions still load as they did.
- **Tooltip corrected.** The HOLD ALTERNATE READING tooltip now says 12 seconds, matching how long the reading actually holds.
- **Field Guide checked against the plug-in.** The built-in manual has been gone through panel by panel and corrected wherever it differed from the plug-in. It now has a full module reference for all ten CONTROL panels, every control's range and default, a tour of the screen, and sections on meters, routing, presets, reset and undo, Settings and mono tracks. Links that showed as raw text in the plug-in are gone.
- **Sound unchanged.** Your masters sound exactly as they did in 1.0.0.

## 1.0.0 · 22 Oct 2026
- **Deadline Pro, a complete mastering chain on one screen.** Tone, shape, dynamics, loudness and metering in a single plug-in, for AU, VST3 and AAX on Mac and Windows. Twist the macros for the big moves, then open any module to refine it.
- **Six macros.** HIGH for presence and air, MID for forwardness or less honk, LOW for weight and cleanup, HEAT for analogue saturation, FOCUS to make the bass mono and tight, and WIDTH for multiband stereo width with phase protection. Each is a small mastering studio in one knob, and each is completely flat at zero.
- **Gain and dynamics.** INPUT, a bus compressor for glue (COMP), an oversampled soft clipper (CLIP), and LEVEL and CEILING into the QUADRA limiting engine: clipper, catch limiter, look-ahead true-peak limiter and a final safety clamp.
- **TRUE PEAK, HQ and BYPASS.** TRUE PEAK holds the peaks between samples below your ceiling for streaming delivery. HQ lets the limiter look further ahead for gentler limiting, and can be switched mid-playback without a click. BYPASS crossfades smoothly and keeps the meters running.
- **The CONTROL view.** Every module opens into a panel with all its bands, frequencies and switches, and live graphs where it has them. Drag modules to reorder the chain, switch any of them off, and give each its own RESET, undo and redo.
- **A full loudness suite.** Pick STREAMING, LOUD, MAX or a CUSTOM target and read integrated and momentary LUFS, true peak and RMS against it, with the difference to your target always on screen.
- **Metering built for mastering.** IN and OUT level meters, a REDUCTION meter showing compressor, clipper and limiter side by side, LF WIDTH, correlation and width, and a 64-band spectrum analyser. The meters can pop out into a window of their own.
- **Presets and snapshots.** Fifteen factory presets, your own categories and favourites, and snapshots for comparing variations of one master.
- **Eight skins.** From Atomic, vivid blue and orange on true black, to Accessible. The sound is identical in every one.
- **The Field Guide built in.** The full manual, searchable, inside the plug-in.
- **Mono tracks.** Mono in to stereo out and mono in to mono out, where your host offers them.
- **The Atomic Arcade.** Eight games hidden behind the atom logo, for when the bounce is running.

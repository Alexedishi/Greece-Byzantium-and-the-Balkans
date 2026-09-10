##########################
# GATES OF THE BOSPHORUS #
##########################
Mod Version: 4.1.1
Game Version: 1.13.11 / 1.14-beta

Mod Author: Alexedishi
Contributors: LordR, Caelreader, CipherParadox
Special Thanks: RationaLess, Bahmut|Chris

####---------- Mod Dependencies ----------####
 - Community Mod Framework: https://steamcommunity.com/sharedfiles/filedetails/?id=3385002128

####---------- Version Compatibility ----------####
#		GotB Patch	....	Victoria 3 Patch
#		4.1.1		....	1.13.11
#		3.4.12		.... 	1.12.3
#		3.3.7		.... 	1.10.6 / 1.11.1
#		3.2.8		.... 	1.9.8
#		3.0.8		.... 	1.8.7
#		2.2.11		.... 	1.7.7
#		2.1.3		....	1.6.2
#		2.0.3		....	1.5.13
#		1.0.0		....	1.5.6


####---------- Current Content Scope ----------####
The following countries are in scope:
- GREFM: Greece (including Byzantium, the Ionian Islands, and Samos)
- BALKFM: Montenegro, Serbia, Bulgaria, Romania (and the Principalities), Bosnia, Albania
- TURKFM: Ottoman Empire (including Turkey)
- MGRBFM: Egypt, Tripolitania/Libya, Tunis, Fezzan
- HAYKFM: Kurdistan, Armenia

The following countries will eventually come into scope:
- BALKFM: Croatia, Slovenia
- LEVAFM: Syria, Lebanon, Palestine
- HAYKFM: Assyria

**Notes:
- Zionism, Pan-Arabism, & Iranian flavor are OUT OF SCOPE for this mod


####---------- Mod Structure and Organization ----------####
This mod is broadly divided into the following "modules" which can be identified by their prefixes:
grefm_: Contains content for Greece, Byzantium, and other Hellene, Rhomaios, and Urum countries
balkfm_: Contains content for the Southern Slav, Romanian, and Albanian countries
turkfm_: Contains content for the Ottoman Empire and the Turkish state
mgrbfm_: Contains content for the Ottoman subjects in Northern Africa
haykfm_: Contains content for the Kurdistan, Armenia, and Assyria states
levafm_: Contains content for the Levantine countries
eqfm_: Contains content for the Eastern Question and Expeditions; was formerly merged with turkfm

These are other prefixing conventions used in this mod:
*Generic and shared files are prefixed with "gbbf_"
*Script imported from Community Mod Framework is prefixed with "com_"
*Script imported from Morgenrote: Dawn of Flavor is prefixed with "mgr_" regardless of Morgenrote content pack origin
*Script imported from This Land is Mine is prefixed with "tlim_" regardless of TLIM content pack origin
*Script imported from "Awaken Thee Romanian" is prefixed with "atr_"

There are leftover references to older modules that you might find:
eocfm_: Once contained content for the Eastern Orthodox Church; has been superseded by Kingdom of God (kog_)
byzfm_: Once contained content for Byzantium; has been merged with grefm_
bulfm_: Once contained content for Bulgaria; expanded into balkfm_

**Notes:
-The current mod acronym is GotB; my common prefix is "gbbf_"; this was set before the name from GBBF to GotB and will not change
-The CMF trigger uses the much older "grefm_" generic acronym; this will not change


####---------- Naming Standards, Entry Prefixing, and Variable Names ----------####
- Entry names should be intuitive and readable, i.e. "grefm_bavarocracy_progress_var"

- The following entry prefix/suffix conventions should be following:
 Note: <module> should be replaced with according to which module the object belongs to, i.e. "grefm_bavarocracy_progressbar"
 -- Alerts:
 -- Amendments: amendment_gbbf_**
 -- Buildings: building_gbbf_**
 -- Characters: <module>_<TAG>_<last_name>_<first_name>
 -- Custom Loc: <module>_**_type
 -- Decisions: <module>_**_decision
 -- Decrees: decree_gbbf_**
 -- Diplo Actions: gbbf_**
 -- Diplo Plays: dp_gbbf_**
 -- Ideologies (Interest Group): ideology_gbbf_**
 -- Ideologies (Character): ideology_gbbf_**_leader
 -- Ideologies (Movement): ideology_gbbf_**_movement
 -- Journal Entries: je_<module>_**
 -- Journal Groups: je_group_gbbf_**
 -- Messages: <module>_**        <---- DO NOT prefix with "notification_"
 -- Political Movements: movement_gbbf_**
 -- Production Methods: pm_gbbf_**
 -- Production Method Groups: pmg_gbbf_**
 -- Script Values: <module>_**_value
 -- Scripted Buttons: <module>_**_button
 -- Scripted Effects: <module>_**_effect
 -- Scripted GUIs: <module>_**_sgui
 -- Scripted Progress Bar: <module>_**_progressbar
 -- Scripted Triggers: <module>_**_trigger
 -- State Traits: gbbf_state_trait_**
 -- Static Modifiers: modifier_<module>_**
 -- Subject Types: subject_type_gbbf_**
 -- Treaty Articles: gbbf_**
 -- Trigger Loc: <module>_**
 -- War Goals: gbbf_**

- Variables should be handled with the following conventions:
 -- Prefix with the module the variable belongs to (i.e. gbbf_, grefm_, balkfm_, etc)
 -- If the variable is used to store a value, suffix it with "_var"
 -- If the variable is used in a boolean trigger (has_variable), suffix it using any of the following:
    "_started", "_completed", "_failed", "_happened", "_cooldown", "_tracker", "_target"
 -- If a variable(s) is used only for a specific journal entry and its direct content, store the variable(s) in that journal
 -- Scripted effects are provided to aid in variable management

- Other conventions:
 -- Variable lists shoud be suffixed with "_list"
 -- Variable maps should be suffixed with "_varmap"

*Deviation from these systems is encouraged if it makes the object more readable or intuitive*


####---------- Planned Content/Reworks ----------####
----GREFM: Greek Content Module (GRE, ION, GRE_SAM, BYZ)
 - Increase number of factors that contribute to the Hellenism vs Romanism journal
 - Expansion to Theodoro Content

----BALKFM: Balkans Content Module (YUG, MON, SER, BUL, ROM, BOS, ALB, CRO. SLO)
 - MON: Content for the 1905 Constitution
 - MON: New journal "The Spirit of the Black Mountain": Lead Montenegro towards an independent identity; uses Morgenröte's writer mechanics
 - SER: Content for the Serb People's Movement
 - SER: Content for the Serbian Radical Constitution, Timok Rebellion, and May Coup
 - SER: Event chain representing the Krivošije uprising
 - BUL: New Naturalism journal for players using Morgenröte if Ferdinand is chosen as prince.
 - ROM: Rescript journal variables
 - BOS:Content for the Austrian Administration (modernization of Bosnia)
 - ALB: First Chapter of Albania content from the GEC into the early 1900s
 - CRO: Initial round of content
 - SLO: Initial round of content

----TURKFM: Ottoman Content Module (TUR, TURAN)
 - TUR:  Second Chapter of Ottoman Content extending from Abdulmecid to Abdulaziz

----MGRBFM: Maghrebi Content Module (EGY, TRI, TUN, FZN)
 - EGY:
 -- New journal "Egyptian Nationalism" representing the three-way struggle between the Arab, Misri, and Pharonic identities in Egypt
 - TRI:
 - TUN:
 - FZN:

----HAYKFM: Highlands Content Module (KUR, ARM, ASS)
 - KUR:
 - ARM:
 - ASS:

----LEVAFM: Levantine Content Module (SYR, LEB, PAL)
 - SYR:
 - LEB:
 - PAL:

----EQFM: Eastern Question & Expeditions Content Module
 - Balkans: Culture-specific movement radicalism effects in Balkan Separatism events
 - Balkans:Expand the Balkan Wars to cover the Macedonian Question
 - Pirates: Add more random events/interactions
 - Karadag: Consider more province-level mechanics
 - Desert: Add more random events
 - Highlands: New global journal entry "The Eastern Highlands" to represent the struggle between Russia and the Ottomans over their border

----Compatibility:
-- The "A National Language" journal now supports Morgenröte's writer mechanics (Greek tags)
-- New journal "A National Epic" journal; uses Morgenröte's writer mechanics (Montenegro)
-- New journal "The Naturalist King" - Partake in Ferdinand I's naturalist tendencies; uses Morgenröte's naturalist mechanics (Bulgaria)


####---------- Works Cited ----------####:
 Last Updated: 05.01.2024

 Greek History:
 1. Clogg, Richard (1979). A Short History of Modern Greece
 2. Clogg, Richard (2002). A Concise History of Greece
 3. Finlay, George (1877). A history of Greece, from its conquest by the Romans to the present time, B.C. 146 to A.D. 1864, Vol 7
 4. Gallant, Thomas (2016). Modern Greece: A Political and Social History from the War of Independence to the Present
 5. Gennadios, Ioannes (1870). Notes on the Recent Murders by Brigands in Greece
 6. Kairophylas, Kostas (1915). Eleftherios Venizelos, His Life and Work
 7. Christmas, Walter (1914). King George of Greece
 8. Avdela, Efi (2005). Engendering ‘Greekness’: Women's Emancipation and Irredentist Politics in Nineteenth-Century Greece
 9. Tsivanopoulos, Sōkrates (1864). Greece: Its Condition During the Reign of King Otho and Is Prospects under His Majesty George I.
 10. Petropulos, John A (1968). Politics and Statecraft in the Kingdom of Greece, 1833-1843

 Last Words by Koert Davidse: vimeo . com / 88034680


####---------- Planned Updates ----------####

--Update 4.2.0--
New Additions:
- ##New journal "The Nature of Yugoslavia" Promote a Centralized or Federalist approach to the Yugoslav state
- ##Added "Yugoslav Integralist" ideologies and movement representing the Integralist movement in Yugoslavia
- ##Fully implemented the Young Turks content with varying outcomes for the Republican movements in the Ottoman Empire
- ##New journal "The Foundation of the State" representing the multiple outcomes of Turkish identity after the failure of the Tanzimat
- ##Rebuilt "The Teachings of al-Sanusi" into a global journal with new mechanics, events, and modifiers

Fixes:
- ##Fixed several issues that could derail Greece's "Military League" journal


####---------- Published Updates ----------####

--Update 4.1.2--
Fixes:
- Fixed modifier_balkfm_yugoslavist_separatism also being applied to subjects of Yugoslav overlords
- Fixed turkfm_tanzimat.201 accidentally being linked to Young Turks weekly pulse
- Small fixes since CMF/GotB are out of sync during the 1.14 open beta


--Update 4.1.1--
Fixes:
- Fixed STATE_IONIAN_ISLANDS missing from several georegions


--Update 4.1.0--
New Additions:
- Reworked the "Throne of Thorns" journal:
  -- Scripting refactored to use variable maps & effects/triggers reviewed
  -- New custom journal widget showcasing the two dynastic leaders
  -- Fixed several cases where the Dynastic changeover events would not fire
  -- New character role "Pretender" for the non-ruling dynasts
- Completely rebuilt the "Powder Keg of Europe" journal & associated content:
  -- Scripting refactored to use variable maps & effects/triggers reviewed and improved in many cases
  -- Improved event scripting to better integrate with features from 1.10 and 1.13
  -- Integration with the new CMF Situations UI widget to better present the journal content
- Added a "Charioteer" trait in the event your redneck ruler joins a chariot races
- Replaced and updated several icons and gfx
- Added state trait and georegion for the Dinaric Alps

Balancing/Adjustments:
- Changed Abdulmecid's ideology from Reformer to Ottomanist
- Adjusted Yugoslav project so only Yugoslav countries are involved
- Political movements will no longer contribute negative progress to Ottoman identities
- Reduced grefm_megali_idea_complete_pan_greek_value to 14 from 15
- Reduced required Silk Planation levels in je_grefm_constantinople to 12 from 20
- Ludwig von Armansperg is now marked as married
- Completed Tanzimat agendas now counts towards Reformist progress
- modifier_turkfm_reorganizing_spirit now decays
- Mehmed Emin Rauf Pasha now has a reformer ideology
- Koca Husrev Mehmed Pasha now has the Ottomanist ideology

Fixes:
- Added missing localization for Metaxism content
- Fixed broken effects in the Triumph buttons
- Moved grefm_byzantium.020's scripting into monthly state pulse
- Fixed Amalia of Oldenburg being a transgender icon :sadge:
- balkfm_croatia.300 will no longer try to add a journal that already exists
- Added scope assertions to the options in balkfm_romania.004/5
- Fixed several issues with the Black Mountain buttons should MON get obliterated early
- Political movements will no longer contribute negative progress to Ottoman identities
- Fixed on_action issue that could cause modifier_balkfm_yugoslavist_separatism to be applied multiple times
- Added handling for head-taking modifiers in the event MON or TUR are dead
- Added effect to replace Turkish homelands with Ottoman homelands in the "Ottoman Motherland" event
- Added Kosovo to Greek Heartlands and Byzantine Empire georegions
- Fixed incorrect variable scope for je_grefm_the_dedilomeni_principle progress bar
- Fixed a collision in history files resulted in incorrect ideologies
- Several small localization mistakes


--Update 4.0.8--
Fixes:
- Fixed incorrectly gated effects in eqfm_balkans.008/9


--Update 4.0.7--
Fixes:
- Fixed an issue with the Tanzimat "Organize the Bureaucracy" agenda not correctly displaying its requirements
- Fixed several mismatched modifiers and variables in the "An Ottoman Legacy" journal
- Replaced country_law_enactment_time_mult with country_law_enactment_speed_mult


--Update 4.0.6--
New Additions:
- Added a game rule to reduce the number of starting Kurdish tags
- Added Rhomaios homelands in mainland Greece

Fixes:
- Split Kurdistan history files from main history files
- Over a hundred small script and loc fixes thanks to Tiger
- Fixed some mixed up effect scopes for AI actions
- Updated state region name effects for 1.13 strategic regions
- Fixed the on_actions still treating the escalation/deescalation variables as global scope instead of journal scope
- Removed content relating to the Exarchate of Bulgaria (this has been disabled for over a year; will find a home in KoG)
- Fixed the DLC Bavarocracy variant being excluded from the Constitutionalist ideology logic
- Added a trigger to cover Eastern Thrace being lost to a revolt (14 Regions journal)
- Fixed grefm_greece.031 not saving the ruler scope
- Fixed trigger issue preventing the Megali Idea from completing
- Fixed regional control triggers for The Sick Man of Europe not evaluating correctly
- Removed deprecated event balkfm_bulgaria.160
- Fixed the option effects being reversed in eqfm_balkans.008/9


--Update 4.0.5--
Fixes:
- Fixed triggers for electoral confidence being multiplied by 100


--Update 4.0.4--
Fixes:
- Cleaned up the activation script and initial events for je_grefm_venizelism
- Removed grefm_greece.046
- Added safety trigger to keep je_grefm_venizelism from closing early


--Update 4.0.3--
Fixes:
- Reduced some error spam for missing modifiers
- Added more missing loc for several Egypt events

Notes:
- Rekeyed geographic_region_middle_east_highlands to geographic_region_armenian_highlands


--Update 4.0.2--
New Additions:
- Added a game rule to change the Ottoman map color to red

Fixes:
- balkfm_yugoslavia.002 will no longer cancel if the country has nationalism researched
- Fixed turkfm_sick_man.019 not adding the Tanzimat reform agendas
- mgrbfm_egypt.005 now remembers to save Said from sinking into the void
- Added missing loc for several Egypt events


--Update 4.0.1--
Balancing/Adjustments:
- Reworked modifiers for Greek language outcomes
- Blocked Abdulmecid getting put into a regency if he's still a minor

Fixes:
- Added missing name loc for Djemal
- Fixed turkfm_sick_man.019 making Abdulmecid ruler just to immediately yeet him out the window


--Update 4.0.0-- **Major Update**
New Additions (grefm):
- New journal entry "Metaxism" representing the emergence of anti-monarchism and authoritarianism in Greece
- Added Metaxism ideology for Greece's version of Fascist-related thought
- Added Greece as a formable country
- Added several geographic regions to support Megali Idea content
- Ludwig von Armansperg starts as the ruler of Greece with Otto in a regency
- Added additional dynamic hub names for Constantinople

New Additions (balkfm):
- Rebuilt "Nacertanije" into a global journal "The Yugoslav Project"
- Added scripted buttons to "The Yugoslav Project" to annex Yugoslav countries in a manner similar to Greek annexations
- Added five new dynamic country names for the Serbian Empire tag
- Added Pero Petrović and Stanko Petrović as starting politicians for MON
- Added Anto Daković, Ilarion Roganović, Mitrofan Ban, and Jelena Vicković as historical characters for MON
- MON can pick up Novica Cerovic as a general and politician
- Added Smail Aga and Hasan Aga as starting characters for BOS
- BOS starts with a claim on Montenegro

New Additions (turkfm):
- New journal "The Young Turks" representing an alternative fail state to the Tanzimat
- New journal "Restoring Anadolu" in the event post-Ottoman TUR does not control all of Anatolia
- New journal chain "The Rampaging Wolf" for post-Ottoman Turkish expansion
- New journal "The Armenian Expulsions"
- New building "Avret Pazarları" (Slave Market of Constantinople) with scripting for the Carcassian slave trade
- New amendments "Çiftlik" for Land Reform and "Esir Pazari" for Slavery
- New "Young Turks" political movement with "İttihadism" and "Kemalism" ideologies
- Added a new formable tag "Turan"

New Additions (mgrbfm):
- New journal "The Ambitions of Muhammad 'Ali" representing the expansionist goals of Muhammad Ali
- New journal "The Dawn of the New Egypt" representing the modernization goals of Muhammad Ali
- New journal "Taming the Nile" representing the long-winded struggle to control the waters of the Nile
- New journal chain "The Egyptian Caliphate" representing the idea of an Egyptian Empire
- New journal "The Subjugation of Sudan" for Ali Pasha's efforts to secure his hold on Sudan
- New journal "The Ethiopian Frontier" for the Egyptian invasion of Ethiopia
- New journal "The Arabian Gulf" for the Egyptian attempt to control the Red Sea
- New journal "Securing Fezzan" for Fezzan
- Added several historical rulers for EGY
- Added flags to both TRI and LBY
- Decentralized a portion of the Egyptian desert
- Added Copt culture and converted all Misri Oriental Orthodox pops to it
- Added "Nile Barrage" government building as a potential in Lower Nile states
- Added "Sharan Trade Networks" government building to some Saharan states
- Added "Esparto Plantations" agricultural building to Libya and Tunisia
- Moved Joseph Anthelme Sève to Armed Forces leader for EGY
- Added Hayreddin Pasha as a starting character for TUN

New Additions (haykfm):
- Researched and added more historical characters to the Kurdish emirates
- Armenia is selectable from the "Sick Man of Europe" objective and spawns as the Eyālet-i Erżurūm

New Additions (eqfm):
- Rebuilt the "Black Mountain" journal into a global journal to merge and expand on content for Ali Pasha Rizvanbegović
- FZN now has access to the "Securing the Desert" journal entry
- Improved localization with additional tooltips, explanations, and text icons

Mod Integrations:
- Integrated the "Awaken Thee, Romanian!" mod with permission:
-- Added a game rule to change Romania's color to its cream color from Victoria 2
-- Added multiple flags for Moldavia and Wallachia
-- Added DNA for Alexandru Ioan Cuza, Alexandru Ghica, and Carol and Ferdinand Hohenzollern

V3 Patch 1.13 Related Changes:
- Replaced most scopes to sr: with geographic region triggers
- Updated journals to comply with new pinning params and widget injection
- History-generated haracters now have defined home states
- Updated DLC icon
- Removed usage of Memento Mori variable

Compatibility:
- GotB now has built in compatibility with Morgenröte: Dawn of Flavor:
-- The "Greek Cultural Roots" journal now supports Morgenröte's archaeology mechanics (Greek tags)
-- The "Venizelism" journal now supports Morgenröte's artistic tradition mechanics (Greece)
-- The "14 Regions of Constantinople" now supports Morgenröte's Architect mechanics (Byzantium)

Balancing/Adjustments:
- Updated several event videos to use IP3/IP4 gfx
- Merged all Ottoman Legacy sub-journals into a singular journal
- Merged all Venizelism sub-journals into the primary journal
- Merged all Tanzimat Reform sub-journals into a singular journal
- "Megali Idea" and "Sick Man of Europe" journal entries now use geographic regions instead of strategic regions
- Replaced IP3's "Serbia and Montenegro" journal for better integration; this remains DLC-locked
- Cloned IP3's mon_state_formation.5 to balkfm_yugoslavia.007 for better integration; this remains DLC-locked
- je_balkfm_mon_military_reform now requires 10 military units and an Arms Industries building
- Refactored multiple Romanian characters to use templates
- Both TRI's and FZN's starting journals will activate after their war is resolved
- Reworked wargoal enforcement detection for Balkan Situation escalation/deescalation
- Merged je_eqfm_senusiyya_main and je_eqfm_senusiyya_sub into je_eqfm_senusiyya
- Added 6 Sulfur resources to Kosovo
- Added Silk Plantation resource to Bosnia
- Added 4 Sulfur resources to East Aegean Islands
- Added potential triggers to several formable tags
- Byzantine Restoration journals now use geographic regions instead of strategic regions in most cases
- Ottomans now start with Migration Controls enacted
- "Dedilomeni Principle" journal now accounts for electoral confidence
- Reworked eqfm_balkans.008/009 to have discrete effects
- Implemented several scripted effects and script values for better value/var management
- Refactored most instances of create_character to use templates
- MON and BOS start with a bilateral truce
- Adjusted modifier_grefm_armansperg_regency to match Landowners regency modifier
- "Westernized Thought" modifier changed to be a decaying modifier

Fixes:
- Large localization pass to fix typos, formatting, puncutation, etc.
- Reworked script handling the creation and tracking of Serbian dynastic heads
- Updated Balkan situation localization to better indicate sources of escalation/descalation
- Fixed a case where subjects could get stuck as Eyalets
- Building the Biljarda is now mandatory for the "Prince-Bishopric" journal if IP3 is active
- Declaring the Principality of Montenegro is now mandatory if IP3 is active
- Fixed a situation where "Change of Tack" journal's fail conditions could be true when the journal activates
- Enabled two monarchy-specific flags for MON
- je_balkfm_cultural_identity now checks for je_balkfm_national_awakening instead of nationalism in its fail trigger
- Completing je_balkfm_national_awakening no longer changes Bosnia's state religion to Orthodox
- Fixed error spam from balkfm_validate_serbian_characters scripted effect
- Fixed several instances of age instead of birth_date
- Fixed several outdated character template calls
- Fixed several improper/non-flowing modifier type placements
- Added missing custom loc for byzantium.023
- Fixed dozens of small localization typos and errors
- Improved the scripting of the Chariot Race events
- Montenegrin journals that involve AUS now check for it to exist first
- Changed all instances of set_relations in history to change_relations
- Improved scripting for the Megali Idea completion triggers
- Fixed several issues in the completion tooltips for the Megali Idea
- Fixed a duplicated trigger in the "Dedilomeni Principle" journal
- Refactored implementation of quotation marks in localization
- Refactored all instances of pirates_expedition_ to adriatic_expedition_
- Refactored all instances of black_mountain and the_black_mountain to karadag
- Refactored geographic_region_balkan_situation to geographic_region_rumelia
- Fixed confusing localization in Greek king election buttons
- Updated progress bars to use CMF's colored progress bars
- Fixed an effect sequencing mistake that would jam the Piracy expedition progress
- Fixed several scoping issues in Piracy events
- Fixed an issue were several Piracy events could fire despite there being no expedition
- Fixed eqfm_pirates.030 being very eager to let you know that pirates have been spotted
- Fixed a scoping issue in the loc for balkfm_croatia.201
- Refactored all character template names to shorten key length
- Pirate raid events will only occur if the involved country has a coastal state
- "Brigands Raid Again" event will only occur if the affected country has more than one state
- "Canonize Ancestor" scripted button is now correctly visible in je_balkfm_mon_prince_bishopric
- Added missing effects and localization to grefm_greece.047/048
- Graia now has the correct map color instead of neon pink
- Fixed a trigger fail in the Megali Idea journal that could brick the journal
- The Mehmed II death event no longer domes Abdulmecid instead
- Reworked the trigger block for eqfm_pirates.015
- eqfm_karadag.022/023 now use the correct event icon
- Fixed broken scopes in eqfm_balkans.103 and .124

Notes:
- [!!] The "Young Turks," "Amrenian Expulsions, and "Metaxism" journals are in a beta state, please report issues to the Steam page/Discord
- The journal entry "The Teachings of al-Sanusi" has been temporarily disabled; this needs a few more weeks of work to be ready
- Egypt and Fezzan are now in scope- Arabian Peninsular, Pan-Arab, and Muslim content remain *out of scope*
- Libyan and Tunisian content split from "turkfm" into "mgrbfm"


--Update 3.4.12--
Fixes:
- BOS and TUR now start with Debt Slavery
- Added scripted button to form BYZ to the Megali Idea Journal


--Update 3.4.11--
Fixes:
- Pirates completion event now shows the country that captured the Pirate Leader instead of a broken scope
- Added some extra script to regenerate the Serbian dynastic ruler in the event the templated character gets clipped


--Update 3.4.10
Balancing/Adjustments:
- Tanzimat Army journal now cares about all army units for completion
- Tanzimat Agriculture journal now boosts anti-Traditionalism movements on completion
- Tanzimat Economy now creates and/or boosts Land Reform movements on completion
- Tanzimat Education provides an option of two modifiers
- Tanzimat modifiers are now hosted within their respective journals after starting the Tanzimat
- Reduced intensity of tuberculosis custom trait (to -50% from -5000%)
- Added an option to turkfm_sick_man.019 to immediately start the Tanzimat instead of clicking the journal button


--Update 3.4.9--
New Additions:
- Added Greek-language dynamic state and hub names to the Balkans, Anatolia, Levant, and Egypt state regions
- Added (1) Base, (3) Monarchy, (1) Theocracy, and (1) Socialist flags to Montenegro
- Added (4) Monarchy, (1) Theocracy, and (1) Socialist flags to Serbia

Balancing/Adjustments:
- Serbian Empire tag now uses Serbia's flags
- Removed Greek Formables game rule

Fixes:
- Removed broken tooltip from Greek Empire tag name


--Update 3.4.8--
Fixes:
- Fixed Piracy expedition journal closing prematurely
- Banished the phantom Russian Kars state to the aether
- Adjusted Balkan involvement triggers so countries don't become uninvolved by moving their capital to Constantinople
- Added missing event option names in several Greek Empire formation events


--Update 3.4.7--
Balancing/Adjustments:
- Ottoman Palaces will now deactivate if controlled by a country other than TUR
- Limited notification spam for the Balkans Situation if players are uninvolved
- The Ottomans now start with a Military Formation deployed to the front with Soran
- Libya is Exempt from Military Service at game start

Other:
- Updated has_amendment triggers to match new functionality


--Update 3.4.6--
Fixes:
- Fixed native Greek rulers not being created as rulers


--Update 3.4.5--
New Additions:
- Added two new Distribution of Power laws for the Ottomans
- Added one new Bureaucracy law for the Ottomans
- The Ottomans now start with the Imperial Divan and Scribal Bureaucrats laws active

Balancing/Adjustments:
- The Ottoman Intelligentsia now start in government without causing legitimacy problems, no longer start with the Anti-Slaver ideology, & now gain the liberal ideology via event
- Added a decaying modifier to the Ottomans representing the ongoing military disarray from the Auspicious Incident

Other:
- Added entry modes to custom cultures to improve compatibility
- Added a proper Ottomanist IG ideology


--Update 3.4.4--
New Additions:
- Added government-dependent flags for the BYZ tag for Authoritarian Democracies, Technocracies, and Theocracies.

Balancing/Adjustments:
- Moderated some stances for the Scribalistic and Ottomanist ideologies

Other:
- Cloned localization entries to other languages (see Steam page for known translations)


--Update 3.4.3--
Fixes:
- Blocked regencies via CMF as needed
- Fixed an issue where balkfm_romania.602 will have no options
- Disabled the base game transfer_ionian_islands_decision


--Update 3.4.2--
New Additions:
- Added over 20 Dynasty-dependent flags for the BYZ tag
- Added Rhomaios pops in Syria and Egypt

Balancing/Adjustments:
- Made the triggers in the "Seek Royal Marriage" scripted button less esoteric
- Nikitaras now has the Constitutionalist ideology and will join as an agitator is there is an open slot available
- Reduced the amount of Infamy gained just for choosing to pursue the maximalist Megali Idea

Fixes:
- Fixed a missing change_tag effect that prevented AST from completing the Megali Idea
- Fixed a corner case where players could lock themselves out of deploying Adriatic Expeditions


--Update 3.4.1--
Fixes:
- Fixed bad effect sequencing in balkfm_serbia.007 that could cause the base game regency mechanics to break the Dynasty Rivalry script


--Update 3.4.0--
New Additions:
- Added a scripted button for Otto's marriage to Amalia for IP3 users
- Reworked the "Dedilomeni Principle" journal to have a clear goal and stronger effects
- "The Military League" journal has been completely reworked due to the coup changes and is no longer gated behind VotP
- Added DNA for Nikolas Zorbas courtesy of LordR
- Venizelos events have been reworked to provide better integration with the Megali Idea journal
- Added a "Venizelist" movement that will spawn when Venizelos becomes active
- Reworked "The Defenders of the Constitution" journal to have discrete fail conditions instead of a short time limit
- Added the Simić brothers as characters for Serbia
- Added several missed IP3 characters to Greece & Serbia
- "The Powder Keg of Europe" and "The Pirates of the Adriatic" journals have been reworked to function as global journal entries
- Added a new Ottoman law amendment, "Elifbâ," to the education system lawgroup
- Added Aromanian and Romani cultures & pops across the Balkans
- Added custom geographic regions for Aegyptus and the Levant

Other:
- Updated script to comply with INJECT/REPLACE entry modes
- Added a popup that will inform users to install CMF if it is not present
- Content for Armenia, Kurdistan, and the Assyrians has been moved into its own content module, "haykfm"
- Updated several building keys to match 1.12 keys
- je_eqfm_balkan_situation journal renamed to "The Powder Keg of Europe"
- Merged je_eqfm_eastern_question, je_eqfm_balkan_situation_crisis, & je_eqfm_balkan_situation_riots into je_eqfm_balkan_situation
- Replaced existing geography triggers with geographic regions
- Updated the Senussi journal script math for the addition of Zuwayya
- Removed TRI_KUF tag & associated history effects


--Update 3.3.7--
Balancing/Adjustments:
- Adjusted the support threshold for balkfm_serbia.007 triggering down to 20 from 50
- Cementing Dynastic Succession for Serbia now requires having at least 50 legitimacy

Fixes:
- Fixed je_balkfm_state_reform checking for pm_simple_farming instead of pm_simple_organization


--Update 3.3.6--
Fixes:
- Fixed a broken scripted trigger
- Fixed a variable mismatch in je_balkfm_bos_ali_pasha


--Update 3.3.5--
Fixes:
- Fixed broken flag and name triggers for BYZ
- Greek country annexation variables will now increment monthly
- The base game Megali Idea journal is no longer visible
- Fixed all Italian reconquest event variants firing for the player regardless of primary culture
- Turkish palace decisions have been limited to the Ottomans
- Slightly adjusted the triggers for the Megali Idea and Byzantine Restoration for better functionality
- Fixed the excavation completion event spamming itself if the player doesn't knowledge it right away
- Fixed an oversight with the Triumph buttons
- Fixed an oversight where you could start an excavation multiple times and thus lock yourself out of progress
- Removed duplicated modifier in the Byzantine Restoration journal
- Fixed an oversight that allowed the Greek Cultural Roots journal to close pre-maturely


--Update 3.3.4--
New Additions:
- Added a diplomatic play to annex eyalet subjects
- Added ending bonuses to Ali Pasha content

Fixes:
- Silistra and Yanya are now created as eyalet subjects
- Reviewed and adjusted triggers for several non-political Greek historical events
- Ali Pasha event chain no longer ends prematurely

Other:
- Added more state region based scripted triggers


--Update 3.3.3--
Fixes:
- Added "People of the Book" law to Yanya and Hersek
- Added Kosovo as a requirement to form several empires in the Balkans


--Update 3.3.2--
Balancing/Adjustments:
- Controlling all of Western & Eastern Serbia is required to activate the "Serbian Heartlands" journals

Fixes:
- Added some missing localization for Turkish palace decisions
- Added Kosovo clam to balkfm_serbia.200


--Update 3.3.1--
Fixes:
- Added diplomatic action to annex Eyalet subjects
- Fixed event spam when the expedition leader dies in the Adriatic and Black Mountain expeditions
- Added missing content to turkfm_sick_man.009


--Update 3.3.0--
**NOTE: Any DLC-specific content will NOT be provided by GotB unless you own National Awakening (IP3)**

IP3-specific Integrations:
- Merged the IP3 and GotB Bavarocracy journals; mechanics will vary depending on whether the player has IP3 installed
- Added new journal entry "The Black Mountain" to MON & TUR; this journal integrates the Montenegrin raiding journal from IP3
- Reworked GotB's "National Awakening" into a prelude to IP3's "National Awakenings" journal
- Integrated the "Forming Yugoslavia" content into Nacerantije
- Integrated the Russian aid mechanics into "The Prince-Bishropic"
- "Negotiate Adriatic Access" button provides different triggers depending on whether the player has IP3 installed
- The Dynastic Rivalry journal will take on a different name depending on whether the player has IP3 installed
- Integrated the scripted buttons from Throne of Thorns into the Dynastic Rivalry journal
- Merged GotB's "Military Modernization" journal into the IP3 "Prussia of the Balkans" journal
- The Balkan Situation Crisis phase will unlock for IP3 owners and integrates content from the Great Eastern Crisis journal

1.10 General Integrations:
- Integrated the 1.10 Megali Idea objective variations
- Failing the "Sick Man of Europe" or "Reorganization of the State" GotB journals will trigger the "Grand Collapse" journal from 1.10

New Additions:
- Refactored the "Eastern Question" to use the new CMF Situations Framework
- Added support for CMF's DLC Icons in journal entries
- GotB now enables the vanilla Olympics decision for any country that has the Hellene primary culture and controls Attica
- Scripted buttons for annexations have been added to Megali Idea variants with decision fallbacks
- Added new Raiding Expedition events and mechanics to "The Black Mountain"
- The Dynastic Rivalry journal will show the leaders of each house in the journal entry
- Rebuilt the "Reorganization of the State" journal and added a new "Imperial Identity" system; success in the Tanzimat will allow players to enforce an Islamist identity for the Empire or take on a new "Ottoman" primary culture
- Added new diplomatic actions for subjects to have more participation in the Balkan Situation
- Added new journal entry "The Young Ottomans" to TUR which can culminate in the 1876 Coup
- Added lobby flavor text to relevant journals
- Added new treaty article to Cease Raiding for Montenegro/Turkey
- Added new treaty article to Return Kotor for Austria/Montenegro

Balancing/Adjustments:
- Reduced duration of excavations for the "Greek Cultural Roots" journal
- Hersek is created as unrecognized BOS tag
- Yanya is created as unrecognized ALB tag
- Silistra is created as unrecognized BUL tag
- "Cement Dynastic Succession" button now requires having the matching consul
- Consul triggers now check for AUS/RUS to exist before evaluating
- Adjusted the Regulamentul Organic journal to account for the new Regulamentul law
- Rise of Nationalism journal now checks for acceptance levels
- All countries now receive the Eastern Question journal; only involved countries will get the starter event
- Removed some scripting and loc from the Rise of Nationalism journal since it is partially superseded by the Eastern Question
- Removed custom Millet System laws (superseded by IP3)
- Reduced initial Balkan Escalation progress and intensity of Unrest / Hostility modifiers
- Reworked and simplified the Bulgarian Irredentism journals
- Adjusted the Bulgarian Irredentism journals to play nice with the reworked Nacertanije
- Removed several custom journal entry groups
- Reviewed and cleaned up the scripting in all custom journal entries
- Adjusted the state names used for the Libyan Desert / Libya
- Added a new state name for the Tubu-controlled desert

Fixes:
- Several localization fixes
- Removed the Accelerate/Mitigate Tensions diplo actions and replaced them with scripted buttons for performance reasons
- Bulgarian National Awakening events will now only fire for Bulgaria
- The Senussi journal now removes its modifier on completion
- "Embrace Senussi" button is now possible for non-TRI tags
- Fixed several small bugs that could stop Piracy progression

Notes:
- **ALL ORTHODOXY CONTENT HAS BEEN REMOVED FROM GOTB** This is in preparation for the release of the Kingdom of God mod
- The following GotB journals and their associated content have been gated behind IP3: "Nacertanije" and "Balkan National Awakening" as there is no reasonable avenue for deconfliction
- Updated screenshots and DLC icon on the workshop


--Update 3.2.9--
Notes:
- Technical update to change thumbnail


--Update 3.2.8--
Fixes:
- Reworked triggers for Accelerating/Mitigating Balkan Tensions diplo actions


--Update 3.2.7--
New Additions:
- Added Jelali, Shakak, and Ardalan as tribal subjects of Iran

Balancing/Adjustments:
- Removed scripted rebellions for Yugoslav countries


--Update 3.2.6--
New Additions:
- Added five Kurdish Emirates/Principalities with Kurdistan now available as a formable
- Added two journals for the Kurdish Emirates
- Added Eyālet-i Kurdistan as a formable by journal entry
- Add a new Sick Man journal "The Kurdish Frontier"

Fixes:
- Fixed several missing/broken modifier multipliers


--Update 3.2.5--
Balancing/Adjustments:
- Rescripted several Romanian journal script values and their associated variables/effects
- Expanded localization entries for Romanian content
- Added scripted progress bars to some Romanian journals

Fixes:
- Fixed error spam from turkfm_riot_progress_value in certain contexts
- Yanya is now correctly spawned as an Ottoman puppet
- Completing the Brigandage journal now counts towards the Regulamentul completion


--Update 3.2.4--
New Additions:
- Added a game rule to remove culture limitations on Greek formables (are you happy now, you filthy casuals)
- Added a game rule to spawn Yanya and Silistra at game start if playing as the Ottomans

Balancing/Adjustments:
- Rescripted the Senusiyya journal, events, and effects
- Rescripted/rebalanced the script effects and values for the Bavarocracy
- Added Violent Suppression Decree as a factor in the Nationalist Insurrection journal
- Improved script value breakdown to show which countries are accelerating/decelerating tensions
- Expanded several localization entries for the Bavarocracy

Fixes:
- Added missing opinion flag for the Senusiyya journal
- Adjusted triggers for Orthodox decrees
- Fixed a mistake in calculating Accelerate/Decelerate Tensions script value
- Fixed math error in the Dynastic Rivalry journal


--Update 3.2.3--
Fixes:
- Fixed triggers for adding Ottoman Legacy journals
- Bavarocracy progress value now checks for the Legacy journals instead of completion variables

--Update 3.2.2--
Fixes:
- Fixed "Legacy of Rhomania" event repeatedly firing

--Update 3.2.1--
New Additions:
- Added game rule to reduce Ottoman starting radicalism for the first six months
- Added starting cultural minority movements to the Ottomans for the Hellene, Serb, and Bulgarian cultures
- Added phase-specific modifiers to cultural minority movements

Balancing/Adjustments:
- Gated Ottoman Legacies behind starting laws
- Added ruler popularity to Dynasty Rivalry progress values
- Added Serbian consulship mechanic to the Dynasty Rivalry journal
- Removed Millet System social hierarchy
- Added acceptance modifiers to the Millet System laws
- Completely re-scripted the Balkan Nationalism journal to interact with political movement mechanics
- Removed bespoke country secession scripting and reworked the Race Riot scripting
- Reduced needed number of pirate expeditions to 4 from 5
- Reduced maximum peril limit for Pirate Expeditions down to 5 from 8
- Split The Rise of Nationalism progressbar into two progressbars with script value breakdowns
- Added several details to Ottoman journals to expose underlying values/variables
- Rebalanced Tanzimat progress factors
- Removed landowners from the starting Ottoman government

Fixes:
- Added missing opinion flags for Pirates of the Adriatic
- Fixed trigger issue in gbbf_balkans_culture_trigger
- Fixed weights for Piracy chase events
- Fixed missing localization in the Balkan situation journal
- Added missing localization in turkfm_balkan_situation.133
- Fixed incorrect values for clamping expedition variables
- Added missing clamp effect in excavation scripting
- Fixed a broken effect for Tanzimat progress bar

Notes:
- Refactored turkfm_separatism_phase_var into turkfm_balkan_situation_phase_var


--Update 3.2.0--
Balancing/Adjustments:
- Event & localization files have been split and refactored; several content files have also been split into sub-files
- Dynastic Rivalry journal has been re-scripted to improve its reliability
- Dynastic Rivalry progress factors have been rebalanced
- Peles Castle is now buildable like any other building and its journal mechanics have been removed

Fixes:
- Fixed several missing variables for Tunis
- Small fixes and updates to localization entries

Notes:
- ALL EVENT IDS HAVE BEEN REFACTORED. The localization entries themselves remain unchanged.


--Update.3.1.6--
Fixes:
- Added backup triggers to balkfm_cement_monarchy_button

--Update 3.1.5--
New Additions:
- Added a tag for Republika Srpska
- Republika Srpska and Hersek are now releasable

Fixes:
- Yanya now has the Albanian culture (instead of Bosniak)
- Removed Turkish culture from Hersek
- Removed illegal French PB Embassy from Greece at game start
- Adjusted scripting in dynastic takeover events to avoid event spam
- Urum & Rhomaios pops are now correctly present in Theodoro
- Re-exported several gfx files to fix resolution issues

Note:
- The sidebar button disappearing has been partially fixed. This is an engine issue with scripted widgets, Paradox is investigating.

--Update 3.1.4--
Fixes:
- Re-exported all gfx to use correct compression

--Update 3.1.3--
Fixes:
- Fixed missing scope in balkfm.210
- Removed incorrectly sequenced effect in je_turkfm_separatism_riots
- Fixed incorrect scopes in autonomy on_actions
- Fixed character ideology trigger blocks
- Fixed leftover instances of modifiers still using months in conjunction with modifier time defines

--Update 3.1.2--
Balancing/Adjustments:
- Added a new flags for Graia if the capital is in Thessaly or Northern/Western Thrace

--Update 3.1.1--
Balancing/Adjustments:
- Added power bloc embassies to the Treaty of London articles
- Added a new flag for Graia if the capital is in Albania

Fixes:
- Replaced instances of months with days in events that use the modifier_time values
- Removed some redundant files

--Update 3.1.0--
New Additions:
- Added new ideology icons courtesy of Caelreader
- Orthodoxy window can now be opened using the alerts

Balancing/Adjustments:
- The "National Awakening" journal will now boost progress in the "Earning Recognition" journal
- Added Liberty Desire reduction to Rumelia if they are a subject of Bulgaria
- Added progress bars to Battenburg Monarchy journal
- Updated ai_change blocks to use script math
- Replaced has_diplomatic_pact with any_scope_treaty where appropriate
- Removed Turkish building rework
- Moved large amounts of history effects from GLOBAL into the appropriate history files
- Adjusted how vanilla journals and event are overridden
- Replaced instances of months with days for modifier_time defines
- Moved gbbf_game_start_effect from the objectives on_start to on_game_started_after_lobby
- Updated any modifiers impacted by CoC/1.9
- Limited the Piracy JE strictly to countries on the Adriatic

Fixes:
- Fixed typo in Gennaios Kolokotronis' birthdate
- Cleaned up eocfm alerts script
- Fixed broken Patriarch initialization effect
- Fixed turkfm_millet_abolished_enact_effect never actually existing to be executed
- Fixed several typos in localization
- Fixed a situation where the Convoke Council button could be permanently enabled
- Fixed bad trigger preventing countries from being turned into their recognized counterparts after completing the National Awakening journals
- Belonging to Russia's Power Bloc now provides support for Alexander Battenburg
- Tuned up Balkan Rebellion creation script
- Graia can now access the "14 Regions of Constantinople" journal

################################################################################

--Update 3.0.8--
Fixes:
- Fixed typo preventing the Graia reconquest journal from opening

--Update 3.0.7--
Fixes:
- Fixed missing icons in certain modifiers

--Update 3.0.6--
New Additions:
- Added reconquest journal entry variants and events for Graia
- Added "Thourios" sfx to grefm.300

Fixes:
- Moved "Epitaph of Seikilos" sfx to grefm.275
- Fixed "Support Hellene Gunnrunners" button never becoming visible
- Removed redundant modifier loc in grefm
- Lots of script cleanup thanks to moving to IntelliJ
- Removed /dlc directory; this is unneeded
- Replaced nottomans_country_has_greek_culture_trigger with gbbf_country_has_greek_culture_trigger
- Removed several dummy events
- Fixed an OLD issue in grefm.004

--Update 3.0.5--
Technical:
- Added an automated update release workflow courtesy of Bahmut

--Update 3.0.4--
New Additions:
- Added tablemap coin graphic courtesy of LordR
- Added a new Empire-tier country tag "Graia" to represent the Hydrid Greek identity Empire

Balancing/Adjustments:
- Secure the Countryside journal now only checks for states in the Balkans & Danubia
- Returned je_turkfm_separatism_main's completion requirement to having Multiculturalism enacted

Fixes:
- Fixed issue in the metadata file
- Fixed countries having no laws in Hellene revolt countries
- Added missing localization in turkfm.254
- Fixed localization function error in several strings
- Removed states history file; this was included in error
- Fixed small localization typo in one of the notifications
- Fixed Yugoslavist Uprising event making you declare war on yourself by moving balkfm.214 from gbbf_monthly_pulse to turkfm_monthly_pulse

--Update 3.0.3--
Fixes:
- Fixed certain rite modifiers not getting removed correctly
- Fixed eocfm.169 being able to fire multiple times before applying its modifier
- Fixed a typo in a script value which reduced the rite modifier to 10% of its intended value


--Update 3.0.2--
Fixes:
- Reworked poor effect structure in turkfm_sick_man.005 & turkfm_sick_man.006


--Update 3.0.1--
New Additions:
- Added a new custom loc for controlling Constantinople with Autocephaly

Balancing/Adjustments:
- je_grefm_greater_greece now requires completing the Greek Nationalism journal with a hydrid identity choice
- je_grefm_greater_greece will now appear for Theodoro

Fixes:
- Fixed CTD in grefm.300 and added superevent window to grefm.800
- Adjusted Seat Controller custom loc and associated scripted effect


--Update 3.0-- "Mehmed Emin" **Major Update**
** Mod rename to "Gates of the Bosphorus" **

New Additions:
#### grefm
- Added PMs/PMGs to the Mega Palation and Hippodrome
#### turkfm
*First Chapter of Ottoman content up to the First Constitutional Era*
- Reworked "Sick Man" journal to represent the fight to hold onto and reclaim Ottoman territories and subjects
- New "Reordering the Empire" journal representing the attempts to modernize the Imperial administrative apparatus
- New "Rise of Nationalism" struggle-like journal integrating and expanding the "Eastern Question" content
- New Social Heirarchy and Institution representing the Millet System
- New Ideologies to better reflect Ottomanism vs Islamism
- New Journal "The Pirates of the Adriatic" for Albanian Piracy
-New Journals "Entrenching the State" & "Securing the Desert" for Libya
- New Journal "The Teachings of al-Sanusi" & decentralized tag for the Libyan Desert
- New Journal "The Modernization of Tunis" for Tunis
- Dozens of new characters for TUR, LIB, and TUN
- New decentralized country tag "Kufra" for the Libyan desert
- Decisions and events for major palace constructions
- New Buildings "Topkapı Palace" & Dolmabahçe Palace for the Ottomans
- New Building "Mohamedia Palace" for Tunis
- Added custom state names for the Libyan Desert
- Added custom Eyalet and Vilayet government types
#### balkfm
- Added new countries: Hersek, Yanya, and Silistra all selectable from the Objective screen
#### eocfm
**Updated to EOCFM 1.0.5**
- Includes all content from GBBF Version 2.3.6
- Removed all dependencies on grefm, turkfm, and balkfm content from GBBF
- Refactored and improved the entire localization file
- Added several new tooltips and improved existing tooltips
- Added a new icon selection event
- Added eocfm_is_eastern_christian scripted trigger
- Added New Patriarchate Buildings/PMGs/PMs
- Added Liturgical Rite Modifiers
- Removed Patriarch Deposition event
- Added new button to take control of Constantinople if you are not Autocephalous already
- Fixed and Updated Modifier Icons

Balancing/Adjustments:
#### grefm
- Greek Revolt mechanics integrated into the Rise of Nationalism and Eastern Question journals
- Removed the Greek Separatism journal & events
- Changed the "hellene" culture key back to "greek" for compatibility and instead replaced the localization
- Cappadocia, Theodoro, and Trebizond are no longer visible on the map in sandbox mode
- Added Government Administration PMs to the Mega Palation
- Moved Chariot Racing content into a series of PMs for the Hippodrome
- Refactored Greek Separatism buttons into Gunrunners buttons in turkfm
- Removed Chariot Racing Decision
- Added tooltips to the Embrace Identity buttons to warn players about primary culture shifts
- Megali Idea variants will fail if a country is missing the appropriate culture
- Megali Idea variants will not activate if a country already has an active variant
- Set up BYZ and GRE_HEL formables to exclude the primary culture of the opposite tag
- Removed greek culture from BYZ
- Hydrid Identity button now requires pan-nationalism
#### turkfm
- Downgraded Libya to Tier 5 starting tech
#### balkfm
- Removed Slav Agitation effects and replaced them with a Gun-running modifier/effect
- Moved around several events related to Ali Pasha in both Montenegro events and Bosnia events
- New journal "The Ambitions of Ali Pasha" for Hersek
- Added starting truces for Montenegro and Hersek with the Ottomans

Fixes:
- Fixed Balkan tags being created when a country with that tag already exists
- Austria will no longer fight the Ottoman's rebellions for them
- Removed Infinite Montenegros (it was funny, but it had to go)
- Reorganized notifications and added missing loc entries
- Fixed custom buildings showing up in every state\
- Streamlined some of the objective loc

Notes:
- The eqfm module has been merged into turkfm; majority of loc replaced
- The eocfm module has been separated into a separate workflow as it is now shared between Gates of the Bosphorus and Basielia Romaion
- Several files have been merged and renamed for workflow purposes
- Re-keyed several custom country tags to avoid collisions with vanilla and other mods

################################################################################

--Update 2.3.6--
Fixes:
-Added scripting for new CFM sidebar functionality
-Fixed Xenocracy wanting both positive and negative bureaucracy
-Removed held over gui file from pre-CFM

--Update 2.3.5--
Fixes:
-Fixed a missing option in grefm.030 if the Bavarocracy is secured
-Updated CRE, CYP, GRE, and ION definitions to be Hellene primary
-Embracing a Greek identity will now disable the other buttons in the Greek Nationalism journal
-Roman excavations events were calling the wrong loc
-Added missing event video to grefm.801 "Nova Rome Constantinopolitana"
-Fixed outliner not being hidden in the Orthodox Widget
-Fixed loc for Orthodoxy button running over other buttons
-Fixed country triggers for ideologies


--Update 2.3.4--
Fixes:
-Updated for new CFM functionality
-Fixed some missing loc

--Update 2.3.3--
New Additions:
-Expansion to the "Načertanije" journal, adding the ability to provoke Yugoslav rebellions in AUS/TUR and events to unite Yugoslav countries
-Added tags for Dalmatia and Slavonia
-Orthodox Realm (ODXY) path added as an Ecumenical Council option
-New meme journal for ANZFP users to form the Holy Byzantine Emu Empire (GRE_EMU)
-New scripted button for Romania to provoke revolts in Transylvania

Balancing/Adjustments:
-Reduced construction cost for the Old Royal Palace
-Moved Regulamentul sub-journals into the Ottoman Legacy group
-Simplified the sheer number of variables/values used by Romanian journals and implemented some custom loc
-Changed the "Foment Unrest in Austria" button to only target Transylvania
-Expanded & improved tooltips in the Romanian journals
-Added radicalism and modifiers to grefm.142 to make the "Consider Alternate Sites" button more impactful
-Changed the Megali Idea invalid conditions into proper tooltipped fail conditions


--Update 2.3.2--
Fixes:
-Changed Urum culture faith to Orthodox (Theodoro now correctly starts as Orthodox)
-Replaced a subtract with an add in the Khoine progress math


--Update 2.3.1--
Balancing/Adjustments:
-Added file to overwrite Greek state name triggers
-Moved Ottoman Legacy journals to their own journal group


--Update 2.3-- "Czartoryski" **Major Update**
New Additions:
-New journal "A Greek King" representing an alt-history search for a native-Greek king with options to exit the Bavarocracy early
-New journal "Scions of Rhōmanía" as a Rhomaios variant of the Megali Idea
-New journals "The Greek Plan" & "The Last of the Romans" as an Urum variant of the Megali Idea event chain
-Expanded "Greek Nationalism" journal, reflecting the struggle between Ancient Greek & Byzantine identities
-Formation of Byzantium (BYZ) and the Hellenic Empire (HEMP) are now enabled by Greek Nationalism outcomes
-Expanded Archaeology journal, allowing players to focus on Byzantine sites over Greek sites
-New dynamic names for BYZ & HEMP
-Added Konstantinos Kanaris & Gennaios Kolokotronis as agitators for Greece
-Added new Cappadocia tag for central Anatolia
-Added Trabzon, Cappadocia, & Theodoro as options in the Greek State objective

Balancing/Adjustments:
-Merged all Bavarocracy narrative journals into the main journal
-Removed Compulsory Primary School requirement from "The Language Question"
-Removed the "Grecoturkism" journal and events; if it ever returns it will *not* be in that form
-Byzantium (BYZ) & Yugoslavia (YUG) tags restored as formables
-Hellenic Empire (HEMP), Serbian Empire (SRPS) & Bulgarian Empire (TSAR) tags added as formables
-Removed Eastern Roman Empire (ERE) tag and its associated decision
-Removed Roman Empire (SPQR) tag, it is now a dynamic name for BYZ
-Removed the Orthodox Realms (ODXY) event chain
-Merged Chariot Racing Events
-Reduced Intelligentsia buff from "Westernized Thought" modifier to +10%
-Greece now starts with Freedom of Conscience & Private Schools enacted
-Greece now starts with the Devout as part of government
-Removed Empiricism triggers from Greek journals and events
-Changed the University of Athens event to add university throughput
-Reduced Agitator slots and IG buff from Westernized Thought modifier
-Adjusted the ratio of Hellene:Rhomaios pops
-Added South German pops to Greece; these will be removed if the Bavarian Auxilliaries are dismissed
-Greek Homeland events will now occur for both Hellene and Rhomaios countries (you still need Civilizing Mission)
-Added tooltip to Foment Unrest buttons indicating that they will cause a diplomatic incident
-Reduced Bureaucracy cost of Draining Lake Kopais to -100 down from -200
-Increased Bureaucracy cost of Surveying the Corinth Canal up to -200 from -100
-Removed Bureaucracy triggers from the Lake Kopais and Corinth Canal decisions; you're all big boys and girls
-Forming HEMP, BYZ, YUG, TSAR, and SRPS now requires being independent
-Removed country rank and Megas Palation requirement from the Greek empire journals

Fixes:
-Added Cyprus to the Hellene Greek sphere; this was an oversight
-Fixed Greek Separatism buttons still referring to Greek
-Fixed loc error in balkfm.688
-Fixed a CTD in balkfm.578
-Fixed broken triggers for the Greek Homeland events
-Fixed broken script value in the Romanian Nationalism journal

Notes:
-Deleted the Byzantine Empire for administrative reasons (byzfm module merged into grefm)
-Three path system for Greece has been replaced:
--The Purple Phoenix Path is gated behind forming Rhōmanía (BYZ)
--The Revenge of the Greeks Path is gated behind forming Hellas (HEMP)
--The Orthodox Realms Path has been removed and the Orthodox Realms (ODXY) will be formed via the Orthodoxy GUI in a future update


--Update 2.2.12--
Fixes:
-Updated mod for V3 1.8
-Fixed Greek Revolt buttons still referring to Greek culture


--Update 2.2.11--
Fixes:
-Fixed Bavarocracy completion variables not being set correctly
-Removed blank event that can occur for Montenegro
-grefm.110 is delayed by two years
-grefm.121 now requires empiricism


--Update 2.2.10--
Fixes:
-Fixed stale Greek culture reference in the on_actions
-Added compatibility trigger for TLIM
-Reduced farm levels requirement for GRE-side land reform journal to 5
-Fixed Land Reform journal accidentally checking all owned states


--Update 2.2.9--
New Additions:
-New event allowing Ottoman subjects to remain as Ottoman tributaries instead of being ejected without warning from the Ottoman market

Balancing/Adjustments:
-Replaced the "Sick Man" modifier

Fixes:
-Fixed reversed options loc in balkfm.611


--Update 2.2.8--
New Additions:
-Added four "Ottoman Legacy" journals, reflecting the post-Ottoman status of Balkan subjects
-Added event chain, country tag, & characters for the Vojvodina Uprising
-Added Petar Jovanović & Toma Vučić Perišić as starting politicians for Serbia
-Added Stanojlo Petrovic, Mileta Radojković, & Avram Petronijević as agitators for Serbia
-Added Stevan Šupljikac & Josif Rajačić as politicians for Vojvodina

Balancing/Adjustments:
-Adjusted starting political ideologies for Serbia
-Added pro-AUS lobbies to Serbia
-Added Diplomatic Catalysts to Dynastic Rivalry Events
-Greek Bavarocracy sub-journals will now relace themselves with the Ottoman Legacy journals if the Bavarocracy journal closes

Fixes:
-Added missing loc in balkfm.200
-Fixed CTD due to change in eventwindow.gui


--Update 2.2.7--
New Additions:
-Minor Events for the Reign of Danilo II
-Added Đorđije Petrović-Njegoš to Montenegro
-Added Mirko Petrović-Njegoš to Montenegro
-New Journal "The Croatian Question" for the emergence of Croatian Nationalism

Balancing/Adjustments:
-Added more progress sources for the Bulgarian National Awakening
-Bulgarian National Awakening journal now opens with Mass Communication (previously Nationalism)


--Update 2.2.6--
Balancing/Adjustments:
-Pro-constitution Greek characters now use the "Constitutionalist" ideology

Fixes:
-Removed grefm.111 and its hidden variable that could block the Lake Kopais Decision
-Fixed the Caesaropapism source/expense tooltip

Notes:
-GBBF is confirmed to be broadly compatible with BPM; load this mod *after* BPM


--Update 2.2.5--
Fixes:
-Ionian Island annexation decision integrated into grefm and now uses the Hellene culture


--Update 2.2.4--
Balancing/Adjustments:
-Visit Tsar scripted button only requires cordial relations (instead of amicable)

Fixes:
-Greek Annexation Decisions updated to use the Hellene culture

--Update 2.2.3--
New Additions:
-Split Greek culture into Hellene, Rhomaios, & Urum as a first phase for Greek identity content; this is region based for now, with the Demotic Greek space receiving Hellenes, Crimea Urums, and the rest Rhomaios
-New Journal "Montenegrin Nationalism" to assert represent the Declarations of the Principality and Kingdom of Montenegro
-Added 10 random events that can occur while seeking autocephaly

Balancing/Adjustments:
-Homeland states adjusted for the new cultures
-grefm monthly pulse now uses Hellene culture
-Megali Idea journal is now gated behind Hellene culture (A Rhomaios variant is coming soon)
-All custom Greek tags switched to be either Hellene or Rhomaios
-Theodoro also has Urum as primary
-Replaced Sephardic culture with Romaniote in the Ionian Islands
-Increased Greece's starting tech tier
-Reduced Montenegro's starting tech tier
-Greek Feminism characters can now be recruited as agitators
-Reduced the progressbar requirement for the Bulgarian Exarchate from 1000 to 400
-Increased base autocephaly progress from 1 to 2
-Autocephaly monthly progress is no longer fixed and can be affected by choices during autocephaly events
-Adjusted the presentation of tooltips and script value descriptions for the Battenburg Monarchy journal to better show what contributes to the script value

Fixes:
-Fixed missing trigger for grefm.314 in grefm.307
-Fixed broken/looping event triggers in the Revenge of the Greeks sub-journals/events
-Corrected reversed option effects in eocfm.030 "The Struggle of the Clergy"
-Fixed an incorrect Custom Loc type in eocfm.150 "Ecumenical Financing"
-Fixed CTD when clicking balkfm_uplift_rumelia_button due to event not roping in TUR to create ERUM
-Lots of small typos in loc

Notes:
- "Depose Ecumenical Patriarch" button will be disabled if you control Constantinople. This is temporary pending a planned expansion to the Ecumenical Patriarchate.


--Update 2.2.2--
Fixes:
-Samos history and diplomatic history moved to GLOBAL to fix CTD with ANZFP mod


--Update 2.2.1--
New Additions:
-Added new building "Mountain Roads" for Montenegro.
-Phase I of "Black Mountain" journal rebuild complete.
-Added new state trait to Montenegro.

Fixes:
-Shrunk down margins in eocfm widget for lower resolutions.

Misc:
-Added script values, scripted buttons, and initial scripted effects for the Border Conflict.


--Update 2.2-- "Stambolov"
--New Additions:
-Content for the Reign of Ferdinand I / Stambolovism
-Event for the University of Belgrade
-Minor Flavor for Eastern Rumelia's governor-generals
-4 New journals and over a dozen events for the "Xenocracy" in the Ionian Islands
-Added the Principality of Samos for an additional cursed start along with the event chain "Samos in Submission"
-New "Imperial Ambition" journals for the Revenge of the Greeks Path and the Bulgarian Empire
--Teardown of Orthodox Content taking advantage of the new Scripted Widgets:
-Removed Eastern Orthodox journals and replaced them with a new widget
-Removed all eocfm scripted_buttons and replicated their functionality with the widget
-Removed all eocfm annexation decisions (these run contrary to the ethos of Sphere of Influence)
-New Seat Integration events/actions, Autocephaly events, and events for Unifying the Church

Balancing/Adjustments:
-Greece, Montenegro, Serbia, and Romania now start with their initial journals assigned (Ionian Islands, Samos, and Silistra have this by design as well)
-Bavarocracy journal now uses script values instead of variables and custom loc
-Added scripted progressbars to the Greek Language Journal for each dialect
-Adjusted Byzantium path variables for increased flexibility to give more tags access to forming Byzantium in the future
-Added several new toast messages for eocfm events/actions
-Adjusted triggers for the Rumelian union/annexation buttons
-Added alternate "Declare Tsardom" button and event incase Bulgaria is already independent
-Only political leaders will contribute their popularity to the Dacianism/Junimism debate

Fixes:
-Added missing OR in eocfm_is_integrating_seat_trigger
-Finally nailed down a local/global variable mismatch preventing the Turkish Homeland events
-Romanian 1848 variables are correctly initialized
-Fixed nasty typo in eocfm script value
- "Commission Icon" button will not get stuck greyed out for the entire game anymore


--Update 2.1.6--
Fixes/Adjustments:
-Building the Peles Castle will now correctly remove the construction penalties
-Added a fallback decision to remove the modifiers incase they get stuck
-Peles Castle decision now correctly checks to make sure the castle exists


--Update 2.1.5--
Fixes/Adjustments:
-Fixed Scripting for Revolt Buttons
-Added ai_chance to the Greek Separatism buttons to avoid going bankrupt from supporting separatism
-Fixed an incorrect variable trigger preventing the Turkish homelands event
-14 Regions journal will be available immediately after forming BYZ/ERE
-Option to Elect a member of House Ypsilantis to the greek throne has been switched to always appear
-Option to abolish the monarchy in "An Elected Monarch" will enact Parliamentary Republic instead of Presidential. It still requires Egalitarianism to appear.


--Update 2.1.4--
**Updated for V3 1.7**
New Additions:
-New Opener journal "The Armansperg Regency" for Greece with event chain to introduce the Bavarocracy
-Greek Revolts are now handled by je_grefm_greek_separatism
-Revolts will now fire based off a mixture of radical_fraction and Greek support
-New journal entry "The 14 Regions" representing the historic urbanization of Constantinople
-New state trait "The Golden Horn" for Eastern Thrace

Balancing/Adjustments:
-Complete Teardown of "The Bavarocracy" journal and sub-content. The timeout is now a progress bar that drains monthly; this drain speed can be slowed down by completing the sub-journals
	-Integrated the Bavarian Auxilliaries and Turk-Eater decisions as scripted buttons within the main Bavarocracy journal.
	-Old Royal Palace is now available during the Bavarocracy journal chain instead of after abandoning the Byzantine Restoration
	-Added new scripted button to get foreign loans
	-New event "The Philorthodox Conspiracy" behaves like a grefm-specific version of eocfm.006
	-Constitution modifiers also impact political strength on top of opinion.
-Reworked the "Tyranny of House Wittelsbach" journal; The timeout is now a progress bar that depends on IG clout, enacted laws, and ruler popularity.
-Reworked the completion requirements of "A Bavarian Greece" ; it now behaves as an inverse Stamp Out Monarchy journal
-The Megali Idea opening event now adds all claims at once; grefm.200/201 have been merged and the Treaty of Laussane option has been removed
-Reworked events for Archaeology, some have been demoted to notifications and others have new options
-Integrated the Mega Palation survey button into "The 14 Regions"
-Removed Hippodrome survey
-Greece/Byzantium monuments now longer appear in every state
-Removed Cretan Revolt journals
-Removed legacy Venizelism journal
-Subsidizing the Church will now reduce their political strength
-Caesaropapism now reduces Devout political strength by 25%
-New option in grefm.031 in case you arrived via success in Bavarocracy Main
-Added global notification in the event that a riot is suppressed
-Suppressing a riot will reduce tension by 200
-Hidden event added that can start the rioting event chain randomly any time Tension is over 400
-eqfm rebellion effect now creates a dominion with an option to grant autonomy to bring it in line with how grefm rebellions behave

Fixes:
- "Comission Icon" button will now be disabled if the event is active
-Stop Church Subsidies button is now visible regardless of your current amount of PA
-Epirote Revolt event now snatches all Greek pops in Ottoman Albania and moves them to Epirote Albania
-Fixed a trigger issue preventing the stop subsides button from appearing if you have don't have enough PA.
-Deconfliction will now be correctly limited to Balkan uprisings
- "Churches Burned in State" option now correctly deducts money
-Adjusted rounding in some script values.
-Kogalniceanu is now correctly freed from the void
-Milos no longer wears a fez


--Update 2.1.2--
New Additions:
-Added new journal "Romanian Liberalism" representing the political upsets of 1848
-Added new journal "Statutul Dezvoltător" representing the downfall of Alexander Cuza
-Added event representing the election of Carol I
-Added new journal "Greater Romania" representing the expansion of Romania in the 1900s
Balancing/Adjustments:
-Natural secessions in the Balkans will place the struggle into Deconfliction
-All tension events for the Ottomans now send feed notifications
 -Requirement to abolish State Religon replaced with Peasant Levies in "Regulamentul: Legal Standards"
-Exposed values for Serbian Dynastic Rivalry and reworked the underlying scripting to support this
Fixes:
-Eastern Question rioting event will now correctly trigger at high tension
-Ottomans will no longer receive two Eastern Question journals
-Removed Olympics Restoration event; this mod now adjusts the Olympics cost down by 5%
-Greek homeland claims now correctly blocked behind Greece (or any Greek Empire) not existing
-Moldavian Regulamentul journal election cycle reduced to 7 years instead of 14
-Button to divest from Balkan Mitigation/Acceleration is actually visible now

--Update 2.1.3--
New Additions:
-Added new journal "Romanian Nationalism" with events for the literary conflict between Junimism and Dacianism.
-Added two variants of a new journal "Romanian Constitutionalism" to represent the Constitution of 1866.
-Added new journal "A Romanian Empire" to restore the Byzantine Empire with a fixed path to the Purple Phoenix; this triggers after completing Romanian Nationalism.
-Added new building and journal for the Peles Castle; this process will be the standard for monument construction going forward.
-Added minor event for the Romanian National Academy
-Added five DNA sets for Romanian characters courtesy of LordR

Balancing/Adjustments:
-Natural secessions from outside eqfm will also put the Balkans in Deconfliction.

Fixes:
-Removed radical fraction triggers from eqfm riots event and rebuild a lot of the scripting.
-Added missing localization to eqfm events.


--Update 2.1.1--
Fixes:
-Fixed poor trigger structure in checking for an ongoing Ecumenical Council


--Update 2.1-- "Garašanin"  **Major Update**
• Third Chapter of Content for Greece:
	-Event "Nationalist Fervor" has been given content and handles triggering the "Military League" vs. "A Cretan Champion." While less dramatic in most games, this ensures that players will have access to Venizelism content.
	-Journal Entry "Venizelism" now consists of a journal chain similar to the "Bavarocracy," giving the player a chance to experience Venizelos' massive influence over the Greek state.
	-New Event Chain for the "Don Pacifico Affair"
	-Crete Revolt mechanics reworked to take into account Greek radicalism on Crete.
• First Chapter of Yugoslavian Content:
	-Načertanije: Reworked to provide a path to Yugoslavian formation. Take charge of the Yugoslavian cause and diplomatically annex other Yugoslav nations to form Yugoslavia.
• Second Chapter of Serbian Content:
	-Cementing the Monarchy: Balance the reactions of Serbian and Turkish politicians to the Declaraton of a Hereditary Monarchy.
	-Constitutionalism: Guide Serbia through poltical reform under the influence of Ristic.
	-Greater Serbia: Reject Yugoslavism and restore the Serbian Empire.
• Expansion of Content for the Balkans Struggle:
	-The Eastern Question: Defend or Oppose Ottoman interests in Rumelia or take the reigns as the Sultan as the peoples of the Balkans struggle to break free.
	-20 new events and two journals representing the simmering separatism in the Balkans.
• First Chapter of Romanian Flavor:
	-The Regulamentul Organic: Guide the Romanian Principalities through their transiton from post-Ottoman state & elect a new Hospodar every 7 years.
	-Vanilla Romanian Unification events integrated into this mod.
• Minor Addition for Slovene-Croatian Flavor:
	-The Triune Dream: Minor journal entry to properly form the Triune Kingdom.
	-No immediate plans for further work, but Slovene-Croatian flavor is on the docket.
• Other fixes/additions:
	-Increased probability of the Greek/Turkish homeland events by 25x.
	-Agitating in Crete should no longer give the Ottomans/Egyptians infinite infamy
	- "A Bavarian Greece" journal no longer thinks you went bankrupt on completion
	-Byzantium has a new event for getting a Palaiologos Ruler post-1863
	-BYZ, ERE, & ODXY now have a new flag for autocratic theocracies
	-YUG is no longer formable from the nation formation tab
	- "Convoke Ecumenical Council" now has a tooltip indicating what "calls their attention"
• Notes for Sphere of Influence:
	-Event providing a Customs Union between Greece and Epirus has been removed in preparation for SoI.
	-Greece, Bulgaria, and Serbia will receive relevant political lobbies, dependent on what PDX gives them.


--Update 2.0.5--
-Increased probability of the Greek/Turkish homeland events by 25x
-Fixed poor on_action structure causing the Congress of Berlin to repeatedly restart
-The Megali Idea no longer requires Monarchy to complete; also only requires owning Constantinople plus 10 of the formation states; Crete and Ionian Islands now count for this goal.
-Reduced cost of expeditions to -50, and surveys to -100


--Update 2.0.4--
- "The Royal University of Athens" event will no longer occur if Morgenröte is also loaded.
- "Annex Rumelia" button now appears if either Bulgaria and Eastern Rumelia are both subjects of the Ottomans, or if both are independent. This is a fallback incase the Ottomans fail the Sick Man journal AFTER the Great Eastern Crisis. It also will not appear if a player is Eastern Rumelia (but why would you do this).
-Fixed the crisis variables being removed too quickly by a forgotten effect, preventing countries from getting post-Crisis modifiers. (The previous fix exposed this issue).
-Crete's former owner now gets a war goal to reconquer Crete instead of letting them go free after the play.


--Update 2.0.3--
-Updated to Vic3 1.6
-Fixed an issue where the crisis variables were not properly removed following a Turkish victory
-Changed Ferdinand I's last name to Sakskoburggotski (this is anachronistic, but it fits better in the GUI)
-Removed some Bulgarian names from the localization that are now covered by the vanilla localization


--Update 2.0.2--
-Crusade DP now unlocks correctly
-Added 3 events for Crusade start, victory, and defeat


--Update 2.0.1--
-Fixed Obrenović and Karađorđević script values and tooltips incorrectly aligning them to Russia and Austria respectively.
-Added new checks to the GEC Warmup event. Now checks for TUR to not be a subject or junior in a CU. Crisis will not fire at all once TUR has researched pan-nationalism.
-Added a tooltippable to the Patriarch Authority JE explaining all possible sources of PA.
-Added status_desc to the Cretan Revolts JE so Muslim nations can see the current revolt momentum
-Added event recruiting countries with alliances/defensive pacts to defend TUR


--2.0-- **Major Update**
# Mod Rename to "Greece, Byzantium, and the Balkans Flavor (GBBF)
• Third Chapter of Content for Greece representing the role of Venizelos in poltitics.
	• Venizelism: Take Greece along either a republican or monarchist path by either embracing or opposing the reforms of Venizelos.
	• Greater Greece: Guide Greece through the build-up to the Balkan Wars and the greater question of its role in the Balkans.

• New Content Module for Balkans Flavor:
	• Content for Montenegro through the rule of Danilo II:
		• The Prince-Bishropic: Guide Montenegro into becoming a modern nation state.
		• The Wrath of Ali Pasha: Stand your ground against neighboring Ottoman Pashas as they attempt to assert Ottoman authority over Montenegro.
	• Content for Serbia through the rule of Milan I:
		• Constitutionalism: Experience the back-and-forth between houses Obrenović and Karađorđević for control over Serbia.
		• Načertanije: Promote the growth of Yugoslavism as a means to expand Serbian influence.
	• Content for Bulgaria through the short reign of Alexander I:
		• The Battenburg Monarchy: Struggle to maintain power as Alexander I against the Russophiles.
		• The Unification of Bulgaria: Seek Unification with Eastern Rumelia and break free from Ottoman suzerainty.
		• The Golden Lion Roars: Assert Bulgarian revanchism to restore either the Bulgarian Empire or the Byzantine Empire.
	• Content representing the Great Eastern Crisis of 1875-1878:
		• Join either side in supporting or opposing Ottoman authority in the Balkans.
		• Major and minor Turk-splosion events will occur following Ottoman defeats in the Balkans.

• New Content Module for Eastern Orthodox Church Flavor:
	• The Bishops of the East: Utilize state control over the Orthodox Church to assert independence from the Ottoman-controlled Ecumenical Patriarch.
	• Patriarch Authority: Inspired by the system from EU4, gain bonuses based on support from the Church.

• Mod Compatibility:
	• GBBF is now compatible with Morgenröte - Dawn of Flavor. Having both mods active will enable alternate journal entries and additional events within this mod.

• Minor Adjustments/Fixes
	• Epirus now gets a large opinion modifier towards Greece for the purposes of the Customs Union

NOTE FOR TRANSLATION MODS: *Every event* in byzfm has been reordered or modified.


--1.1.4-- *Minor Update**
• Minor Adjustments/Fixes:
	• Added alternate pathways to trigger "A Cretan Champion" assuming you don't meet the conditions for "The Military League"
	• Added event reminding the player that they have a claim on Thessaly (this is a vanilla feature) and don't have to wait for the Megali Idea
	• Ionian Islands receives claims on Attica, Peloponnese, and Thessaly if they go independent (they can already receive the Megali Idea)
	• Epirus revolt will take chunks of Thessaly if its still owned by the Ottomans
	• Event will trigger allowing Epirus to join the Greek market if they manage to become independent
	• Reworked how the cretan revolts journal is handed off between countries that conquer Crete
	• Fixed localization problem with the Turkish Homeland events
	• Women's journal will only fire for Greece


--1.1.3-- **Minor Update**
• Minor Adjustments/Fixes:
	• Removed leftover triggers in the Tyranny and Cultural Roots journals that were blocking progress
	• Fixed a global/loval variable mismatch blocking the Gla excavation
	• Added an excavation for Rhodes & another excavation event that didn't make it for 1.1


--1.1.2-- **Minor Update**
• Minor Adjustments/Fixes
	• Added fixed appearances for several characters.
	• Rebalanced the Lake Kopais journal, the drainage events will trigger more quickly and the Gla excavation should unlock correctly now.
	• Added a prestige buff for completing excavations
	• Added a new "Bavarocrat" ideology to Josef Ludwig von Armansperg and King Otto
	• Removed several IG opinion modifiers during the Bavarocracy phase, the new ideologies are more in line with vanilla game design; IGs will also switch to more liberal ideologies if you go the liberal route based on their support for autocracy
	• Olympics Event only fires once now


--1.1.1-- **Minor Update**
• Minor Adjustments/Fixes on the Greece Side:
	• Added discrete journal groups for a total of 10 groups
	• Added Trikoupis as a character (along with Andreas Metaxas, Alexandros Kontostavlos, Nikitas Stamatelopoulos, and 	Kanellos Deligiannis)
	• Added a new event/modifier for Greece's long history of maritime shipping
	• Removed the progress bar from the Lake Kopais journal; it was misleading
	• Minor adjustment to the Cretan Revolts

• Minor Adjustments/Fixes on the Byzantium Side:
	• Removed the progress bar from the Purple Phoenix journal
	• Adjusted layout of objectives in the Orthodox Realms journal


--1.1-- **Major Update "Trikoupis"
• New Content for Greece:
	• The Dedilomeni Principle: Establish legitimacy in the democractic process under George I.
	• The Military League: Experience a new series of events and journals through the Military League and the Rise of Venizelos.
	• Greek Nationalism: Follow a series of journal entries and events to establish a discrete Greek identity separate from Slavic or Turkish influence.
	• Greek Cultural Roots: Conduct a series of excavations for the Greek Archeological Service
	• The Women's Journal: Support the efforts of Kalliroi Parren in gaining basic rights for women.

• Minor Adjustments/Fixes on the Greece Side:
	• Events on the grefm side have been reorganized under the hood
	• Expanded the Megali Idea journal to fund and provoke revolts in Epirus, Macedonia, and Cyprus along with mechanics for repeatable revolts on Crete and a new Macedonia revolter tag.
	• Added events and journal entries for industrialization and feminism in Greece.
	• Additional events and decisions during the reign of Otto I.

• Minor Adjustments/Fixes on the Byzantium Side:
	• New titles and a personality trait for Byzantine Emperors
	• Decision to change tag to the Eastern Roman Empire (c:ERE)
	• A silly event involving the Hippodrome
	• Small tweaks to the event chains for rebuilding the Imperial Palace and Hippodrome
	• Fixed the Crusade DP (now uses the "Make Protectorate" wargoal)


--1.0.1-- **Minor Update**
• Minor Adjustments/Fixes on the Greece Side:
	• Updated for compatibility with 1.5.7
	• Added temporary decisions to provoke the Epirus and Cyprus revolts (these are temporary and will be replaced with better scripting in 1.1


--1.0-- **Initial Release**
• Content for Greece:
	• The Bavarocracy: A series of events and journals centered around the "Bavarocracy" and the stagnation of the Greek state under Otto I up to the election of George I.
	• The Megali Idea: A rework of the "Greek Nationalism" journal and event chain, ending with the reformation of Byzantium (or you can remain Greece too).
	• Historical characters and an agitator for the era of Otto I.
	• New Epirus revolter tag and the ability to provoke historical revolts in Epirus and Cyprus (and annex them diplomatically).
	• Decision to build the Corinth Canal and event to build the Old Royal Palace.
	• Rebalances the Olympics modifier to make the cost less punishing long-term.
	• Minor event representing the autocephaly of the Greek Orthodox Church

• Content for Byzantium:
	• The Byzantine Restoration: Events and journal entries to reclaim the former Eastern Roman Empire.
	• Alt-history for Byzantium: Branching event chain to reform the Roman Empire, reclaim the lands conquered by the Muslims, or establish control over the Orthodox peoples each having a new country tag and flag.
	• Ability to rebuild the Imperial Palace and the Hippodrome, along with a decision to revive chariot racing (replaces the Olypmics).
	• Theodoro and Trebizond as releasable tags.
	• Homeland events regarding Turkish homelands in Anatolia.
	• Dynamic names for Byzantium
	• Minor Option to Elect a Palaiologos ruler in 1864



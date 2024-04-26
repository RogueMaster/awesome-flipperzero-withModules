<h1>Flipper Zero firmware differences</h1>
<h3>
    <code>::</code> Last updated April 25, 2024. <code>::</code>
</h3>
<p>This document will <em>(hopefully)</em> maintain a list of differences between various forks of the <a
    href="#official">Flipper Zero firmware</a>. <br>If I had a dollar for every time I&#39;ve seen this question asked,
  I wouldn&#39;t be in college debt. ¯\_(ツ)_/¯</p>
    <table><tr>
      <td>
        <strong>Jump to:</strong>
      </td>
      <td><a href="#plugins">RogueMaster</a></td>
      <td><a href="#unleashed">Unleashed</a></td>
      <td><a href="#Momentum">Momentum</a></td>
      <td><a href="#official">Official</a></td>
      <td><a href="#Xtreme">Xtreme</a></td>
      <td><a href="#Dexv">Xvirus</a></td>
      <td><a href="#Squachware">Squachware</a></td>
      <td><a href="#summary">Summary (TL;DR)</a></td>
    </tr></table>

<h2 id="plugins">RogueMaster<kbd>
    <a href="https://github.com/RogueMaster/flipperzero-firmware-wPlugins">RogueMaster/flipperzero-firmware-wPlugins</a>
  </kbd>
</h2>
<ul>
  <li>Remains the best and most updated firmware in the community</li>
  <li>Built off Unleashed as the base firmware (which is a fork of Official dev firmware.)</li>
  <li>First to allow for rename through Name Changer app.</li>
  <li>First to allow for removal of Sub-GHz regional transmission restrictions through Extend Range app.</li>
  <li>Passport fully customizable</li>
  <li>Removes Sub-GHz regional transmission restrictions after changes to <em>extend_range.txt</em> file.</li>
  <li>Allows Sub-GHz extended frequency range (i.e. restaurant pagers) through <em>extend_range.txt</em> file.</li>
  <li>Has Sub-GHz protocols and all the other changes taken from Unleashed FW (see <a href="#unleashed">changes</a>).</li>
  <li>Adds extra custom assets <em>(Mifare classic dict, example files, fun files, etc)</em>.</li>
  <li>Includes some PRs from Unleashed and Official firmware that are not yet merged <em>(bleeding edge)</em>.</li>
  <li>Includes a number of games, some experimental, as well as a real "Games Only Mode".</li>
  <li>Includes an enhanced new "Dolphin Level" system.</li>
  <li>Has added most known community tweaks, plugins & games</li>
  <li>Also includes a number of other small tweaks and changes.</li>
  <ul><li>More details and full list in their <a href="https://github.com/RogueMaster/flipperzero-firmware-wPlugins#readme">README</a>.</li></ul>

</ul>
<h2 id="unleashed">
    Unleashed
    <kbd>
        <a href="https://github.com/DarkFlippers/unleashed-firmware">DarkFlippers/unleashed-firmware</a>
    </kbd>
</h2>
<ul>
    <li>Somewhat active development and Discord community.</li>
    <li>Removes Sub-GHz regional transmission restrictions by default.</li>
    <li>Allows Sub-GHz extended frequency range (i.e. restaurant pagers) through <em>dangerous_settings</em> file.</li>
    <li>Adds extra Sub-GHz frequencies by default through Official <em>setting_user</em> file.</li>
    <li>Adds extra Mifare classic keys to included dict file and leaves user file untouched.</li>
    <li>Can be used to capture and send dynamic encrypted protocols/rolling codes. <em>(Modern garage doors, etc.)</em>
    </li>
    <li>Encrypted Sub-GHz signals and codes can be added manually.</li>
    <li>Current modified and new Sub-GHz protocols list <a
            href="https://github.com/DarkFlippers/unleashed-firmware#current-modified-and-new-subghz-protocols-list">can
            be found here</a>.</li>
    <li>Comes with extra apps and plugins from the general community through SD Application loader (FAP files).
        <ul>
            <li>More details and full list of changes can be found in their <a
                    href="https://github.com/DarkFlippers/unleashed-firmware#readme">README</a>.</li>
        </ul>
</ul>
  
<h2 id="Momentum">
    Momentum
    <kbd>
        <a href="https://github.com/Next-Flip/Momentum-Firmware">Next-Flip/Momentum-Firmware</a>
    </kbd>
</h2>
<ul>
    <li>Xtreme but without the NSFW BS, a direct continuation of the Xtreme firmware.</li>
    <li>Adds custom UI and custom Main Menu themes, and asset packs (icons, animations)</li>
    <li>Removes Sub-GHz regional transmission restrictions by default.</li>
    <li>Allows Sub-GHz extended frequency range (i.e. restaurant pagers) through Momentum Settings App.</li>
    <li>Allows changing Flipper's name via Momentum Settings App</li>
    <li>Has Sub-GHz protocols and most of the other changes taken from Unleashed FW (see <a href="#unleashed">changes</a>).</li>
    <li>Adds extra custom assets <em>(Mifare classic dict, more animations (installed separately), example files, etc)</em>.</li>
    <li>Includes an enhanced/improved "Dolphin Level" system similar to RogueMaster.</li>
    <li>Includes extra apps and plugins from the general community through SD Application loader (FAP files).</li>
    <li>Also includes a number of other small tweaks, changes, and stability fixes.</li>
</ul>

<h2 id="official">Official<kbd>
    <a href="https://github.com/flipperdevices/flipperzero-firmware">flipperdevices/flipperzero-firmware</a>
  </kbd>
</h2>
<ul>
  <li>Has region-locked Sub-GHz transmission because of legal limitations.</li>
  <li>Has no ability to save and send rolling codes (dynamic encrypted) in Sub-GHz, only shows them in captured list.
  </li>
  <li>Factory-set device name that shows everywhere (Bluetooth broadcast, USB connection, etc) that cannot be changed.</li>
    <li><em>The Flipper team has a list of device names with their corresponding production information <a href="https://discord.com/channels/740930220399525928/765282833744265246/971881286543224852">(No shipping address)</a> so they can assist you easier in case of an RMA.</em></li>
  </ul>
<h1 id="official">Outdated Below
  </kbd>
</h1>
<h2 id="Xtreme">
    Xtreme
    <kbd>
        <a href="https://github.com/Flipper-XFW/Xtreme-Firmware">Flipper-XFW/Xtreme-Firmware</a>
    </kbd>
</h2>
<ul>
    <li>Built from RogueMaster originally then converted to fork of <a href="#unleashed">Unleashed</a> + <a href="#official">Official</a> FW for future development.</li>
    <li>Adds custom UI and custom Main Menu themes, and asset packs (icons, animations)</li>
    <li>Removes Sub-GHz regional transmission restrictions by default.</li>
    <li>Allows Sub-GHz extended frequency range (i.e. restaurant pagers) through Xtreme Settings App.</li>
    <li>Allows changing Flipper's name via Xtreme Settings App</li>
    <li>Has Sub-GHz protocols and most of the other changes taken from Unleashed FW (see <a href="#unleashed">changes</a>).</li>
    <li>Adds extra custom assets <em>(Mifare classic dict, more animations (installed separately), example files, etc)</em>.</li>
    <li>Includes an enhanced/improved "Dolphin Level" system similar to RogueMaster.</li>
    <li>Includes extra apps and plugins from the general community through SD Application loader (FAP files).</li>
    <li>Also includes a number of other small tweaks, changes, and stability fixes.</li>
</ul>
<h2 id="Dexv">
    Xvirus
    <kbd>
        <a href="https://github.com/Xvirus-Team/xvirus-firmware">Xvirus-Team/xvirus-firmware</a>
    </kbd>
</h2>
<ul>
    <li>Fork of <a href="#unleashed">Unleashed FW</a></li>
    <li>Adds custom-themed graphics that are not included in the Official Firmware.</li>
    <li>Removes Sub-GHz regional transmission restrictions after changes to <em>extend_range.txt</em> file.</li>
    <li>Allows Sub-GHz extended frequency range (i.e. restaurant pagers) through <em>extend_range.txt</em> file.</li>
    <li>Has Sub-GHz protocols and most of the other changes taken from Unleashed FW (see <a href="#unleashed">changes</a>).</li>
    <li>Adds extra custom assets <em>(Mifare classic dict, example files, etc)</em>.</li>
    <li>Includes extra apps and plugins from the general community through SD Application loader (FAP files).</li>
</ul>
<h2 id="Squachware">
    Squachware
    <kbd>
        <a href="https://github.com/skizzophrenic/SquachWare-CFW">skizzophrenic/SquachWare-CFW - [TalkingSasquach](https://www.youtube.com/@TalkingSasquach)</a>
    </kbd>
</h2>
<ul>
    <li><em>(OEM+)</em></li>
    <li>Fork of <a href="#official">Official</a>.</li>
    <li>Adds custom-themed graphics that are not included in the Official Firmware.</li>
    <li>Keeps Sub-GHz regional transmission restrictions like Official Firmware.</li>
    <li>Has many of the apps that are available from <a href="#plugins">RogueMaster</a>.</li>
    <li>Fresh and active firmware forked from OFW.</li>
    <li>Adds custom animations/moods.</li>
    <li>Includes built-in name changer! (No recompile required to change your devices name).</li>
    <li>Includes extra community based apps and plugins through SD Application loader (FAP files).</li>
    <li>Includes community based Bad USB scripts.</li>
    <li>Includes community based Sub-GHz files.</li>
            <ul>
            <li>More details can be found in their <a
                    href="https://github.com/skizzophrenic/SquachWare-CFW">README</a>.</li>
        </ul>
</ul>
<h2 id="summary">
    📝 Summary
    <kbd>(TL;DR)</kbd>
</h2>
<ul>
    <li>Staying up to date with upstream (official) firmware is important.</li>
    <li>TX restriction removal is illegal in most circumstances, use at your own risk.</li>
    <li>RogueMaster is more focused on visual tweaks, new items, and changes (some experimental).</li>
    <li>RogueMaster is based on Unleashed and OFW and keeps up to date on both on a daily basis.</li>
    <li>Unleashed is more focused on core functionality, stability, and Sub-GHz protocols.</li>
    <li>SquachWare is forked from OFW, adding lots of custom stuff to play with out of the box all while retaining the securities and comfort of OFW.</li>
</ul>

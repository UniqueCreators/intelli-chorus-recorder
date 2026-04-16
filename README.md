# Intelli Chorus Recorder


## Introduction

Intelli Chorus Recorder is a professional-grade REAPER extension engineered to automate and streamline the intricate process of recording layered vocals, harmonies, and instrumental doubles. Developed by Unique Creators, this script is built from the ground up with a core philosophy of universal design and total accessibility. It ensures seamless compatibility with screen readers like NVDA and JAWS via OSARA, providing a robust, hands-free workflow for all audio professionals.


### ⚠️ **SECURITY WARNING: MALICIOUS CLONE DETECTED**

We have identified a malicious clone repository impersonating Intelli Chorus Recorder and distributing malware.

**Official Project:** https://github.com/UniqueCreators/intelli-chorus-recorder  
**Official Website:** https://www.uniquecreators.net  

❌ **DO NOT install from any other repository or unauthorized sources**

If you are installing Intelli Chorus Recorder, ensure you:
1. Use the official UniqueCreators repository
2. Install via ReaPack using our official URL (see Installation section below)
3. Verify the author is **Unique Creators** (https://www.uniquecreators.net)

For security concerns, contact: www.uniquecreators.net/contact

---


## Features

- **Step-by-Step Setup Wizard:** An intuitive, fully accessible initialization process ensures all parameters are configured swiftly without confusion.
- **Session Persistence:** Retain your project settings (track counts, optimal panning, UI preferences) across sessions to maintain creative momentum. 
- **Automated Routing & Track Management:** Automatically generates, routes, organizes into folders, and names tracks, reducing administrative overhead.
- **Intelligent Stereo Panning:** Dynamically calculates mathematically accurate stereo spreads for multiple recording passes based on defined width.
- **Automated Punch-In/Out:** Operates via time selections to perfectly execute automated punch-ins and punch-outs for an unlimited sequence of takes, minimizing user intervention.
- **Screen Reader First:** Integrated spoken auditory feedback (via OSARA) at every phase over the entire recording loop.

## Installation

We utilize ReaPack to ensure you always have the latest, most stable version of our tools. Follow these steps to install the Intelli Chorus Recorder:

1. **Install ReaPack:** If you haven't already, download and install [ReaPack](https://reapack.com/) for REAPER.
2. **Launch REAPER:** Open your digital audio workstation.
3. **Open Extensions:** Press `Alt + X` to open the Extensions menu.
4. **Access ReaPack:** Navigate to the `ReaPack` option and press `Enter` (or click) to open its submenu.
5. **Import Repository:** Select the `Import repositories` option.
6. **Add URL:** Paste the Unique Creators repository URL: `https://raw.githubusercontent.com/UniqueCreators/ReaScripts/main/index.xml`
7. **Confirm:** Press `Enter` or click `OK`.
8. **Sync Packages:** To download the newly added repository data, go to the `Extensions` menu -> `ReaPack` -> `Manage repositories`.
9. **Browse:** Scroll to the bottom of the list to verify the URL is present, then press `Alt + B` or click the `Browse packages` button.
10. **Search:** In the `Filter` edit box, search for **Intelli Chorus Recorder** and press the `Down Arrow` once to focus the list. You will find the script there.
11. **Select Actions:** Press the `Tab` key to reach the `Actions` button and click it.
12. **Install:** Choose the `Install` option (the very first item in the context menu).

*Congratulations! The script is now installed and ready to be used.*

## How to Use

Intelli Chorus Recorder requires minimal setup per use, relying on standard REAPER time selections to handle the heavy lifting.

1. **Set the Recording Range:** First, create a time selection in your REAPER project that spans the exact duration you intend to record (e.g., the 8-bar chorus). *This step is mandatory.*
2. **Execute the Script:** Run the script via the REAPER Actions list, or assign it to a custom keyboard shortcut for rapid access.
3. **Configure the Wizard:** 
    - Upon first launch, the wizard will sequentially prompt you for your setup: Track Count, Max Stereo Pan Width, Input Channel, Track Naming, Folder Grouping, and playback behaviors like Metronome and Count-in.
    - If you have run the script before, it will first ask if you simply want to load your previously saved session settings.
4. **Perform:** Once initialized, the script automatically stops playback, readies the tracks, and begins recording the first layer. 
5. **Loop and Stack:** It will flawlessly auto-stop at the end of the time selection, arm the next track, and begin recording the next take. 
6. **Completion:** A confirmation prompt will notify you when all requested tracks have been beautifully stacked, panned, and recorded.

## FAQs

**Q: Do I need to be a screen reader user to benefit from this script?**  
A: No! While built with extreme accessibility in mind, the automation features save massive amounts of time for any engineer or artist laying down vocal stacks or doubles.

**Q: Why does the script tell me a prerequisite is missing?**  
A: The script requires an active time selection in REAPER so it knows exactly when to punch in and out automatically. 

**Q: Can I use different inputs for each track?**  
A: Currently, the setup wizard asks for a single physical input channel designed for recording a single performer stacking takes sequentially.

**Q: Does it work with the metronome?**  
A: Yes. If your metronome is disabled when firing the script, it will actively prompt you and give you the choice to enable it.

## Support & Contributions

This modular release is open-source. We welcome community contributions! Please review the `CONTRIBUTING.md` file included in this repository.

For technical support, custom accessibility tools, studio inquiries, or to report bugs:
- **Open a Ticket:** Contact us via our official portal at [www.uniquecreators.net/contact](https://www.uniquecreators.net/contact)
- **Website:** [www.uniquecreators.net](https://www.uniquecreators.net)

*We are Unique Creators, and creation is our passion!*

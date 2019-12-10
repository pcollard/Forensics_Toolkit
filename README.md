# Forensics_Toolkit
Comprehensive toolkit for all digital forensics tools used, with brief explanations to facilitate ease of usage.

Linux VMs
The following are prebuilt vms designed to help a forensics investigator by giving them prebuilt tooks and enviornments.

- Caine
  - Computer Aided Investigative Environment, CAINE. Linux distro that contains similar tools to other forensics distros. Contains a GUI with tight security and built-in digitial investigation tools. Less noob friendly.
- Deft 8.2
  - Also contains tools prebuilt into the installation without the need for automated mounting scripts.
- Paladin
  - Provides tool for malware analysis, hashing, and imaging a hard drive. 
  - https://sumuri.com/software/paladin/
-Remnux
  - Malware reverse engineering tools, with specialized tools made to analyze Windows and Linux malware, suspect documents, and to intercept malicious network traffic. 
- Sans Sift
  - Tools for imaging, memory analysis, and timeline creation. Offered for free by SANS.
  - https://digital-forensics.sans.org/community/downloads

Hardware
  - Write blocker
    - Prevents the write action, so the integrity of the image can be verified. Allows an investigator to capture an image of a hard drive without contaminating the image with their own activities.

Software
  - Autopsy
    - My top choice for forensics tools. Very easy to use interface, and the readouts are human readable. This tool is to be used in windows, its really much easier their. Autopsy is an open source GUI, made to analyze data from a hard drive image. 
    - https://www.sleuthkit.org/autopsy/download.php
  - FTK Imager
    - Imaging tool for data acquision. Used similarly to Autopsy above, can be used on a hard drive image. Not as intuitive nor easy to use as Autopsy. License may be required. Did not find anything with FTK imager that was not already found on autopsy.
  - Grep
    - Often included in linux distros, grep processes a logical boolean based on the criteria fed in. That criteria is usually regex, but different flags can be set to change that. Prints out the true condition, flags changing the read out information. 
  - Netcat
    - Used as a networking utility tool. Used to issue commands remotely from a safe environement to the suspects environment. 
  - OSXPMem
    - Mac tool, used to capture memory. Permissions can be troubling, but following any online guide will navigate through those issues easily. Install on your capture device. Make sure that your external hard drive is formatted correctly. The password was fish.
  - Snort 
    - Open source intrusion prevention system, used for both real-time traffic analysis and offline packet analysis. Can be set with a series of rules to refine searches. Can also be used as a firewall, not as intuitive as pfSense, but still a viable option. Can blacklist/whitelist ips.
    - www.snort.org
  - Suricata
    - Open source threat detection engine. Used to analyze pcaps, filters can be set to refine searches and view information. 
    - www.suricata-ids.org
  - TCPdump
    - Also often included in linux distros. Can be used to parse through pcaps, prints out activity on a network at the current moment.
  - Volatility
    - Open source tool for memory acquisition and analysis. Really easy to use, the help function shows all commands. After selecting the correct profile, all sorts of useful information can be found through the built in commands. Able to see open connections, sockets, processes, etc.
  - Wireshark
    - Classic tool used to analyze network traffic. Filters can be set, and the information is layed out in a fairly intuitive manner. Uses pcaps, has a GUI, but is very memory intensive. Would suggest using on a windows machine.
  - Yara
    - Designed by malware researches, like charles schmoot (sp?), from Sandia. Open source and free to use. Uses regex matching to find malicious code. Lots of research and documentation on how to use, and which regex to try using to find malware. Simple but robust tool.
    - https://yara.readthedocs.io/en/latest

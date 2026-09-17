PM2 — Footprinting & Reconnaissance with GHDB

Module Overview

This module focused on Google Hacking Database (GHDB) techniques for footprinting and reconnaissance.

The activities involved identifying publicly indexed resources using Google search operators and GHDB queries.

Task 1 — Security Camera-Related Results

Objective

Identify publicly indexed security-camera-related resources using GHDB search queries.

Results

Seven relevant results were documented during the exercise using different GHDB queries.

The documented results included:

- WebcamXP-related result
- Publicly indexed `/cam/` directory
- NoVus IP camera login page
- Public webcam page
- Real-time IP camera monitoring system
- Publicly indexed DCIM/Camera directory
- Microseven M7CAM IP camera page

GHDB Techniques Used

Examples of the search patterns used included:

- `intitle:"webcamXP" inurl:8080`
- `intitle:"Index of /cam/"`
- `intitle:"NoVus IP camera" -com`
- `inurl:webcam site:skylinewebcams.com inurl:roma`
- `intext:"Real-time IP Camera Monitoring System" intext:"ActiveX Mode (For IE Browser)"`
- `intitle:"Index of "DCIM/camera"`
- `intitle:"Microseven M7CAM IP Camera"`

The exercise demonstrated how search engines can index publicly accessible camera interfaces and directories.

For responsible disclosure and privacy reasons, specific third-party camera URLs and authentication information are not reproduced in this public repository.

Task 2 — Mathematics PDF Directory Results

Objective

Identify publicly indexed directory listings containing downloadable mathematics-related PDF resources.

Search Query

`intitle:index.of "parent directory" mathematics pdf`

Results

Seven relevant publicly indexed results were documented during the exercise.

The results included directory listings hosted by academic and other publicly accessible websites containing mathematics-related PDF resources.

One verified example was a publicly accessible mathematics PDF directory hosted by Dartmouth College.

The exercise demonstrated how search-engine indexing can expose publicly accessible files and directory structures.

GHDB Concepts Demonstrated

The practical exercise provided experience with:

- Google search operators
- `intitle:` operators
- `inurl:` operators
- `intext:` operators
- `site:` operators
- Directory indexing discovery
- Publicly indexed resources
- Search-engine reconnaissance
- OSINT-based footprinting

Evidence

The practical results were recorded during the exercise and retained in the Week 2 project documentation.

The public repository intentionally avoids reproducing unnecessary third-party camera links, authentication information, or other potentially sensitive details discovered during the exercise.

Responsible Use

GHDB techniques can reveal information that has been indexed by search engines without requiring direct exploitation of the underlying systems.

These techniques should only be used for authorized cybersecurity research, education, security assessment, and responsible disclosure.

Module Status

**Completed**

Networkwalks Cybersecurity Internship

**Batch:** B083  
**Participant:** Dan Ngechu  
**Module:** W2-PM2  
**Activity:** Footprinting & Reconnaissance with GHDB

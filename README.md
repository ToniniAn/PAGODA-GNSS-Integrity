
# PAGODA — Camera-Based GNSS Integrity Monitoring

### Independent GNSS position verification using existing UAV cameras

## Background

GNSS signal degradation, jamming and spoofing can disrupt UAV operations or prevent them from taking place. These risks are an increasingly important concern for UAV operators, including those operating outside conflict zones.

EASA, the FAA and ICAO recognise these risks and promote measures to improve GNSS interference detection, operational resilience and the availability of alternative or complementary positioning and navigation capabilities.

**References:**
- [FAA — GNSS Jamming and Spoofing](https://www.faa.gov/air_traffic/publications/atpubs/aip_html/part2_enr_section_1.16.html)
- [ICAO — GNSS RFI: Medium-Term Actions](https://www.icao.int/air-navigation-bureau/gnss-rfi/roadmap/medium-term-actions)
- [EASA — GNSS Outages and Alterations](https://www.easa.europa.eu/en/domains/air-operations/global-navigation-satellite-system-outages-and-alterations)

## The PAGODA Approach

PAGODA aims to provide independent GNSS position verification by analysing images acquired by the UAV's existing camera and comparing them with available geospatial reference data.

It does not require additional sensors, antennas or payloads and can work with openly available geospatial data. It relies on basic time-synchronised video metadata, without requiring deep integration into existing UAV software. This approach makes it potentially compatible with a wide range of UAV cameras, provided the necessary metadata are available. Accurate camera calibration and lens distortion parameters, when available, may further improve positioning accuracy. 

It is designed to alert operators when the reported GNSS position is inconsistent with the camera-based position estimate, including potentially gradual deviations associated with spoofing.

For advanced UAV platforms already equipped with GNSS protection systems, PAGODA could provide an additional, independent layer of position integrity monitoring. For smaller or less sophisticated UAVs, it could offer an affordable solution for monitoring GNSS position integrity and detecting potential spoofing-related anomalies.

**PAGODA aims to make supplementary GNSS integrity monitoring more accessible.**

It is intended as an advisory system: it does not automatically correct the UAV's position or intervene in flight control.

## Experimental Results

Initial proof-of-concept tests were conducted using recorded DJI drone flight data and simulated GNSS position alterations.

The experiments investigated camera-based positioning, detection of an initially altered GNSS position and detection of gradual position drift.

The results, methodology and limitations are presented in the following report:

**[PAGODA_Project_Case_Study.pdf](PAGODA_Project_Case_Study.pdf)**

*The tests were conducted offline. Live operation and performance under real GNSS interference have not yet been validated.*

## Operational Needs Survey

We invite UAV operators, manufacturers, researchers and developers to share their perspectives on the operational relevance and technical requirements of camera-based GNSS integrity monitoring.

The questionnaire aims to assess practical needs, technical compatibility and the potential usefulness of this approach.

**[Participate in the PAGODA Survey](https://docs.google.com/forms/d/e/1FAIpQLSe4pfuR7qvn452SN8WFtinOZQEudGntUO-CjnVBI-Q86o_lAw/viewform?usp=publish-editor)**

Participation is voluntary. The questionnaire is intended for technical and research purposes.

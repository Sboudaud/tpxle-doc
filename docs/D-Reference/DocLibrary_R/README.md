# Abeeway trackers and location services documentation
This page lists all the documentation available for Abeeway trackers, Abeeway Device Manager and the ThingPark X Location Engine.

## Suggested journey through the documentation
The complete documentation listed below can be a bit overwhelming. We recommend to read the documentation in the following order:
1. Read the out-of-the box notice related to your specific tracker model (which will also provide convenient QR codes pointing to essential documentation). The out-of-the-box document is present in the tracker delivery package or it can be downloaded from [here](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k)
2. Read the training on the tracker Button and LED [User Interface](https://actilitysa.sharepoint.com/:f:/t/aby/EiWIqYpAehBKg3Py8I6X07oBFFxUWT3i2FVHYRX2MzXtow?e=ZFkhrM) and on the [Command Line Interface (CLI)](https://actilitysa.sharepoint.com/:f:/t/aby/EgxRhivJUIVNrq1Lwa3qBigBip9FcMMHhBD_ZaA9m8IT6w?e=WLr48X). Many features require activation by button press sequences or CLI commands, and it is important to be familiar with both.
3. Read the [Abeeway Device Manager (ADM) User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EhbJycLDkulLhGAhJpcOztcBa_glwi7WYyyPMz58f-PEUQ?e=YN9ptc). This easy to use online tool will allow you to interact and configure your trackers without having to know the exact configuration commands or parameter IDs.
4. You will need to tune the tracker's LoRaWAN transmit strategy to your specific use case and network. ADM provides default settings but if you want to optimize power consumption for a given private network you will need to make sure the the datarates used are as high as possible. [AN-002_LoRa_Transmission_strategy](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) provides all the details.
5. You will usually need to understand how to tune the embedded GNSS geolocation logic to optimize power consumption and tune it to your local GNSS reception conditions, or configure aggressive timeouts if you want the tracker to switch to WiFi or BLE geolocation as much as possible. [AN-016_GPS_LPGPS](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) provides the required reference.
6. If you need to understand specific parameters when using the Abeeway Device Manager beyond the tooltip information, you can refer to the [Abeeway Trackers Reference Guide](/AbeewayRefGuide/introduction/). This document is not meant to be read end-to-end, but rather as a comprehensive reference for all commands and parameters.
7. You can more information in [Abeeway Firmware trainings](../../D-Reference/DocLibrary_R/#abeeway-firmware-trainings) and [ThingPark X Location Engine trainings](../../D-Reference/DocLibrary_R/#thingpark-x-location-engine-trainings) below for more specific use cases.

The rest of the documentation relates to specific use cases (e.g. BLE scanning, Covid proximity) or specific actions (Firmware update, debugging), and the titles are self-explanatory. You need to read them only if relevant to you.

## Abeeway trackers

### Reference Guides and Tools

| | Resource |
| - | -------- |
| **Asset tracker firmware**| [Abeeway Trackers Reference Guide](/AbeewayRefGuide/introduction/) |  
| **Asset tracker firmware Release Notes**| [Abeeway tracker Firmware Release notes](https://actilitysa.sharepoint.com/:f:/t/aby/ElJzs_L4X5lDviZbdDBi10wBd9F2VUP19HY52fMxh4Z35g?e=xTkQzY) |  
| **Trackers power consumption estimation**| [Power Consumption Estimation](https://actilitysa.sharepoint.com/:f:/t/aby/Er1CBFg9-YxChO-cdxGs5DUBj2CDpFGEhoEQtFeuH9l_4w?e=xmiDVM) |
| **LED patterns for micro tracker and smart badge** | [LED patterns](https://actilitysa.sharepoint.com/:b:/t/aby/Ee9KhtkknRFMiBipu_fWDdgBh5pr8AIyZNYXkTCe5fg18A?e=DtRe8I) | 
| **Asset tracker driver**| [Asset Tracker Driver User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EhpXO62fGtlEstRRCMq6UAgBRgT_0xLToEZd1k_NyGzCcA?e=HlmwTS) |
| **Melodies for Abeeway Trackers** | [Abeeway trackers melody](https://actilitysa.sharepoint.com/:f:/t/aby/Er982mOeCYxLniE8OjVErKwBopXN9-mKCC7VPn5HsJkigA?e=dCGByt) |

### Out of Box User Guides

| | Resource | 
| - | -------- |
| **Micro tracker**| [Micro tracker Out of Box User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k) |
| **Smart badge** | [Smart Badge Out of Box User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k) |
| **Industrial tracker**| [Industrial Tracker Out of Box User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k) |
| **Compact tracker** | [Compact Tracker Out of Box User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k) |
| **Geolocation Module Discovery kit (EVK)** | [Geolocation Module Discovery kit Out of Box User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EuMzuM_frNdHv_PEqLKPIxsBI83xXlrDeOgdLbe6XnaHoA?e=fnAY2k) |

### Certifications

| | Resource | 
| - | -------- | 
| **Micro tracker V2**| [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/Ep_mMs3nYABNkDSrFgI6lQIB1BMjdShDx1yyL0TPl6i2qg?e=rOCV8O) |
| **Micro tracker V3**| [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/Erlh0hDXjFVGqriKiLVvOggBcbYqBQzxp6iBYc7W3Cfbwg?e=U9pIsa) |
| **Smart badge** | [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/EkooWtJT0vJPv2phGGJHp18BT9988i36qQJzkJ2Rtsq-rA?e=w7mqj8) |
| **Industrial tracker V1** | [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/Eqk_LfFUHJBDotzEK2gdX9IBNXcynn_DlKWKqmuCbOYtnw?e=aGg18b) |
| **Industrial tracker V2** | [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/Ek4c_6w2bOBKuP1Bk2VDSjEB48s56zmOwVpzppyjDF1xSQ?e=wWTbuT) |
| **Compact tracker** | [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/EtWpMlYIt0lGk3o2Nx0hKyMBC52iKMXjW2bAuYoxUdvjYg?e=wgyH4y) |
| **Docking station** | [Certification documents](https://actilitysa.sharepoint.com/:f:/t/aby/EnEQl3ZoI4ZArh073pciqXoBoO706gpO262rev0V38G-gw?e=TAemPx) |

### Abeeway Device Manager application

| | Resource | 
| - | -------- |
| **Abeeway Device Manager** (ADM)| [Abeeway Device Manager User Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EhbJycLDkulLhGAhJpcOztcBa_glwi7WYyyPMz58f-PEUQ?e=YN9ptc) |

### Data sheets

| | Resource | 
| - | -------- | 
| **Micro tracker** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/EgWpgfH_tAZLnWxUvbHik4sBrZndICDdFZH0mOPJv21Y_g?e=n97NzZ) |
| **Smart badge** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/ErQx5OT96LVAuVqNst7mOtEBfDCxo7sbOntVT0smN5EVug?e=ukxqa3) |
| **Industrial tracker** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/Evkh40X6gVlHqFouOdAl4uIBj139ph9fzji835sewtlFVg?e=SVf1m4) |
| **Compact tracker** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/EodEe7JCZFhDgGR_IjtmoJUBB5sj9WhdgPThld6yYXWOwg?e=6e5giY) |
| **Smart badge docking station** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/EvDDLZ6OdzVGrv1O3J5P2aoBjlI_rQrBeaafiawmbFONgA?e=d1EOAw) |
| **Geolocation module** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/EgYK6e26eYdPkTnRaIdN15IBJ3W_Lvi4CEtB6_z6ZMRO8Q?e=73BkwT) |
| **Third party accessories** | [Data sheet](https://actilitysa.sharepoint.com/:f:/t/aby/ErQIOhsLoiVFrDW5dcCW2qcBfdsNMAAIdhlkw5Hww8v0Xw?e=fvzYse) |


### Application notes


<html>
<a id="AN-009"></a>
<a id="AN-001"></a>
</html>

| | Description | Resource | Minimum Required MCU/BLE Firmware Version |
| - | ----------- | -------- |-------- |
| **LoRa transmit strategy** | This application note describes the configuration and usage of LoRaWAN® custom transmit strategy. | [AN-002_LoRa_Transmission_strategy](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 1.9.x, BLE: 2.2.0 |
| **Scan collection** | This feature describes the scan collection feature which allows scanning, filtering and reporting up to twenty BLE beacons in several uplink payloads. | [AN-003_ScanCollection](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.0, BLE: 3.1.0 |
| **Device orientation** | This application note explains how to use the accelerometer data from the tracker to detect its orientation. | [AN-005_device_orientation](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 1.9.x, BLE: 2.2.0 |
| **BLE position filtering** | This application note explains the functionality and configuration of BLE position filtering feature that allows reporting of up to four BLE beacon identifiers with different filtering options on BLE UID. | [AN-006_Position_BLE_filtering](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.1.x, BLE: 3.2.2 |
| **Proximity detection** | This application note describes the Proximity detection feature that can be used for contact tracing and proximity detection between people wearing the Abeeway trackers. | [AN-007_proximity-detection](https://actilitysa.sharepoint.com/:f:/t/aby/EgbhcfgQ-bZPrkYbQ7isqYYBPZkOHvKjhwmED46IDtiimA?e=m0AYsd) | MCU: 2.1.x, BLE: 3.2.2 |
| **Proximity detection calibration guide** | This application note describes the positioning and calibration of badges for proximity detection and contact tracing. | [AN-008_proximity-detection-calibration-guide](https://actilitysa.sharepoint.com/:f:/t/aby/EgbhcfgQ-bZPrkYbQ7isqYYBPZkOHvKjhwmED46IDtiimA?e=m0AYsd) | MCU: 2.1.x, BLE: 3.2.2 |
| **MCU firmware update** | This application note describes the MCU firmware update procedure.**This tool is deprecated since MCU FW 2.2. Please use Abeeway Updater tool (see Firmware Update section below)**.| [AN-009_mcu_firmware_update](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 1.9.x, BLE: 2.2.0 |
| **Angle Detection** | This application note describes how to trigger events from the tracker based on its orientation | [AN-010_Angle_Detection](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **BLE Geozoning** | This application note describes the BLE Geozoning feature which can be used to generate alerts from the tracker based on safe/hazard zone detection using BLE | [AN-011_BLE_geozoning](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **Quuppa Beaconing** | This application note describes the Quuppa beaconing feature. | [AN-012_Quuppa_beaconing](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **CLI Usage** | This application note describes the debugging of the tracker over USB interface. | [AN-013_CLI_Description](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **BLE Communication** | This application note describes the interface between the tracker and the mobile APP | [AN-014_BLE communication](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **Debug Trackers** | This application note describes how to debug Abeeway trackers when there is reset or any other unexpected cause| [AN-015_Debug data](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=2DqzTy) | MCU: 2.2.x, BLE: 3.3.0 |
| **GPS/LPGPS Usage** | This application note describes how to configure and use the GPS/LP-GPS feature to optimize accuracy/power consumption of the tracker | [AN-016_GPS_LPGPS](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **Getting started with Mobile APP** | This application note describes how to configure and use the Abeeway mobile APP with the trackers | [AN-017_Mobile APP Getting Started Guide](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.2.x, BLE: 3.3.0 |
| **Motion and Shock detection** | This application note describes how to configure the firmware for motion and shock detection) | [AN-018_Motion_and_shock_detection_V1.0](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.3.x, BLE: 3.3.2 |
| **BLE beaconing** | This application note describes how to configure the firmware to send BLE beacons (iBeacon, Eddystone and Altbeacon) | [AN-019_BLE Beacon transmission](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) | MCU: 2.3.x, BLE: 3.3.2 |


### Firmware Update

| | Description | Resource | 
| - | ----------- | -------- |
| **Abeeway Updater (Firmware Update tool)** | This tool allows MCU and BLE Firmware update of Abeeway trackers. | [Abeeway Firmware Update](https://github.com/Abeeway/Abeeway-updater) |
| **MCU Firmware binaries** | This folder has all the binaries for MCU/Application Firmware. | [ MCU Firmware binaries](https://actilitysa.sharepoint.com/:f:/t/aby/EstKVz_aVwRKkhcNATWI3loBEIgAAIxE0j_Sx8oZ5oiAew?e=g5Op9r) |
| **BLE Firmware binaries** | This folder has all the binaries for BLE Firmware. | [BLE Firmware binaries](https://actilitysa.sharepoint.com/:f:/t/aby/ElfViYe0P9BDiDQYQ9Tv0tYBr3yJpFNa1At2EzVxPujGPw?e=i6sw9e) |
| **Config files** | This folder has all the Firmware config files for different trackers. | [Abeeway Firmware Update](https://actilitysa.sharepoint.com/:f:/t/aby/ErEQcpIhgN9Khxt8q66GBy4Bj9FIV-0rGf5XhaVyCJo2CQ?e=QqegCQ) |
| **BLE firmware update** | This application note describes the BLE firmware update procedure using Nordic NrfConnect smartphone application. | [AN-001_ble-update](https://actilitysa.sharepoint.com/:f:/t/aby/Evqx0qp6AQ1OqrI7-2DoIxsB1wKjLBjykfPh2p7Lo8mP7g?e=VrNdaS) |

### Abeeway Firmware trainings

| | Description | Resource | 
| - | ----------- | -------- |
| **User Interface** | These training slides introduce the user interface (LED, buzzer, button) for Abeeway trackers. | [User Interface](https://actilitysa.sharepoint.com/:f:/t/aby/EiWIqYpAehBKg3Py8I6X07oBFFxUWT3i2FVHYRX2MzXtow?e=ZFkhrM) |
| **Proximity Policy Enforcement** | These training slides introduce basic concepts of proximity solution and how to set it up. | [Proximity Solution](https://actilitysa.sharepoint.com/:f:/t/aby/Eux5K7WVG8JClipPzZsJn7YB4snhG68oscKKw89g20UwRw?e=xqY4gZ) | 
| **Scan Collection** | This feature introduces BLE/WiFi scanning and reporting of up to 20 BLE Beacons/WiFi BSSIDs. | [Scan Collection](https://actilitysa.sharepoint.com/:f:/t/aby/ErgX0cSv_8dNgJZsYVbYVdAB3G-5rve_CK8dHQ1a2dSGkQ?e=6Q2Q47) |
| **BLE Position Filtering** | This feature introduces BLE position reporting of up to 4 BLE beacons. | [BLE Position Filtering](https://actilitysa.sharepoint.com/:f:/t/aby/EpG2Vos3eFxMkSFyWBrkNI8BEBiGorNXW-34K37-NFo-_w?e=4EnC2q) |
| **CLI Usage** | This feature allows to interact with tracker over USB to get the internal logs and also set the tracker parameters. | [CLI Usage](https://actilitysa.sharepoint.com/:f:/t/aby/EgxRhivJUIVNrq1Lwa3qBigBip9FcMMHhBD_ZaA9m8IT6w?e=WLr48X) |
| **Quuppa Beaconing** | This feature enables Quuppa beaconing for Abeeway trackers. | [Quuppa Beaconing](https://actilitysa.sharepoint.com/:f:/t/aby/EucRGJmCxnJEv_QCWbvL58YBkwyfz8RWgTmxU6YMwKJfkg?e=CE7yUH) |
| **BLE Geozoning** | This feature enables BLE geozoning for Abeeway trackers. | [BLE geozoning](https://actilitysa.sharepoint.com/:f:/t/aby/EoMeflwX2UdBnUhmVmwYfOYBYjFIIYupWFfgyNsW2uQvOQ?e=ffx9va) |
| **Abeeway Mobile App** | This feature explains how to use Abeeway Mobile for Abeeway trackers. | [Abeeway Mobile App](https://actilitysa.sharepoint.com/:f:/t/aby/Ep7oeKyEGeZIolF4avQrmf8BBsOOJoFQhjon7jacL4Koig?e=KgYKLP) |

## ThingPark X Location Engine

### ThingPark X Location Engine Trainings

| | Description | Resource | 
| - | ----------- | -------- |
| **ThingPark Location Introduction** | These training slides introduce basic features of ThingPark Location. | [ThingPark Location Introduction](https://actilitysa.sharepoint.com/:f:/t/aby/EqVIEMaqJfVHoNAi90G068UB8K4HMfB1t2eyttWIGlIwbQ?e=JZYdsp) |

### ThingPark X Location Engine Usage

<html>
<table>
    <tr>
        <th>
        </th>
        <th>
            Resource
        </th>
    </tr>
    <tbody>
    <tr>
        <td>
            API
        </td>
        <td>
            <ul>
                <li>
                    <a href="../../B-Feature-Topics/IntegrateAppwithTPLocation_C/">
                        API Overview
                    </a>
                </li>
                <li>
                    <a href="https://dx-api.thingpark.io/getstarted/#/">
                        API Getting Started
                    </a>
                </li>
                <li>
                    <a href="https://dx-api.thingpark.io/location/latest/doc/index.html">
                        API online documentation
                    </a>
                </li>
                <li>
                    <a href="https://dx-api.thingpark.io/location/latest/swagger-ui/index.html?shortUrl=tpdx-location-api-contract.json">
                        API - Swagger
                    </a>
                </li>
                <li>
                    <a href="https://dx-api.thingpark.io/location/latest/tpdx-location-api-contract.json">
                        OPEN API contract
                    </a>
                </li>
            </ul>
        </td>
    </tr>
    </tbody>
</table>
</html>

## ThingPark Market offers

|  | Resource |
| ------------ | -------- |
| For a **private** connectivity network | [Low-Power Location for Private Network Guide](https://actilitysa.sharepoint.com/:f:/t/aby/EkVaNRWQacRLkwOlneNsC3EBPahvZZCOdMRPiJYcH0F4KQ?e=M5NrCz). **This link is deprecated. Please click [here](../../../C-Procedure-Topics/GetStartedAEK_T/) if you bought the marketplace package recently.** |
| For a **public** connectivity network | [Low-Power Location for Public Network Guide](https://actilitysa.sharepoint.com/:f:/t/aby/ErzF-smKHfhKjHbcyiIS7wwBNO3IdQTgCCnJgJTFR0Cj-Q?e=Qq6wCm). **This link is deprecated. Please click [here](../../../C-Procedure-Topics/GetStartedAEK_T/) if you bought the marketplace package recently.** |

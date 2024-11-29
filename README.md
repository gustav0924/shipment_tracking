![banner](assets/banner.webp)
# Logistics Shipment Tracking
## Authors
-  [@gustav0924](https://www.github.com/gustav0924)
## Overview
This project automates the process of tracking shipments across multiple carriers (UPS, FedEx, DHL) and integrating the tracking information with an SAP system. It was developed to streamline the monitoring of inbound deliveries, improve accuracy in estimated delivery dates, and potentially automate updates to delivery dates within SAP.

## Tech Stack
This project utilizes the following technologies:
* **Programming Language:** Python
* **SAP Automation:** `win32com`
* **Web Scraping:** `selenium`, Microsoft Edge WebDriver
* **API Interaction:** `requests`, `http.client`, DHL Express Track API, FedEx Tracking API
* **Data Processing:** `pandas`
* **Configuration:** `configparser`

## Quick glance at the results

| InboundDelivery  | MaterialKey 	    | Description | DeliveryQuantity | Means of Transport - Key	|  Bill of landing - Key |    Due Date        | trackingnumber     |     status  | estimatedTimeofDelivery | Carrier	Source	  | DateCalculated | Action |
|-------------------	        |------------------	|------------- |--------------|---------------- |------------ |-------------- |------------| ------------------------------ || ------------------------------ |
|184228431	| 740375-0020  |  VOICE COIL,19.6X5.9.1.5OHM,NO TINSEL |  21,600      | 1021216221      |	773412432028 |   21/09/2023  0:00:00  |      773412432028   |     Ready for pickup    | 2023-05-15 00:00:00 | FEDEX	| Bill    | 2023-05-17 00:00:00	| Pending To Receive






Program result becomes an xlsx file

![screenshot](assets/screenshot.png)

## Additional Files
SAP python file that can be used for further development
individual REST API python file for FEDEX and DHL

## Repository Structure

```
├── assets
│   ├──  Manual.ipynb                              <- python notebook as manual sample 
│   ├──  stmp.py                                   <- stmp python module 
|
|
├── assets
│   ├──  banner.png                                <- banner file for README
│   ├──  screenshot.png                            <- screenshot sample of program running
│
|
├── datasets
│   ├── 09252023_webdata.xlsx                    <- the dataset created as an xlsx file
│   ├── ListPart.xlsx                            <- the dataset used to extract data and search each material part
│
│
├── LICENSE                                       <- license file.
│
|
├── README.md                                     <- this readme file.

```

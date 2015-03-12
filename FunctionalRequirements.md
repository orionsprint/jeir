#Functional Requirements of Mobicents EIR

# Introduction #

Below is the requirements for Mobicents EIR Platform

  * EIR should receive IMEI and may receive IMSI from MSC through checkIMEI MAP Message.
  * EIR should validate the IMEI size with 15 digits. Should have a switch to turn-on or turn-off answering blackList or whiteList respectively.
  * EIR should have a RBI List Status (RBI: Reporting Body Identifier – is the first two digits of IMEI). RBI should be in activated or deactivated mode. Should be able to activate for instance RBI 01 and to deactivate for RBI 30. And should be possible to work with a range, for instance 02-09 activated and 54-85 deactivated.
  * If RBI is deactivated, EIR should answer blackList.
  * EIR should have a list of IMEI and/ or IMSI with status white or black.
  * User should be capable to turn-on and turn-off monitoring for what was answered to one IMEI. A kind of trace. Should be stored.
  * User should be able to create a black list of IMEIs and/or IMSI. This is a group of IMEIs and/or IMSIs with black status.
  * User should be able to create a white list of IMEIs and/or IMSI. This is a group of IMEIs and/or IMSIs with white status.
  * User should be able to deactivate the blackList.
  * User should be able to deactivate the whiteList.
  * User should be able to provision one list through csv file.
  * User should be able to provision one-by-one IMEI inside black or white list.
  * User should be able to provision one-by-one IMEI and IMSI inside black or white list.
  * EIR should store the list creation date.
  * EIR should store the username that created the list.
  * EIR should store the username that deactivated the list.
  * EIR should store the date that the list was deactivated.
  * EIR should store the creation date of RBI.
  * EIR should store the username that created the RBI.
  * EIR should store the date that the RBI was deactivated.
  * EIR should store the username that deactivated the RBI.
  * User should be able to query some IMEI and/or IMSI inside a list.
  * User should be able to generate reports from his query.
  * User should be able to give a name to one list.
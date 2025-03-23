# Description

Fork of ES8266 nonOS SDK, focused on fixing some issues and getting rid of proprietary components.

The goal is to keep essential libraries, not tied to Espressif technologies, providing an SDK that can be used on Green-Keeper IoT projects.

## Open source libraries

### Present on original SDK

These libraries were ported to work with ESP8266, and provided on original SDK.

Are libraries ready to use and deal with most protocols that goes above the Wi-fi stack:

* From src/third_party
  * `liblwip.a` - Lightweight IP (lwIP) TCP/IP stack
  * `libmbedtls.a` - SSL/TLS Protocol Implementation
  * `libjson.a` - SICS JSON

* From src/driver_lib
  * `libdriver.a` - Drivers for I2C, SPI, UART

## Ommited from original SDK

These libraries were ported to work with ESP8266, but we don't know how,

They were ommited from original SDK, and basically deal with most of Wi-fi stack:

* [WPA Suplicant](https://github.com/digsrc/wpa_supplicant)
  * `libcrypto.a` - Crypto / Hashing functions
  * `libwpa.a` - Wi-fi WPA (wi-fi protected access)
  * `libwpa2.a` - Wi-fi WPA2 (wi-fi protected access v2)
  * `libwps.a` - Wi-fi WPS (wi-fi protected setup)


* [FreeBSD Wifi Stack](https://github.com/freebsd/freebsd-src/tree/23db5fccb60a1b008c7cbd3a6b88f9a6b1bac167/sys/net80211)

  * `libnet80211.a` - Wi-fi MAC IEEE 802.11


# Proprietary

These libraries are totally proprietary.

There are some open source versions, from reverse engineering process, but most found so far are not quite accurate:

* Essential for most applications
  * `libmain.a` - Main application framework (a kitchen sink)
  * `libpp.a` - Wi-fi PP (protocol processing)
  * `libpy.a` - Wi-fi PHY (physical layer)
  * `libc.a` - C support functions
  * `libgcc.a` - GCC support functions
  * `libhal.a` - Hardware abstraction layer (very obscure)


* Non-essential for most applications
  * `libairkiss.a` - Wifi AirKiss
  * `libat.a` - AT command firmware
  * `libespnow.a` - ESP-NOW protocol implementation
  * `libpwm.a` - Pulse Wave Modulation from software
  * `libsmartconfig.a` - Wifi Smart Config
  * `ligssl.a` - SSL features (very obscure)
  * `libupgrade.a` - OTA upgrades self managed (system_upgrade_start)
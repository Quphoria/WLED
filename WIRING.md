# ESP32 Dance Floor Controller With Ethernet & OLED
## Ethernet Wiring
| -- | ------------------------------------------------------------------------------ |
| 21 | RMII EMAC TX EN  == When high, clocks the data on TXD0 and TXD1 to transmitter |
| 19 | RMII EMAC TXD0   == First bit of transmitted data                              |
| 22 | RMII EMAC TXD1   == Second bit of transmitted data                             |
| 25 | RMII EMAC RXD0   == First bit of received data                                 |
| 26 | RMII EMAC RXD1   == Second bit of received data                                |
| 27 | RMII EMAC CRS_DV == Carrier Sense and RX Data Valid                            |

## esp32dancefloorcontroller_eth_oled
| -------------------------- | ------------ |
| 1 (ADDRESS NOT GPIO)       | eth_address  |
| -1 (Use Internal Osc)      | eth_power    |
| 16 (RX2)                   | eth_mdc      |
| 18                         | eth_mdio     |
| ETH_PHY_LAN8720            | eth_type     |
| ETH_CLOCK_GPIO17_OUT (TX2) | eth_clk_mode |

## Led Outputs
| -- | ----- |
| 12 | LED 1 |
| 13 | LED 2 |

## OLED
| -- | --- |
| 15 | SDA |
| 2  | SCL | 

New:
| -- | --- |
| 14 | SDA |
| 4  | SCL | 
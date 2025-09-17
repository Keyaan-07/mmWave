# mmWave Radar
This project includes building a complete mmWave radar that could operate at 60GHz. It uses the Texas Instruments IWRL6432 as the radar IC. This radar IC is operable between 57GHz-64GHz. The main goal of this project is to make a small module to use this IC as a radar. 
The board is a 6 layer board(4 layer was possible but 6 layers was cheaper). The 6 layer board costs only $2. 

[KICANVAS](https://kicanvas.org?)

# Images
Schematic:  
![schematic](/images/sept6/schematic.png)  
PCB:  
![PCB1](/images/sept17/pcb1.png)
![PCB2](/images/sept17/pcb2.png)
3d: 
![3d1](/images/sept17/3d1.png)
![3d2](/images/sept17/3d2.png)

# BOM
because the top sides contains BGA footprint which i've never soldered before, i am doing PCBA services for the top side and i will assemble the bottom side by myself
| ITEM                        | COST  | NOTE                           |
| --------------------------- | ----- | ------------------------------ |
| PCB                         | 2     | 6-Layer PCB                    |
| PCBA                        | 51.71 | PCBA service from jlcpcb.com   |
| SHIPPING from JLC           | 9.28  | shipping cost                  |
| PCBA discount               | -15    | 15 USD coupon from JLCONE yayy(valid till 19 sept) |
| LCSC Total (BOM_PCB_Bottom) | 14.55 | bottom side all parts          |
| Total                       | 62.54 | USD                            |

----
### BOM - Top Side of PCB(PCBA recommened)
| Designator                          | Designation      | Footprint                              | Price   | Quantity(for 2 PCBA) | Amount(USD) | JLCPCB Part Number |
| ----------------------------------- | ---------------- | -------------------------------------- | ------- | -------------------- | ----------- | ------------------ |
| C1, C2                              | 15p              | 402                                    | 0.001   | 4                    | 0.004       | C1548              |
| C6, C8, C10, C12, C14               | 2u2              | 603                                    | 0.006   | 10                   | 0.06        | C23630             |
| C5, C11, C13, C18, C19, C25, C7, C9 | 10u              | 603                                    | 0.056   | 16                   | 0.896       | C19702             |
| R2, R3                              | 100k             | 402                                    | 0.001   | 2                    | 0.002       | C25741             |
| R4, R5, R6                          | 10k              | 402                                    | 0.001   | 3                    | 0.003       | C25744             |
| U1                                  | IWRL6432BDBAAMFR | BGA-102_L6.5-W6.5-P0.50-TL_TI_IWRL6432 | 16.0095 | 2                    | 32.019      | C22428198          |
| U2                                  | W25Q128JVS       | SOIC-8_5.3x5.3mm_P1.27mm               | 1.131   | 2                    | 2.262       | C97521             |
| U3                                  | AMS1117-3.3      | SOT-223-3_TabPin2                      | 0.1615  | 2                    | 0.323       | C6186              |
|                                     |                  |                                        |         | Total                | 35.569      |                    |
| PCB Cost                            | 2                | USD                                    |         |                      |             |                    |
| Economic PCBA price                 | 51.71            | USD                                    |         |                      |             |                    |
| Total                               | 53.71            | USD                                    |         |                      |             |                    |


----
### BOM - bottom side of PCB(order and solder yourself)
if DNO is yes, i am not ordering the respective parts and cost has not been added to BOM.
| Designator             | Designation        | Footprint                          | DNO - Do not order | MOQ | Price  | Quantity | Amount(USD) | Supplier link                                      |
| ---------------------- | ------------------ | ---------------------------------- | ------------------ | --- | ------ | -------- | ----------- | -------------------------------------------------- |
| C3, C20, C22, C23, C24 | 10u                | 603                                | No                 | Yes | 0.0197 | 20       | 0.394       | https://www.lcsc.com/product-detail/C7393892.html  |
| C4, C21                | 2u2                | 603                                | No                 | Yes | 0.0228 | 20       | 0.456       | https://www.lcsc.com/product-detail/C48579298.html |
| C15                    | 47n                | 402                                | Yes                | \-  | 0      | 1        | 0           | https://www.lcsc.com/product-detail/C5142571.html  |
| C16, C17               | 1u                 | 603                                | No                 | Yes | 0.0056 | 50       | 0.28        | https://www.lcsc.com/product-detail/C29936.html    |
| L1                     | 470n               | 805                                | No                 | Yes | 0.098  | 5        | 0.49        | https://www.lcsc.com/product-detail/C45385171.html |
| L2                     | 100n               | 805                                | No                 | Yes | 0.098  | 5        | 0.49        | https://www.lcsc.com/product-detail/C45385168.html |
| R1                     | 10k                | 402                                | Yes                | \-  | 0      | 1        | 0           | https://www.lcsc.com/product-detail/C3020235.html  |
| R7                     | 100k               | 402                                | No                 | Yes | 0.0277 | 20       | 0.554       | https://www.lcsc.com/product-detail/C313329.html   |
| R8                     | 18k                | 402                                | No                 | Yes | 0.005  | 10       | 0.05        | https://www.lcsc.com/product-detail/C2759512.html  |
| U4                     | TPS628502QDRLRQ1   | SOT-583-8_L2.1-W1.2-P0.50-LS1.6-BR | No                 | No  | 1.94   | 3        | 5.82        | https://www.lcsc.com/product-detail/C3193229.html  |
| Y1                     | 40MHz Crystal      | Crystal_SMD_3225-4Pin_3.2x2.5mm    | No                 | Yes | 5      | 0.1679   | 0.8395      | https://www.lcsc.com/product-detail/C18221410.html |
| J1                     | Connector_02x08    | connector_pin2.54mm                | No                 | Yes | 5      | 0.0586   | 0.293       | https://www.lcsc.com/product-detail/C42431811.html |
|                        |                    |                                    |                    |     |        |          |             |                                                    |
|                        | Merchandise total: | 7.88                               | USD                |     |        |          |             |                                                    |
|                        | Shipping           | 3.77                               | USD                |     |        |          |             |                                                    |
|                        | Handling charges   | 3                                  | USD                |     |        |          |             |                                                    |
|                        | Discount           | \-0.1                              | USD                |     |        |          |             |                                                    |
|                        | Total              | 14.55                              | USD                |     |        |          |             |                                                    |

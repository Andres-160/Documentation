The antennas are a key component for any radio link solution and the same   for radio waves are applicable here. The right combination depends on the objectives, like short-range (all-around flight) or long-range flight for more advanced pilots. A good starting point is the default antennas for the wifi cards at the workbench (omnidirectional), once you get confident with the system during a line of sight and short flights, you can move with directional antennas. 

As nothing is free, changing your antennas is a trade-off, while omnidirectional antennas give you autonomy to fly around your position, these antennas offer limited range, on the other side directional antennas concentrate the radiated pattern and allow a long-range at the cost of the need of pointing the antennas precisely, in other words, more antenna gains more directional. For the high directive antenna, add components like trackers are recommended to keep always pointing the main antenna pattern lobule to the aircraft.

### 5 TIPs for Antennas
1. Make sure you have proper wiring and you have followed all previous sections, wrong connections can lower your range or destroy your radio link.
2. Start simple using Omni antennas, and move with directional ones as you get more experience. 
3. Make sure you use the same polarization on both sides, Vertical/Vertical, Horizontal/Horizontal. The cross-polarization can work but you will lose 3dB (half of the power).
4. Lower bands like 2.4GHz can benefit the range, however, in some areas, this band is highly polluted and you may consider 5.8GHz. Try changing also the channels in the selected band. 
5. When using directional antennas meant to ground side, always aligned with the airside, consider using ATT (automatic antenna tracker). Omnidirectional antennas are always recommended in the Airside.

The below link explains how the video quality is impacted under different scenarios.
https://www.youtube.com/watch?v=T78JRAELjec

### Range Calculation 
A typical question is related to the maximum range, link budget or system range have relation to three main elements: Transmitter power, Antenna gains, and Receiver sensitivity. The next formula can be used to calculate  this:

`R = 10^( (Lfs-LM-32.44-20*Log(f)) / 20)`

`Lfs =  Ptx + Gtx + Grx – Srx `

 where,
* `R = range in Km`
* `f = frequency used MHz` 
* `LM = Link Margin dB`
* `Lfs = free space path loss dB`
* `Gtx = Tx antenna gain dBi`
* `Grx = Rx antenna gain dBi`
* `Ptx = Tx power dBm`
* `Srx = Sensitivity Rx`
* `Srx = Sensitivity Rx`

| Ground Side antenna / Gain | Air Side antenna / Gain | Frequency GHz | Power TX mW | Theoretical range Km * | Notes |
|:---:|:---:|:---:|:---:|:---:|:---:|  
| Maple 5dB Omni  / 5dBi | Maple 5dBi Omni / 5dBi | 5.2GHz | 200 | 2.9 | Excellent upgrade for default antennas | 
| Flat Panel Direct / 14dBi | Maple 5dBi / 5dBi | 5.2GHz | 200 | 8.2 | Directional antenna with ATT |
| Planar Direct / 17dBi | Omni / 5dBi | 5.8GHz | 500 | 16.37 | Directional antenna high range ATT |

*Network card receiving sensitivity approx. -93dBm
¡Link margin assumed 10 dB


***

| Brand | Antenna | Polarization | Frequency GHz | Link * |
|:---:|:---:|:---:|:---:|:---:|  
| Maple | Flat Panel FY-05A | Vertical | 5.8G | [Maple leaf 14dB](https://de.aliexpress.com/item/1005002363442414.html?spm=a2g0o.detail.1000060.1.503d7a06Df2DUH&gps-id=pcDetailBottomMoreThisSeller&scm=1007.13339.169870.0&scm_id=1007.13339.169870.0&scm-url=1007.13339.169870.0&pvid=30e1916d-79e8-4bfb-83ba-eef6777847aa&_t=gps-id:pcDetailBottomMoreThisSeller,scm-url:1007.13339.169870.0,pvid:30e1916d-79e8-4bfb-83ba-eef6777847aa,tpp_buckets:668%230%23131923%2335_668%230%23131923%2335_668%23888%233325%2315_668%23888%233325%2315_668%232846%238112%231997_668%235811%2327188%2383_668%232717%237558%23140_668%231000022185%231000066058%230_668%233468%2315612%23327_668%232846%238112%231997_668%235811%2327188%2383_668%232717%237558%23140_668%233164%239976%23381_668%233468%2315612%23327) |
| Maple | Planar Antenna  | Vertical | 5.8G | [Planar 17dB](https://de.aliexpress.com/item/32989509234.html?spm=a2g0o.detail.1000014.1.61b153755LLnFy&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.13338.192131.0&scm_id=1007.13338.192131.0&scm-url=1007.13338.192131.0&pvid=1dfa41c1-d87c-4da2-8620-67be3840574e&_t=gps-id:pcDetailBottomMoreOtherSeller,scm-url:1007.13338.192131.0,pvid:1dfa41c1-d87c-4da2-8620-67be3840574e,tpp_buckets:668%230%23131923%2378_668%23888%233325%2320_3338%230%23192131%230_3338%233142%239890%238_668%232846%238107%231934_668%232717%237565%23731_668%231000022185%231000066059%230_668%233422%2315392%23445) |

*Links are only for reference purposes. 

under construction, it will be added more as users test.  
